##1. Initial Setup
	Upload the Code:
	Open the Arduino IDE on your computer.

	Go to File > Open and navigate to the location where you downloaded the Chhavi repository.

	Open the Example_Websocket.ino file located in the Firmware -> Arduino -> Example_Websocket folder.

	In the Arduino IDE, make sure you have selected the correct board. Go to Tools > Board and choose the ESP32 WROOM module.

	Update the WiFi credentials to match your network. Look for the following lines (around line 14) and replace SSID with your WiFi SSID and PWD with your WiFi password:

	const char* ssid = "SSID";
	const char* password = "PWD";

	Click the Upload button to compile and upload the sketch to your Chhavi device.

##2. Connecting to the Device
	Power On the Device:

	Make sure your Chhavi device is connected to a power source.
	Connect to WiFi:

	Once the device is powered on, it will automatically connect to the WiFi network you specified during setup.
	Access the Web Interface:

	Open a web browser on any device connected to the same WiFi network.
	Enter the IP address of the Chhavi device in the address bar. You can find the IP address from the Arduino IDE's serial monitor after uploading the code.

##3. Using the Web Interface
	The Chhavi web interface allows you to interact with the device using a simple interface in your web browser. Here's how to use the available options:

	Enroll Finger:

	Press 'a' to enroll a new fingerprint.
	Capture and Identify Finger:

	Press 'b' to capture a fingerprint and identify it against the enrolled templates.
	Remove All Templates:

	Press 'c' to remove all enrolled fingerprint templates.
	Save Template:

	Press 'd' to save the captured fingerprint as a new template.
	Get Version:

	Press 'h' to retrieve the version information of the device.
	Wait for Finger:

	Press 'i' to initiate waiting for a finger to be placed on the sensor.
	Exit Program:

	Press 'q' to restart the device.
	Sending Commands:

	You can also enter any of the above commands directly into the text box on the web page and press 'Enter' to execute them.



	##Enroll Your Finger:
		Press 'a' to enroll a new fingerprint.
		Follow these steps to enroll your fingerprint:
		a. Place your finger on the fingerprint sensor.
		b. Wait for the device to capture your fingerprint data.
		c. The web interface will display a success message, indicating that your fingerprint has been enrolled.


	##Validate Your Fingerprint:
		Press 'b' to capture a fingerprint and identify it against the enrolled templates.
		Follow these steps to validate your fingerprint:
		a. Place your finger on the fingerprint sensor.
		b. The device will capture your fingerprint and compare it against the enrolled templates.
		c. If the captured fingerprint matches an enrolled template, the web interface will display a message indicating a successful match.
		d. If there is no match, the interface will display a message indicating that the fingerprint was not recognized.
		Please note that the device's LEDs and vibration motor may provide feedback during the enrollment and validation processes.

##4. Interacting with Results
	As you use different commands, the device will provide feedback through the web interface.
	The web page will display responses such as "Match with template ID: X", "No match", "Template saved with ID: X", and so on.
	The device LEDs and vibration motor may also provide visual and tactile feedback based on the command executed.

##5. Additional Information
	The device is equipped with NFC and fingerprint capabilities, allowing secure access control.
	Feel free to explore the code provided in the repository to understand more about the device's functionality and how it communicates with various components.
	That's it! You're now ready to enroll and validate fingerprints using your Chhavi NFC and Fingerprint Device. If you have any questions or encounter any issues, refer to the provided resources or contact our support team.

	Enjoy the convenience and security offered by your Chhavi device!