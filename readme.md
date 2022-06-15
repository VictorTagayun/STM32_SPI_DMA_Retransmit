# STM32 SPI DMA Retransmit

Control SPI Circular DMA retrasmission of data/packet using an external interrupt pin. 

## Purpose
When the DMA is in circular mode, there is no control on when to resend the SPI packed even is the data is not yet available. The SPI bus (with circular DMA) will keep sending the data.  

Being able to control when to send the SPI data/packet in DMA is a big advantage on the processing of data in a timely manner.  

## Steps / Procedure

1. One pin for an external interrupt
2. In SPI, enable DMA and external syncronization

## Project files

1. NUCLEO-G474RE_LL-SPI_DMA - normal SPI DMA setting
2. NUCLEO-G474RE_LL-SPI-EXT-TRIG-CIRC-DMA - SPI Circular DMA with external interrupt for syncronization 

