## GNURadio NoVNC Docker Environments for Multiple Versions
These Docker images provide a fully functioning NoVNC GUI environment for running different versions of GNURadio
Currently I have builds for GNURadio 3.8, 3.9 and 3.10. My hope is to offer a multi-version development solution for porting and cases that require concurrent versions of GNURadio.

### PyBombs Replacement?
As a long-time user of PyBombs, I understand the Pros/Cons of it. The GNURadio core framework has improved immensily since the days of 3.7/3.8, so I have found that keeping active versions of older GNURadio builds serves me less and less. However, there are occasions where I'd like to investigate a block that is only available for an older verison of GNURadio (for example GNURadio 3.8), which is where I use these containers. After I see they can work, I have the choice to either port the block, or create a slimmer container for the blocks from an older version and use ZMQ sockets for the inbound/outbound streams (more on that in another project).

#### CREDITS
All credit really goes to [@tdsepsilon](https://twitter.com/tdsepsilon) for his post [here](https://teaandtechtime.com/simple-gnuradio-server-setup-with-novnc-docker/)
I just changed the dependencies and repos to match various versions.
