- required Arduino function definitions

```C++
void setup() {
	// do at start, runs it once
}
void loop() {
	// repeat forever
}
```

[[arduino constants]]

```
void setup() {
	pinMode(13, OUTPUT);
}

void loop() {
	digitalWrite(13, HIGH);
	delay(1000);
	digitalWrite(13, LOW);
	delay(1000);
}
```
