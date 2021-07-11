# iceoryx_demos

---
## Introduction

[iceoryx](https://github.com/eclipse-iceoryx/iceoryx) is an inter-process-communication (IPC) middleware for various operating systems (currently we support Linux, MacOS and QNX).

This is a project for demos. I'll implement simple message transmission to heavy data transmission by using iceoryx to test its performance and robustness.

---
## Content

TBD

---
## Build and test

[`vcstool`](https://github.com/dirk-thomas/vcstool) and [`colcon`](http://colcon.readthedocs.io/) would make building convieniently but not necessary. With `vcstools`, you will be able to manage all projects you are using easier than `git submodule`. With `colcon`, the compilation and dependencies of projects would be clearly and simply.

If you didn't install `iceoryx` in your system. Download with 

```
mkdir -p demos_ws/src
cd demos_ws/src
git clone https://github.com/homalozoa/iceoryx_demos.git
vcs import . < iceoryx_demos/depends.repos
cd ..
```

and build with 

```
colcon build --merge-install
```

All projects under `./src` would be compiled at once.

