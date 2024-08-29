---
layout: page
title: mc-crawler <i class="fa-solid fa-circle-info fa-xs"></i>
importance: 1
related_publications: true
description: A MobileCoin network crawler.
---

<a href="https://github.com/wiberlin/mc-crawler">
<img align="left" style ="padding: 1em 1em 0 0;" src="https://github-readme-stats.vercel.app/api/pin/?username=wiberlin&repo=mc-crawler&show_owner=true&theme=dracula"/>
</a>

[mc-crawler](https://github.com/wiberlin/mc-crawler) is a crawler for the
[MobileCoin](https://mobilecoin.com/) network built in Rust.
The project begun as a small research project as part of my required coursework
for my Master's but I later continued working on the crawler within the scope of
my part time job at the Weizenbaum Institute.
The overall goal of this project was to learn more about the budding
cryptocurrency on a technical level, i.e., learn about the network size and
structure of the peer-to-peer overlay, which we achieved by first collecting
data using a crawler.

The binary crawls the network and communicates with the validators using RPCs
provided by the MobileCoin API.
The crawler provides 2 JSON files with a crawl report comprising data about
found nodes such as hostnames, public keys and IP-based geolocation data.
We [published a paper](https://arxiv.org/pdf/2111.12364.pdf) with our findings
based on the data collected by the crawler and analyses performed with a related
tool -- the [fbas_analyzer](https://github.com/wiberlin/fbas_analyzer).
The TLDR is that there are a total of 10 validator nodes operated by 7 different
organisations and the MobileCoin quorum system resulting from individual
validators' configurations prioritises safety over liveness.

I also wrote an [API](https://api.crawler.mc.trudi.group/v1) using
[Rocket](https://rocket.rs/) and MongoDB with which the crawl data can be
queried via HTTP; unfortunately the API code is currently not open source.

<b>New Technologies</b>
- MongoDB
- Rocket
- GitHub Actions
- Gitlab CI
