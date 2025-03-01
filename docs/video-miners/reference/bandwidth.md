---
title: Bandwidth Requirements
sidebar_position: 3
---

# Bandwidth Requirements

The bandwidth requirements for video miners are based on the amount of video
data that needs to be uploaded and downloaded during transcoding.

The amount of available bandwidth will not only impact the number of streams
that can be transcoded on a machine, but also the speed of data upload/download
which needs to be fast so that video streaming applications can receive
transcoded results as soon as possible.

The amount of bandwidth required for a stream will depend on the bitrate of the
source stream and the bitrate of the output renditions. The download bandwidth
required for a single stream can be roughly estimated as the bitrate of the
source stream. The upload bandwidth required for a single stream can be roughly
estimated as the sum of the bitrates of each of the output renditions for the
stream. As a result, the total number of streams that can be transcoded given a
certain amount of available of bandwidth will vary.

While there is not a strict bandwidth requirement for video miners, past testing
has demonstrated that 1G upload/download bandwidth is a good starting point if
possible. If you do not have access to this amount of bandwidth you will still
be able to transcode on the network, but you will have a lower ceiling on the
number of streams you will be able to handle.

Upload/download bandwidth available can be tested with tools such as:

- [speedtest](https://www.speedtest.net/apps/cli)
  - By default the tool will run a bandwidth test against the closest public
    server, but there is also an option to run the test against a specified
    public server
  - Note: The results of this test also depend on the available bandwidth on the
    server used
- [iperf3](https://iperf.fr/)
  - This tool can be run on client and server machines that you have access to
  - If you have access to a machine with good bandwidth availability in a region
    that you expect/want to receive streams from, then this tool will likely be
    more useful than speedtest

