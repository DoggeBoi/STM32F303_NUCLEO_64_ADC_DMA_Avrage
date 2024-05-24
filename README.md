# STM32F303_NUCLEO_64_ADC_DMA_Avrage
Proof of concept test project for HAL-based DMA ADC voltage sensing with a STM32F303 NUCLEO-64 board and a simple voltage splitter. 
0-15.5v (18.5v absolute max). Voltage measured around R2, R1 = 9949Ω, R2 = 2003Ω. Output printed to the serial monitor over UART at  33Hz.
Output calibrated with a lab bench power supply at 12v. Conversion factor 0,005 for 12-bit output. Running point average with 1024 values captured from the last ~240us.
Very stable at two decimals (voltage, after raw data conversion). Will be used between 6-15v, ~0.1v drift at the limits, acceptable.
