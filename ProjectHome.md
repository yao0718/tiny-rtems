Descripton:

RTEMS is a real-time embedded operating system. Currently a minimum RTEMS application will automatically include part of reentrant C library, shutdown code and filesystem infrastructure. These codes are hard to remove because they are tightly coupled with other kernel components. This project would focus on breaking linkages between components so they can be configured by the user. The goal is to be able to provide the user with a full featured RTEMS library and defer as much configuration as possible to application configuration and link time.

In this project I will introduce several changes to RTEMS source code and its build system to make it more 'tiny', configurable and scalable. These include: an alternative lightweight standard POSIX file I/O interface ; more configuration options and simplified configuration steps; modifications to the source code to take more features out at the user's discretion. And finally I will give a well-written User's Manual and a Design & Implementation description in detail.

The original proposal is available here:

http://www.rtems.org/wiki/index.php/TinyRTEMS

http://www.rtems.org/wiki/index.php/Open_Projects

Profit for RTEMS:

1. RTEMS can run on many deeply embedded, resources constrained systems, like 8bit or 16 bit CPUs in industry control area, low memory environments such as SoC ARM implementations with only 16KB ROM and 4KB RAM, and safety critical applications which need to eliminate all the unused code and data

2. RTEMS would be more configurable and scalable. As many features are taken out as an optional, users can take better control of their programs, thus increasing the efficiency and reliability