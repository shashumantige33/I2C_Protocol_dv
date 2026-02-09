# I2C_Protocol-dv
I2C is a synchronous, serial, multi-master, multi-slave communication protocol. It uses only two wires to communicate between devices:
  SCL (Serial Clock Line) – Carries the clock signal
  SDA (Serial Data Line) – Carries the data
I2C is widely used for short-distance communication between microcontrollers and peripherals such as sensors, EEPROMs, RTCs, and displays.

1. Start Condition

Communication begins when the master pulls SDA low while SCL is high.

2. Slave Address + R/W Bit

7-bit or 10-bit slave address

1-bit R/W flag (0 = Write, 1 = Read)

3. Acknowledge (ACK/NACK)

Receiver pulls SDA low to send ACK

Leaves SDA high to send NACK

4. Data Transfer

Data is transferred in 8-bit bytes

Each byte is followed by ACK/NACK

5. Stop Condition

Communication ends when SDA goes high while SCL is high.
