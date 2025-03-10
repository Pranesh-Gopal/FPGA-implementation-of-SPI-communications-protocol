The Serial Peripheral Interface (SPI) is a synchronous communication protocol widely used for high-speed
data transfer between devices. It facilitates full-duplex communication using signals such as Chip Select (CS),
Serial Clock (SCLK), and data lines (MOSI/MISO).
This Verilog module implements an SPI master protocol on an FPGA to transmit 16-bit data to an SPI slave
device. It generates the necessary SPI signals (spi_cs_l, spi_sclk, spi_data) and operates using a finite state
machine (FSM). The FSM transitions through states to handle data loading, clock toggling, and bitwise data
transmission, ensuring compliance with SPI timing requirements.
The design includes a 5-bit counter to track transmitted bits and supports asynchronous reset for initialization.
This implementation is suitable for applications such as sensor interfacing, data logging, and communication
with external peripherals like flash memory or DACs.
