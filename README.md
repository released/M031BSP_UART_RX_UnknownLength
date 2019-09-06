# M031BSP_UART_RX_UnknownLength

update @ 2019/09/06

Use UART RX to receive unknown length

- At UART02_IRQHandler , take (N-1) byte in UART RX buffer (UART FIFO : N byte) , 

and at last transmit , will trigger RX timeout , then calculate this RX packet total length

