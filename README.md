## Overview

This is a fork of https://github.com/TeamNewPipe/NewPipe

[A pull request](https://github.com/TeamNewPipe/NewPipe/pull/11743/commits) was introduced into v0.27.3 which slowed the feed loading. 

This fork reverts those changes. 


## Installation

Download the APK file to your phone:
https://github.com/JoeSchiff/newpipe_perf/latest

Open the APK file in your phone to install.

## Differences from NewPipe

I make only 2 changes to the app. Both changes are to this file:
app/src/main/java/org/schabi/newpipe/local/feed/service/FeedLoadManager.kt

Increased `PARALLEL_EXTRACTIONS` from 3 to 6.
And set `BATCH_SIZE` to an arbitrarily high number.



