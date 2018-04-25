---
layout: post
title:  "Docker Drops #1 - Docker logs a bit more expressive"
date:   2018-04-25 00:00:31 -0300
categories: en docker drops
---

**Docker Drops** is something that I just invented right now...

The idea is to show you a **simple**... a **very very simple**... **extremely simple**: command, concept, tool, or idea that could be useful for you.


## Docker logs (wait for it):

Yesterday we found a problem in one of our production site, and while troubleshooting we suspected that specific one container didn't ran as expected.
So we said: Let's go get the logs!

To get the logs of a Docker container is a no brainer command: `docker logs <CONTAINER ID>`. Simple right?!
But when the logs are too long we need to cut it off to pick the important parts.

The first thought was to `tail` or `grep` part of the output, but after a few synapses I decided to inspect the information returned by `docker logs --help` :)

**Suddenly some wild arguments appears**

- `docker logs -t` or `docker logs --timestamps` will print out the timestamp at the beginning of each line of the log. *Good to grep*!

- `docker logs --detail` will show you extra information

- `docker --since <STRING>` will filter and show you the logs since the date you put in <STRING>. It could be absolute, like: ` 2013-01-02T13:23:37` or relative: 42m for 42 minutes)


That's it!

Hope that helps!
