- protocol for co,puters to talk to each other
- uses two one-way wires TX -> RX, RX -> TX, one trasnmits, one received
- sends data serially, byte-by-byte
- baudrate (bits per second) for Arduino 9600 or 115200

```C++
void Serial.begin(baudrate);
void Serial.print(string);
void Serial.println(string);
```

# Example usage

![[Attachments/Screenshot 2026-08-28 at 15.30.44.png]]
