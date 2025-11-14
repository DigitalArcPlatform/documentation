---
title: Home
layout: home
nav_order: 1
---

# Archiving Out of the Box

Our DigitalArc toolkit provides an easy-to-edit template for community-storytelling and archiving projects, from pre-event planning through storytelling collection to publishing a digital archive of the event

<!-- ================== TABLE OF CONTENTS ================== -->
{%- assign collection_labels = site.collections | map: "label" -%}
{%- if collection_labels contains "docs" -%}
  {%- assign all_pages = site.collections["docs"].docs | where_exp: "d","d.output != false" -%}
{%- else -%}
  {%- assign all_pages = site.pages | where_exp: "d","d.output != false" -%}
{%- endif -%}

{%- comment -%}
Build a normalized list of ONLY docs/**/index.md pages, capturing:
  depth  = 1|2|3  (# of folders between 'docs/' and 'index.md')
  top    = first folder after docs/
  second = second folder (if depth >= 2)
  third  = third folder (if depth >= 3)
  ord    = nav_order (default 999999)
  url    = page.url
  ttl    = page.title
{%- endcomment -%}
{%- assign normalized = "" -%}
{%- for d in all_pages -%}
  {%- if d.path contains 'docs/' and d.path contains '/index.md' -%}
    {%- assign rel = d.path | remove_first: 'docs/' -%}
    {%- assign parts = rel | split: '/' -%}
    {%- assign parts_size = parts | size -%}
    {%- assign depth = parts_size | minus: 1 -%}

    {%- if depth >= 1 and depth <= 3 -%}
      {%- assign top    = parts[0] -%}
      {%- assign second = '' -%}
      {%- assign third  = '' -%}
      {%- if depth >= 2 -%}{%- assign second = parts[1] -%}{%- endif -%}
      {%- if depth >= 3 -%}{%- assign third  = parts[2] -%}{%- endif -%}
      {%- assign ord = d.nav_order | default: 999999 -%}
      {%- capture row -%}{{ depth }}|||{{ top }}|||{{ second }}|||{{ third }}|||{{ ord }}|||{{ d.url }}|||{{ d.title | strip }}{%- endcapture -%}
      {%- assign normalized = normalized | append: row | append: "~~" -%}
    {%- endif -%}
  {%- endif -%}
{%- endfor -%}
{%- assign rows = normalized | split: "~~" | reject: "" -%}

{%- comment -%}
Helpers to gather sorted groups
{%- endcomment -%}
{%- assign top_items = "" -%}
{%- for r in rows -%}
  {%- assign c = r | split: "|||" -%}
  {%- if c[0] == '1' -%}
    {%- assign top_items = top_items | append: c[4] | append: "@@" | append: r | append: "~~" -%}
  {%- endif -%}
{%- endfor -%}
{%- assign top_items = top_items | split: "~~" | reject: "" | sort_natural -%}

<div class="toc">
  <h2>Table of Contents</h2>

  <ol>
  {%- for ti in top_items -%}
    {%- assign tb = ti | split: "@@" -%}
    {%- assign trow = tb[1] -%}
    {%- assign tcols = trow | split: "|||" -%}
    {%- assign top_slug = tcols[1] -%}
    {%- assign top_url  = tcols[5] -%}
    {%- assign top_ttl  = tcols[6] -%}
    <li>
      <!-- TOP LEVEL LINKS TO PAGE URL -->
      <a href="{{ top_url | relative_url }}">{{ top_ttl }}</a>

      {%- comment -%} Gather second-level index pages under this top folder {%- endcomment -%}
      {%- assign seconds = "" -%}
      {%- for r in rows -%}
        {%- assign c = r | split: "|||" -%}
        {%- if c[0] == '2' and c[1] == top_slug -%}
          {%- assign seconds = seconds | append: c[4] | append: "@@" | append: r | append: "~~" -%}
        {%- endif -%}
      {%- endfor -%}
      {%- assign seconds = seconds | split: "~~" | reject: "" | sort_natural -%}

      {%- if seconds != empty -%}
      <ul>
        {%- for si in seconds -%}
          {%- assign sb = si | split: "@@" -%}
          {%- assign srow = sb[1] -%}
          {%- assign sc = srow | split: "|||" -%}
          {%- assign sec_slug = sc[2] -%}
          {%- assign sec_url  = sc[5] -%}
          {%- assign sec_ttl  = sc[6] -%}
          <li>
            <!-- SECOND LEVEL LINKS TO PAGE URL -->
            <a href="{{ sec_url | relative_url }}">{{ sec_ttl }}</a>

            {%- comment -%} Third-level index pages under this second folder {%- endcomment -%}
            {%- assign thirds = "" -%}
            {%- for r3 in rows -%}
              {%- assign c3 = r3 | split: "|||" -%}
              {%- if c3[0] == '3' and c3[1] == top_slug and c3[2] == sec_slug -%}
                {%- assign thirds = thirds | append: c3[4] | append: "@@" | append: r3 | append: "~~" -%}
              {%- endif -%}
            {%- endfor -%}
            {%- assign thirds = thirds | split: "~~" | reject: "" | sort_natural -%}

            {%- if thirds != empty -%}
            <ul>
              {%- for th in thirds -%}
                {%- assign tb3 = th | split: "@@" -%}
                {%- assign trow3 = tb3[1] -%}
                {%- assign tc3 = trow3 | split: "|||" -%}
                {%- assign third_url = tc3[5] -%}
                {%- assign third_ttl = tc3[6] -%}
                <!-- THIRD LEVEL LINKS TO PAGE URL -->
                <li><a href="{{ third_url | relative_url }}">{{ third_ttl }}</a></li>
              {%- endfor -%}
            </ul>
            {%- endif -%}

          </li>
        {%- endfor -%}
      </ul>
      {%- endif -%}
    </li>
  {%- endfor -%}
  </ol>
</div>

