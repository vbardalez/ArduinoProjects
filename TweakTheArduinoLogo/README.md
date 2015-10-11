	//Arduino Code
	void setup() {
	Serial.begin(9600);
	}
	
	void loop() {
	Serial.write(analogRead(A0)/4);
	
	delay(1);
	}
	
	// Processing Code
	/*import processing.serial.*;
	Serial myPort;
	PImage logo;
	int bgcolor = 0;
	void setup(){
	colorMode(HSB, 255);
	logo = loadImage("http://arduino.cc/logo.png");
	size(logo.width, logo.height);
	println("Avaliable serial ports:");
	println(Serial.list());
	myPort = new Serial(this, Serial.list()[0], 9600);
	}
	void draw(){
	if (myPort.available() > 0) {
		bgcolor = myPort.read();
		println(bgcolor);
	}
	background(bgcolor, 255, 255);
	image(logo, 0, 0);
	}*/
