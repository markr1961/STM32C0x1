## STM32C0x1 projects
Multiple projects based on the new STM32C0 family and its demo boards.
Existing projects use STM's CubeIDE. At some future point things may be changed to IAR WARM v9.40.2. (v9.2 is the minimum version required to support the C0 family.)

2025-08-08  
add the base projects, their sources and libraries and CubeMX/CubeIDE definition files. There is a lot of detritus that should be cleaned out.
add CubeIDE workspace and project files. Some of these may need to be trimmed later.

#### blinky

#### DK32C011
doesn't build due to missing definition of COM_NBR and missing prototype for MX_USART2_Init()
There maybe other issues with trying to build the C31 discovery project on a C11.

#### nucleo_c31_adc_dma

#### WS2812B-pwm-dma
a WS2812B driver project. 
Adapted from https://controllerstech.com/interface-ws2812-with-stm32/
uses CubeMx to drive a timer with DMA. modified for STM32C0.
The CubeMx project appears like it was hacked up. It complains about an invalid MCU type (STM32C031C6Tx).

