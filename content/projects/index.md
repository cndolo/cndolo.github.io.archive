+++
title = "Computer Scientist"
date = 2022-02-05
+++

<a href="https://github.com/cndolo">
  <img style="float: left"  style ="padding: 0 1em 0 0;" src="https://github-readme-stats.vercel.app/api/top-langs/?username=cndolo&layout=compact&theme=dracula"/>
</a>
<a href="https://github.com/cndolo">
  <img style="float: right" src="https://github-readme-stats.vercel.app/api/?username=cndolo&show_icons=true&theme=dracula"/>
</a>
This is a brief showcase of some of the projects I have worked on recently.

I only mention open-source projects available on GitHub - unfortunately none of the `Go` projects I have collaborated on is publicly available.
The badges below are clickable links to the projects' respective repositories.

<a href="https://github.com/wiberlin/mc-crawler">
  <img align="left" style ="padding: 1em 1em 0 0;" src="https://github-readme-stats.vercel.app/api/pin/?username=wiberlin&repo=mc-crawler&show_owner=true&theme=dracula"/>
</a>

[mc-crawler](https://github.com/wiberlin/mc-crawler) is a crawler for the [MobileCoin](https://mobilecoin.com/) network built in Rust.
The project begun as a small research project as part of my required coursework for my Master's but I later continued working on the crawler within the scope of my part time job at the Weizenbaum Institute.
The overall goal of this project was to learn about the budding cryptocurrency, i.e. learn about the network size and structure of the peer-to-peer overlay, which we achieved by first collecting data using a crawler.

The binary crawls the network and communicates with the validators using RPCs provided by the MobileCoin API.
The crawler provides 2 JSON files with a crawl report comprising data about found nodes such as hostnames, public keys and IP-based geolocation data.
We [published a paper](https://arxiv.org/pdf/2111.12364.pdf) with our findings based on the data collected by the crawler and analyses performed with a related tool - the [fbas_analyzer](https://github.com/wiberlin/fbas_analyzer).
The TLDR is that there are a total of 10 validator nodes operated by 7 different organisations and the MobileCoin quorum system resulting from individual validators' configurations prioritises safety over liveness.

I also wrote an [API](https://api.crawler.mc.trudi.group/v1) using [Rocket](https://rocket.rs/) and MongoDB with which the crawl data can be queried via HTTP; unfortunately the API code is currently not open-source.

**New Technologies: MongoDB, Rocket, GitHub Actions, Gitlab CI**

<a href="https://github.com/wiberlin/stellar_analysis/commits?author=cndolo">
  <img align="left" style ="padding: 1em 1em 0 0;" src="https://github-readme-stats.vercel.app/api/pin/?username=wiberlin&repo=stellar_analysis&show_owner=true&theme=dracula"/>
</a>

Prior to working on [stellar_analysis](https://github.com/wiberlin/stellar_analysis"), I collaborated on the development of an analysis library for networks such as Stellar - the [fbas_analyzer](https://github.com/wiberlin/fbas_analyzer).
It is a command line framework written in Rust that performs numerous analyses and returns metric about the given network.

We compiled select fragments of the aforementioned framework to WebAssembly in this project and provide an interactive analysis software.
This allows users to perform the analyses in their browser without knowledge of the command line or the Rust ecosystem.
We also maintain a website for [Stellar](https://trudi.weizenbaum-institut.de/stellar_analysis/) and [MobileCoin](https://trudi.weizenbaum-institut.de/mobilecoin_analysis/).

[Stellarbeat](https://stellarbeat.io) - a prominent website showing the status of the Stellar network - integrated this project into the website enabling users to perform analyses on [stellarbeat.io](https://stellarbeat.io) directly.

**New Technologies: WebAssembly, JavaScript**

<a href="https://github.com/networkit/networkit/commits?author=cndolo">
  <img align="left" style ="padding: 1em 1em 0 0;" src="https://github-readme-stats.vercel.app/api/pin/?username=networkit&repo=networkit&show_owner=true&theme=dracula"/>
</a>

[NetworKit](https://github.com/networkit/networkit) is an open-source tool suite for high-performance network analysis with multiple regular contributors.
It is developed in C++ for high performance, but is exposed as a Python module to users.

The algorithms implemented in C++ are exposed to Python via [Cython](https://cython.org/) - a superset of Python providing bindings between C-like languages and Python.
I generally refactored a lot of code while I contributed to this project, e.g. I was significantly involved in modularisation of the Cython interface from one giant file to several modules.

**New Technologies: Cython, project-wide Git, Jupyter Notebook**
