---
layout: post
title: Satellites and Stuff
---

Currently some of my my work surrounds making ESA Sentinel 2 data available for parts of the UK, well that may seem like a nice easy task but the fun just doesn’t stop with heres a massive zip file have fun. 

First off we the raw data needs to be processed so that it is useable in the first place, this process is something we call the Analysis Ready Data format (for Sentinel 1 and 2). Both sections are based on a number of different bits tied together with as much string as you can feasibly produce.

At their core we have a Docker container which is our workhorse, giving us a repeatable, versioned process, these can be found in the JNCC github. [Sentinel 1](https://github.com/jncc/s1-ard-processor) is based aroudn the ESA SNAP toolbox and [Sentinel 2](https://github.com/jncc/s2-ard-processor) based around the ARCSI toolbox developed by Pete Bunting at Aberystwyth University. These nuggets of processing are wrapped up with a layer of orchestration written in [Luigi](https://github.com/spotify/luigi) to do the magic around the black boxes inside.

Another side project that comes out of this is a general arty thing I do with the imagery, it makes good and unique gifts for all. I will probably continue posting more of these when I make them;

!/images/2020-01-25-Satellites-and-Stuff/uk.png]({{ site.baseurl }}/images/2020-01-25-Satellites-and-Stuff/uk_thumbnail.png)