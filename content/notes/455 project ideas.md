
Interface with Daisy Seed / Arduino


### Project description

This project aims to create a motion sensor and alarm notification system. A distance sensor and Arduino microcontroller connected to a computer will be placed vertically against a doorway to detect when someone enters a room. If motion is detected, the Arduino + computer will send the current timestamp and distance data to an SQS queue. This queue will be connected to a lambda function that processes the data and formats it if necessary. When finished, the data will be put into another SQS queue. An Amplify web/mobile app will allow a user to view the most recent alarm events. The user will also be able to turn the alarm on or off, which starts or stops the lambda function from posting to the downward queue. Additional small features may be added to the app if I find any opportunities to add them during the development process.

### Design diagram
- Amplify for web app
- SQS for sending requests
- Lambda for processing requests or for receiving data from device
- Rekognition
- IoT to connect with arduino
- Arduino connection
	- Motion detecting sensor
	- Sends log to queue / lambda which processes more information
	
[[455 Diagram.canvas|455 Diagram]]