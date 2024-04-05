IoT 


Any reference books?
* 21 IoT Experiments - labs are all based on this
	* 15 bucks on kindle
* Raspberry Pi IoT Projects: Prototyping experiments for makers
	* Additional reference book

IoT Labs
* Gonna have to look at the powerpoint

Hardware requirements
- Raspberry Pi 3 B+ (or 4)
- USB keyboard and mouse
- HDMI monitor

Tools that might also be nice to have
- Adafruit Ladyada's Electronics Toolkit - soldering kit with heating/connecting wires
	- More available on syllabus

Syllabus again
- Seems to focus on pretty basic arduino stuff - kind of a retread of hardware course from last year until later down the line 

Intro to IoT
- The presence of IoT in today's world
	- IoT: Term for extension of existing internet structure to **billions of connected devices**
	- IoT is all around us
	- IoT helps improve quality of life
	- IoT system is usually made up of:
		- Controllers
		- Sensors
		- Actuators - influence the environment
		- Hardware
		- Software
IoT process flow
	A simple IoT system includes sensors connecting to actuators or controllers
		Thru wireless or wired connection

Building blocks of an IoT system
- Controllers (RasPi and Arduino)
	- Responsible for collecting data from sensors
	- Have ability to make immediate decisions
	- Adds intelligence to things
	- May send data to remote computers
	- Continuously analyzes and processes information
	- Uses actuators to modify conditions
- Actuators
	- **Performs an action**
	- Basic motor that can be used to control a system
	- Hydraulic, electric, or pneumatic
	- Responsible for transforming electrical signal into physical output
- Sensors
	- Device used to monitor and measure a physical property
	- May be connected to controller either directly or remotely

Processes in controlled systems
- Processes
	- Series of steps or actions taken to achieve a desired result
	- Uses inputs to execute required actions
- Feedback
	- When the output of a process affects the input
	- Referred to as feedback loop
	- Can provide positive or negative real-time information to controller based on behavior
	- Examples
		- Negative feedback: Shut off AC when temperature is low
		- Positive feedback: Turn on AC when temperature is high

Control systems
- Three components of a control system
	- Controller: Uses inputs and outputs to manage behavior of system
		- Attempts to achieve a desired state
	- Plant: The controlled portion of the system
	- Sensor: Measure a physical property
- Control theory: Choosing the adjustments to apply to a plant to achieve a desired output
	- Applied to many systems
		- Driving a car
		- Home automaton
		- Home security
		- Home thermostat
	- Car example
		- Input
			- Speed, direction, proximity to other cars
		- Action
			- Accelerate, brake, steer
		- Output
			- Control speed, direction, and proximity to other cars

- Closed-loop control systems
	- Uses feedback to determine whether the collected output is the desired output
	- Naming conventions come from circuit naming conventions so it's not always accurate

Models of communication
- Layered networking models are used to illustrate how a network operates and model how devices communicate
- Benefits include:
	- Assists in protocol design
	- Fosters competition
	- Decouples layers, prevents changes in one layer from impacting others
	- Provides **common language** to describe network functions and capabilities
- Physical, data link, and network layers: Concepts that are used to illustrate how network communication operates
	- TCP and UDP - standard transfer protocols
	- TCP is connection oriented, UTP is user oriented (non-connection oriented. send packet, pick a god and pray)

TCP/IP protocol suite and communication
- Application layer
	- Name system, host config, email, file transfer, web
- Transport layer
	- UDP and TCP
- Internet layer
	- IP, IP support, routing protocols
- Network access layer
	- PPP, ethernet, interface drivers

- For our purposes: We care about application and transport layer
