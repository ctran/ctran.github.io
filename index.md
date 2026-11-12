---
layout: splash
title: Cuong Tran
header:
  overlay_color: "#0d1117"
  overlay_filter: 0.2
  actions:
    - label: "See my projects"
      url: "#projects"
    - label: "GitHub"
      url: "https://github.com/ctran"
excerpt: "Software engineer at ServiceNow in San Diego, CA. I build developer tools and maintain open source."
intro:
  - excerpt: "Hi, I'm Cuong, a software engineer at ServiceNow. I maintain open source tools for **Ruby on Rails** and **Java**, and tinker with **Nix** packaging in my spare time."
projects:
  - title: "annotate_models"
    excerpt: "A Ruby gem that adds a schema summary comment to your ActiveRecord models, fixtures, specs, factories and `routes.rb`, so the table layout is always in view.<br><br>`Ruby` · 4.4k+ ★"
    url: https://github.com/ctran/annotate_models
    btn_label: "View on GitHub"
    btn_class: "btn--primary"
  - title: "TinyRadius"
    excerpt: "A small, fast Java library for sending and receiving Radius packets per RFC 2865/2866. Originally written by Matthias Wuttke.<br><br>`Java` · 130+ ★"
    url: https://github.com/ctran/TinyRadius
    btn_label: "View on GitHub"
    btn_class: "btn--primary"
  - title: "nixpkgs-bin"
    excerpt: "Official prebuilt binaries packaged for Nix, pinned with SHA-256 hashes and updated automatically by GitHub Actions. Ships <a href='https://mise.jdx.dev/'>mise</a> today.<br><br>`Nix`"
    url: https://github.com/ctran/nixpkgs-bin
    btn_label: "View on GitHub"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

<h2 id="projects">Featured projects</h2>

{% include feature_row id="projects" %}

## Get in touch

The best way to reach me is through [GitHub](https://github.com/ctran). Bug reports and pull requests on any of the projects above are welcome, especially for [annotate_models](https://github.com/ctran/annotate_models).
