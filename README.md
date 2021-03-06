# OpenVSLAM: A Versatile Visual SLAM Framework
[![Documentation Status](https://readthedocs.org/projects/openvslam/badge/?version=master)](https://openvslam.readthedocs.io/en/master/?badge=master)

## Overview

<img src="./docs/img/teaser.png" width="640px">

<img src="https://raw.githubusercontent.com/wiki/xdspacelab/openvslam/media/tracking.gif" width="640px">

OpenVSLAM is a monocular, stereo, and RGBD visual SLAM system.
The notable features are:

- It is compatible with **multiple camera models** and can be easily customized for other camera models.
- Created maps can be **stored and loaded**, then OpenVSLAM can **localize new images** based on the prebuilt maps.
- The system is fully modular. It is designed by encapsulating several functions in separated components with easy-to-understand APIs.
- We provided **some code snippets** to understand the core functionalities of this system.

One of the noteworthy features of OpenVSLAM is that the system can deal with images captured with multiple camera models, such as perspective, fisheye, and equirectangular.
If needed, users can implement extra camera models (e.g. dual fisheye, catadioptric) with ease.
For example, visual SLAM algorithm using **equirectangular camera models** (e.g. RICOH THETA series, insta360 series, etc) is shown above.

Some code snippets to understand the core functionalities of the system are provided.
You can employ these snippets for in your own programs.
Please see the `*.cc` files in `./example` directory or check [Simple Tutorial](https://openvslam.readthedocs.io/en/master/simple_tutorial.html) and [Example](https://openvslam.readthedocs.io/en/master/example.html).

We provided [documentation](https://openvslam.readthedocs.io/) for installation and tutorial.
Please contact us via [GitHub issues](https://github.com/xdspacelab/openvslam/issues) if you have any questions or notice any bugs about the software.

## Installation

Please see [**Installation**](https://openvslam.readthedocs.io/en/master/installation.html) chapter in the [documentation](https://openvslam.readthedocs.io/).

[**The instructions for Docker users**](https://openvslam.readthedocs.io/en/master/docker.html) are also provided.

## Tutorial

Please see [**Simple Tutorial**](https://openvslam.readthedocs.io/en/master/simple_tutorial.html) chapter in the [documentation](https://openvslam.readthedocs.io/).

A sample ORB vocabulary file can be downloaded from [here](https://drive.google.com/open?id=1wUPb328th8bUqhOk-i8xllt5mgRW4n84).
Sample datasets are also provided at [here](https://drive.google.com/open?id=1A_gq8LYuENePhNHsuscLZQPhbJJwzAq4).

If you would like to run visual SLAM with standard benchmarking datasets (e.g. KITTI Odometry dataset), please see [**SLAM with standard datasets**](https://openvslam.readthedocs.io/en/master/example.html#slam-with-standard-datasets) section in the [document](https://openvslam.readthedocs.io/).

## Community

If you want to join our Slack community, please fill out the application form from the following site(s):

- [http://bit.ly/openvslam](http://bit.ly/openvslam)
- [http://bit.ly/openvslam-jp](http://bit.ly/openvslam-jp) (日本語: in Japanese)

## Currently working on

- ROS support
- IMU integration
- Python bindings
- Implementation of extra camera models
- Refactoring

Feedbacks, feature requests, and contribution are welcome!

## License

**2-clause BSD license** (see [LICENSE](./LICENSE))

The following files are derived from third-party libraries.

- `./3rd/json` : part of [nlohmann/json \[v3.6.1\]](https://github.com/nlohmann/json) (MIT license)
- `./3rd/popl` : part of [badaix/popl \[v1.2.0\]](https://github.com/badaix/popl) (MIT license)
- `./3rd/spdlog` : part of [gabime/spdlog \[v1.3.1\]](https://github.com/gabime/spdlog) (MIT license)
- `./src/openvslam/solver/pnp_solver.cc` : part of [laurentkneip/opengv](https://github.com/laurentkneip/opengv) (3-clause BSD license)
- `./src/openvslam/feature/orb_point_pairs.h` : part of [opencv/opencv](https://github.com/opencv/opencv) (3-clause BSD License)

## Contributors

- Shinya Sumikura ([@shinsumicco](https://github.com/shinsumicco))
- Mikiya Shibuya ([@MikiyaShibuya](https://github.com/MikiyaShibuya))
- Ken Sakurada ([@kensakurada](https://github.com/kensakurada))
