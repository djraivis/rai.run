---
description: Test to reinstal M1
slug: reinstalM1
public: true
layout: ../../layouts/BlogPost.astro
title: re-instal M1
createdAt: 1724145803666
updatedAt: 1724147589814
tags: []
heroImage: /posts/reinstalM1_thumbnail.jpg
---

Work with vidoe:
- `brew install ffmpeg`
  - `ffmpeg -i input.mp4 -c:v copy -c:a copy output.m4v`
  - `ffmpeg -i input.m4v -b:v 1000k -c:v h264 -c:a aac -strict -2 output_compressed.m4v` 
  - `ffmpeg -i input.m4v -c:v libvpx -b:v 1M -c:a libvorbis output.webm`
  - `ffmpeg -i input.m4v -c:v libvpx -b:v 500k -c:a libvorbis -b:a 64k output_compressed.webm`

