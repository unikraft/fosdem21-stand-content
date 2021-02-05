---
description: |
  Unikraft is a Linux Foundation project able to build extremely efficient and
  secure software stacks/unikernels. By tailoring the operating system,
  libraries and tools to the particular needs of each application, it vastly
  reduces virtual machine and container image sizes to a few KBs drastically
  cutting down the software stack's attack surface. Our evaluation using
  off-the-shelf popular applications such as Nginx, SQLite, and Redis shows that
  running such applications on Unikraft results in a 30%-50% performance
  improvement compared to Linux guests. In addition, Unikraft images for these
  apps are around 1MB, require less than 10MB of RAM to run, and boot in around
  1ms on top of the VMM time (total boot time 2ms-70ms).
  
layout: stand
show_on_overview: true
logo: stands/unikraft/logo.svg
new_this_year: |
  <p>
  In early 2021 we will be releasing the v0.5.0 (Tethys), which will be our
  biggest release yet.  Since our last presentation at FOSDEM2020, in addition
  to growing the community, we have added a large amount of features to
  Unikraft:
  </p>
  <ul>
    <li>
      Security features, including stack protection, ASAN, Intel MPK, etc.
    </li>
    <li>
      Increasing POSIX support (140+ syscalls and counting), including support
      for standard applications (e.g., nginx, SQLite, Redis, etc.)
    </li>
    <li>
      Native support for many programming languages and language environments:
      C++, Python/Micropython, Go, Lua, Web Assembly (WAMR), JavaScript
      (Duktape), Ruby and Rust (ongoing).
    </li>
    <li>
      Network performance optimizations for KVM
    </li>
    <li>
      Support for networking and performance optimizations for Xen
    </li>
    <li>
      ARM64 bare metal support for the Raspberry Pi 3 and the Xilinx Ultra96-v2
      boards.
    </li>
    <li>
      Page table support.
    </li>
    <li>
      Initial support for Amazon Firecracker
    </li>
    <li>
      Cloud-based deployments (GCP, AWS, Digital Ocean).
    </li>
    <li>
      Improvements to the ARM64 platform, including virtio and multi-thread
      support
    </li>
    <li>
      Basic musl support And lots of other features and bug fixes. 
    </li>
  </ul>
  <p>
  Finally, we are hard at work integrating Unikraft into standard frameworks
  such as Kubernetes and Cloud Foundry.
  </p>
showcase: |
  <img src="https://camo.githubusercontent.com/7e8177294667930f661d874b396e28ff71869dfcc9891a2c702d5b8b93503f5d/687474703a2f2f756e696b726166742e6f72672f6173736574732f696d67732f686f772d756e696b726166742d776f726b732e737667" width="25%" style="float:right;" />
  <p>
  Unikraft is an automated system for building specialized POSIX-compliant OSes
  known as unikernels; these images are tailored to the needs of specific
  applications. Unikraft is based around the concept of small, modular
  libraries, each providing a part of the functionality commonly found in an
  operating system (e.g., memory allocation, scheduling, filesystem support,
  network stack, etc.).
  </p>
  <p>
  Unikraft supports multiple target platforms (e.g., Xen, KVM, and Linux 
  serspace) so that it is possible to build multiple images, one for each
  platform, for a single application without requiring the application developer
  to do any additional, platform-specific work. In all, Unikraft is able to
  build specialized OSes and unikernels targeted at specific applications
  without requiring the time-consuming, expert work that is required today to
  build such images.
  </p>
  <p>
  If you run significant amount of services on public cloud infrastructure, you
  should come to our stand to find out how Unikraft can help you seamlessly
  debloat your deployments; for example, in recent experiments on AWS we have
  been able to cut costs by half when running NGINX compared to a Linux image.
  If you come from the automotive industry, Unikraft can act as a minimal guest
  that can provide POSIX-like functionality while providing a relatively cheap
  certification path. And if you work on IoT or edge cloud deployments, Unikraft
  can even run bare metal on ARM devices, providing substantial efficiency on
  such hardware-constrained devices. 
  </p>
  <h3>Linux Foundation and Xen Incubator Project</h3>
  <div style="padding:1em;background-color:#444;text-align:center;">
    <img src="http://unikraft.org/assets/imgs/xen-project.svg" style="width:45%" />
    <img src="http://unikraft.org/assets/imgs/linux-foundation.svg" style="width:45%" />
  </div>
  <br />
  <h3>Find us on Online</h3>
  <ul>
    <li><a href="http://unikraft.org">Website</a></li>
    <li><a href="https://github.com/unikraft/unikraft">Github</a></li>
    <li><a href="https://wiki.xenproject.org/wiki/Category:Unikraft">On Xen Project</a></li>
    <li><a href="https://xenproject.org/developers/teams/unikraft/">About the Xen Project Team</a></li>
  </ul>
themes:
- Operating Systems
title: Unikraft
website: http://unikraft.org
chatroom: unikraft
---
