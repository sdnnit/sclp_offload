## SCLP offload module


### Overview

SCLP (Segment-oriented Connection-less Protocol) is a novel L4 protocol 
for accelerating performance of existing tunneling protocols, such as 
VXLAN and NVGRE. The SCLP protocol is designed to take advantage of 
a GSO (Generic Segmentation Offload) and a GRO (Generic Receive Offload) 
features of the Linux kernel, and this module contains full-implementation 
of both features for SCLP.


=
### Contents

* sclp.h          : SCLP header definition

* sclp_offload.c  : GSO/GRO implementation for SCLP


=
### Supported distributions

Currently, the SCLP offload module has been tested on the following distributions.

 * Redhat Enterprise Linux 6.5, 6.6


=
### Install

### 1. Getting the source code of the SCLP offload module

You can download the code from the GitHub repository.

    https://github.com/sdnnit/sclp_offload


### 2. Bulding the SCLP offload module

To build the module, you can simply use the make system

```sh
$ make
```

If the building process succeeds, 'sclp_offload.ko' file is created in the current directory.


### 3. Installing the SCLP offload module

```sh
# insmod sclp_offload.ko
```

=
### Papers

Overview of the SCLP protocol and the offload module are described in the following 
paper.

* R. Kawashima, S. Muramatsu, H. Nakayama, T. Hayashi, and H. Matsuo, 
"SCLP: Segment-oriented Connection-less Protocol for High-Performance 
Software Tunneling in Datacenter Networks", Proc. 1st IEEE Conference on 
Network Softwarization (NetSoft 2015), London, UK, April 2015 (to appear).


=
### Contact 

Ryota Kawashima &lt;kawa1983<span>@</span>ieee.org&gt;

