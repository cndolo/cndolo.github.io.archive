---
layout: page
title: stellar_analysis <i class="fa-solid fa-circle-info fa-xs"></i>
importance: 2
related_publications: false
description: Interactive analyses of the Stellar public network using fbas_analyzer compiled to WebAssembly.
---

<a href="https://github.com/wiberlin/stellar_analysis">
  <img align="left" style ="padding: 1em 1em 0 0;" src="https://github-readme-stats.vercel.app/api/pin/?username=wiberlin&repo=stellar_analysis&show_owner=true&theme=dracula"/>
</a>

Prior to working on
[stellar_analysis](https://github.com/wiberlin/stellar_analysis"), I
collaborated on the development of an analysis library for networks such as
Stellar -- the [fbas_analyzer](https://github.com/wiberlin/fbas_analyzer), which
is a command line framework written in Rust that performs numerous analyses and
returns metrics about the given network.

We compiled select fragments of the aforementioned framework to WebAssembly in
this project and provide an interactive analysis software.
This allows users to perform the analyses in their browser without knowledge of
the command line or the Rust programming language.
We also maintain an interactive website for
[Stellar](https://trudi.weizenbaum-institut.de/stellar_analysis/) and
[MobileCoin](https://trudi.weizenbaum-institut.de/mobilecoin_analysis/).

[Stellarbeat](https://stellarbeat.io) -- a prominent website showing the status
of the Stellar network - integrated this project into the website enabling users
to perform analyses on [stellarbeat.io](https://stellarbeat.io) directly.

<b>New Technologies</b>
- WebAssembly
- JavaScript
