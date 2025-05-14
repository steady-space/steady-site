+++
title = "Products"
date = 2025-05-13T12:34:28-05:00
draft = false
type = "page"
+++

Welcome to **steady space** — a calming hub of digital tools and gentle guidance.  
Crafted for the dreamers, doers, and those trying again.

<br>

<div class="product-grid">

  <div class="product-card">
    <div class="product-image-banner" style="background-image: url('/images/zen-toolkit-cover.png');"></div>
    <h2>🧘 Zen Toolkit</h2>
    <p>The complete calming bundle — includes the full book, companion Field Notes, and reflective prompts.</p>
    <a href="https://gum.new/gum/cmalnfax9001k03jo64ztd8y6" target="_blank" class="product-button">→ View Product</a>
  </div>

  <div class="product-card">
    <div class="product-image-banner" style="background-image: url('/images/lotus-icon.png');"></div>
    <h2>📖 Zen Sample Chapter</h2>
    <p>A free preview of the full Zen Toolkit. For when you just want to dip your toes into something calm and grounding.</p>
    <a href="https://gum.new/gum/cmamtgpg3001v03l130i43rhz" target="_blank" class="product-button">→ Try Free Chapter</a>
  </div>

  <div class="product-card">
    <div class="product-image-banner" style="background-image: url('/images/lotus-icon.png');"></div>
    <h2>💼 Calm Job Search Tracker</h2>
    <p>A peaceful Notion dashboard for hopeful job seekers. Made to reduce stress — not add to it — while you organize and navigate your path.</p>
    <a href="https://gum.new/gum/cmamt2a4f000l03l1axlgge2d" target="_blank" class="product-button">→ View Product</a>
  </div>

</div>

<br><br>

{{< rawhtml >}}
<section class="latest-note">
  <h2 class="section-title">📝 latest field note</h2>
  {{ $recent := first 1 (where site.RegularPages "Section" "field-notes") }}
  {{ range $recent }}
    <div class="note-preview">
      <h3 class="note-title">
        <a href="{{ .RelPermalink }}">{{ .Title | lower }}</a>
      </h3>
      <p class="note-description">{{ .Params.description }}</p>
      <a href="{{ .RelPermalink }}" class="product-button">→ Read more</a>
    </div>
  {{ end }}
</section>
{{< /rawhtml >}}
