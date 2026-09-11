> [!NOTE] Arduino platform
>
> - open-source platform (large community) for a micro-controlller board
> - hardware specification
>   - micro-processor computer (ATmega328P)
>   - A clock (resonator)
>   - A power supply (16Mh)
>   - a usb interface
> - software specification
>   - arduino IDE (code editor for C++ code, compiler, programmer)
>   - arduino library

# Hardware anatomy

![[Attachments/Screenshot 2026-08-28 at 14.46.15.png]]

- USB port: 5V, ~1A
- VIN: 7-12V, ~1A
- digital pins: 5V, ~40mA
- pins 0-1: serial COM
- pin 13: LED pin
- pin (~): PWM (pulse width modulation pins)

# API (application programming interface)

- what functions and objects arduino gives you access to, what their inputs and outputs are
