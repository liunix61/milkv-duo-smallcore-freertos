# milkv-duo-smallcore-freertos

This package is obtained from https://github.com/milkv-duo/duo-buildroot-sdk, from which we download the `FreeRTOS` ported to Milk-V Duo into the Buildroot. This `FreeRTOS` will run in the small core and will not do anything because it is simply a template with some basic UART demos. You can realize your own ideas by adding code to

```
output/build/milkv-duo-smallcore-freertos-hash/cvitek/task/comm/src/riscv64/comm_main.c
```

If you say Y, then every time you make Buildroot, it will automatically compile and include the `FreeRTOS` into the `fip.bin`, which will then be packed into `sdcard.img`

https://github.com/gtxzsxxk/milkv-duo-smallcore-freertos
