<h1> FreeRTOS On RZN2L With Debugging </h1>

## 1. Introduce
![image](https://github.com/khoatm98/RZN2L-freeRTOS/assets/64945894/79b24636-2a78-45b0-8a95-067b73898987)


- FreeRTOS is a real-time operating system kernel for embedded devices that has been ported to 35 microcontroller platforms
- FreeRTOS is designed to be small and simple. To make the code readable, easy to port, and maintainable, it is written mostly in C, but there are a few assembly functions included where needed (mostly in architecture-specific scheduler routines).
- FreeRTOS provides methods for multiple threads. A tick-less mode is provided for low power applications.
- FreeRTOS kernel features:
  + Pre-emptive or co-operative operation
  + Very flexible task priority assignment
  + Software timers
  + Queues
  + Binarysemaphores
  + Countingsemaphores
  + Recursivesemaphores
  + Mutexes
  + Tick hook functions
  + Idle hook functions
  + Stack overflow checking
  + Trace hook macros
 

## 2. FreeRTOS Structure & Hierarchy
- Download sources:
```shell
 https://sourceforge.net/projects/freertos/files/FreeRTOS/
```
```
FreeRTOS
  ├── Demo             (Contains demo application for every official FreeRTOS port)
  ├── Test             (contains the tests performed on common code and the portable layer code)
  └── Source           (Core FreeRTOS kernel file)
      ├── include      (Consists of The core FreeRTOS kernel header files)
      └── portable     (Consists of Processor specific code)
          ├── Compiler (Contains all the ports created by compiler)
          ├── MemMang  (Contains The sample heap implementations)
          └── ...
```

- Structure & Hierarchy:
```
FreeRTOS.h
   ├── FreeRTOSConfig.h        (Application specific configuration options)
   ├── projdefs.h              (Basic FreeRTOS definitions)
   └── portable.h              (Definitions specific to the port being used)
         ├── portmacro.h
         └── mpu_wrappers.h

FreeRTOS.h
   ├── list.c
   ├── croutine.c
   ├── timers.c
   ├── heap_?.c
   ├── queue.c
   └── tasks.c
```

## 3. Goal
- Understanding various RTOS concepts with FreeRTOS Programming and Debugging
- Using RZN2L Standard Peripheral Driver APIs to configure peripherals
- FreeRTOS Debugging using E2 Studio
- Using FreeRTOS API with code examples
- ...

## 4. Prepare

| Software              | Hardware               |       
|-----------------------|------------------------|

 
