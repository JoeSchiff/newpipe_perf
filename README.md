## Overview

This repo creates a fork of [NewPipe](https://github.com/TeamNewPipe/NewPipe).

[A pull request](https://github.com/TeamNewPipe/NewPipe/pull/11743/commits) was introduced into NewPipe v0.27.3 which slowed the feed loading for YouTube videos. 

This fork reverts those changes.

Currently based on NewPipe v0.27.6

<br>

## Installation

Download the APK file to your phone:\
https://github.com/JoeSchiff/newpipe_perf/releases/download/v0.27.6/NewPipe_v0.27.6_perf.apk

Open the APK file in your phone to install.

<br>

## Differences from NewPipe

I made only 3 changes to the app. 2 changes to this file:\
app/src/main/java/org/schabi/newpipe/local/feed/service/FeedLoadManager.kt

Increased `PARALLEL_EXTRACTIONS` from 3 to 6.\
Increased `BATCH_SIZE` from 50 to an arbitrarily high number.

I also built as `assembledebug` instead of `assemblerelease` (until I can figure out how to sign it).

