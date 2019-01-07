# Subutai Blueprint for Elasticsearch Server

There's a few ways to cook up ES:

  1. Using the default package configuration
  2. Using the bare bones configuration in this BP

If you're installing a large enterprise configuration then you can go with
the first method. This approach causes some issues in Subutai, that can be
dealt with but why deal with the pain: namely around file descriptor
limits and max memory mapping pages. Sometimes you just need a simple
installation that just works well in a smaller container footprint, and that's
exactly what this BP does.

If you want to go back into history to see the first attempt that used approach
\#1 then please look at the following [commit version](https://github.com/akarasulu/elasticsearch-bp/tree/d9994f2c4c6dceb93e406997df18e3c0ac8ccc22).
It used the official repository and packages to setup the environment however
had issues concerning resources.
