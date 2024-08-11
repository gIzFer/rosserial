# rosserial

## Changes I've done:
 - 'fixed' error `marked 'override', but does not override` in `service_client.h: virtual void call()`
 - reduced ram usage for rosserial_arduino by using `PROGMEM` on strings

## How I built it:

```
cd rosserial_client
cmake .
make
source devel/setup.sh

cd ../rosserial_arduino
cmake .
make
source devel/setup.sh
rosrun rosserial_arduino make_libraries.py PATH_TO_WHERE_TO_BUILD_LIBRARY
```

(instructions from memory; might have to do `make install` too)

---

[![Build Status](https://travis-ci.org/ros-drivers/rosserial.svg?branch=melodic-devel)](https://travis-ci.org/ros-drivers/rosserial)

Please see [rosserial on the ROS wiki](http://wiki.ros.org/rosserial) to get started.
