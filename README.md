# ompl-debian

This repository includes debian files for custom OMPL packages for Personal Robotics Lab.

We need the custom OMPL packages on Ubuntu 14.04 and Ubuntu 16.04 for the following reasons.

**Ubuntu 14.04**

AIKIDO requires OMPL (>= 1.2.1) by [aikido #446](https://github.com/personalrobotics/aikido/pull/466), but the available OMPL packages on Ubuntu 14.04 (i.e., `libompl-dev`: 0.13.0, `ros-indigo-ompl`: 1.0.0) are too old.

**Ubuntu 16.04**

The system version of OMPL packages `libompl-dev` (v1.0.0) is too old for AIKIDO, and `ros-kinetic-ompl` (v1.2.1) has a runtime-error issue (see [aikido #363](https://github.com/personalrobotics/aikido/issues/363) for detail).

To address above issues, [PRL PPA](https://launchpad.net/~personalrobotics/+archive/ubuntu/ppa) provides `libompl-dev` (v1.2.1) that includes the fix for [aikido #363](https://github.com/personalrobotics/aikido/issues/363) for Ubuntu 14.04 and 16.04. This repository contains the debian files for the packages. The PPA source packages recipes are here:
  * [Ubuntu 14.04](https://code.launchpad.net/~personalrobotics/+recipe/prl-ompl-daily-trusty)
  * [Ubuntu 16.04](https://code.launchpad.net/~personalrobotics/+recipe/prl-ompl-daily-xenial)
