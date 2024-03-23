## FasterLIO-PPF

This is the code repo of integrating PPF (Plane Pre-Fitting and Skeleton Tracking) into [FasterLIO](https://github.com/gaoxiang12/faster-lio).


The PPF is introduced by our paper "[LIO-PPF: Fast LiDAR-Inertial Odometry via Incremental Plane Pre-Fitting and Skeleton Tracking](https://ieeexplore.ieee.org/abstract/document/10341524/)"  (**IROS 2023**).

### Quick Start

```bash
catkin_make
source devel/setup.bash
roslaunch faster_lio mapping_velodyne.launch
```

In another terminal:
```bash
rosbag play /path/to/your/bag/file
```

For details about building and running, please refer to [FasterLIO](https://github.com/gaoxiang12/faster-lio).


### LIO-SAM with PPF
If you are looking for LIO-SAM with PPF, please check out [LIO-PPF](https://github.com/xingyuuchen/LIO-PPF).


### Citation

If you find our work useful or interesting, please consider citing our paper:
```latex
@inproceedings{chen2023lio,
  title={LIO-PPF: Fast LiDAR-Inertial Odometry via Incremental Plane Pre-Fitting and Skeleton Tracking},
  author={Chen, Xingyu and
        Wu, Peixi and
        Li, Ge and
        Li, Thomas H},
  booktitle={2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  pages={1458--1465},
  year={2023},
  organization={IEEE}
}
```



