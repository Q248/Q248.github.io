---
layout: page
title: Protocols
permalink: /protocols/
description: Protocols I use and share. Click a name to read it, or the PDF icon to download.
nav: true
nav_order: 3.5
---

<ul class="qy-protocols">
{%- for p in site.data.protocols -%}
<li>
<div class="qy-protocol-text">
<a class="qy-protocol-title" href="{{ p.page | relative_url }}" target="_blank" rel="noopener">{{ p.title }}</a>
{%- if p.description -%}<div class="qy-protocol-desc">{{ p.description }}</div>{%- endif -%}
</div>
{%- if p.pdf -%}<a class="qy-protocol-pdf" href="{{ p.pdf | relative_url }}" download title="Download PDF"><i class="fa-solid fa-file-pdf"></i></a>{%- endif -%}
</li>
{%- endfor -%}
</ul>