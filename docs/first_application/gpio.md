---
sidebar_position: 1
---
# 3.1 GPIO Read/Write Operation Example


<iframe width="560" height="315" src="https://www.youtube.com/embed/TiuxZgGBuSM?si=Fu5bWfOOugeD_WL0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

In the `/app/40pin_samples/` directory of the development board, there are various test codes for the functionalities of the 40-pin GPIO, including input/output testing, PWM, I2C, SPI, UART, etc. All the test programs are written in Python. For more detailed information, please refer to the [40PIN User Guide](../python_development/40pin_user_guide/40pin_define.md).

Taking `/app/40pin_samples/button_led.py` as an example, this program configures pin 38 as an input and pin 36 as an output. The output state of pin 36 is controlled based on the input state of pin 38.

## Environment Setup
Connect pin 38 to 3.3V or GND using jumper wires to control its voltage level.

## Running the Program
Execute the `button_led.py` program to start the GPIO read/write operation.

```bash
sunrise@ubuntu:~$ cd /app/40pin_samples/
sunrise@ubuntu:/app/40pin_samples$ sudo python3 ./button_led.py
```

## Expected Result
By controlling the voltage level of pin 38, the output level of pin 36 can be changed.

```bash
sunrise@ubuntu:/app/40pin_samples$ sudo python3 ./button_led.py
Starting demo now! Press CTRL+C to exit
Outputting 0 to Pin 36
Outputting 1 to Pin 36
Outputting 0 to Pin 36
```