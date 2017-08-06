# Flight-Computer

=== PROJECT OUTLINE ===
I want to create a flight computer for use in scientific ballooning projects at the university and high school level. I have a bunch of research to do and am looking for collaborators with an expertise in this area.

NOTE: There are "flight computer" Arduino projects out there but these are data loggers or APRS beacons, not a system that can send commands to the balloon in flight and receive data.

=== REQUIREMENTS ===
The system needs to communicate with a scientific ballooning payload by using a packet radio (APRS) approach over ham radio frequencies. The ground station needs to send emergency commands (such as to initiate an unplanned cutdown) and receive critical data (payload temperature, battery condition, etc..)  It does not have to send position information - this will be accomplished through a separate APRS beacon. It does not need to receive scientific data - these will be stored on-board and recovered with the balloon payload after landing.

=== SELECTED APPROACH ===
Using the strengths of each system, the flight computer on the balloon will be an Arduino (the Mega, because it has more serial connections) and the base system will be a Raspberry Pi running Python.

=== CONCEPT TESTING ===
This approach will be tested in three steps over the summer and fall. Step 1 will be to connect the Arduino to the RPi through a wired serial connection and get them talking to each other. Step 2 will be to connect each device's serial I/O to a modem (terminal node controller or TNC), connected in turn to a ham radio to create a package. The two packages will communicate with each other over the air. Step 3 will be to move the two packages as far apart as possible, the goal being communication over a 20 mile line-of-sight separation. (The balloon is expected to reach a max altitude of 100,000 ft.)

=== FUTURE ===
Once concept testing is complete, development can begin on the actual flight systems. My goal is to make the solution open source. I am currently in an MSIS program and may use parts of this project for academic credit at some point. (Any input from collaborators will be appropriately cited.) Once shared with students, they will be able to fork this project for their own academic work.

=== REQUEST FOR INPUT ===
I have spent the past 20+ years tinkering with a variety of systems and relish the process of getting square pegs to fit in round holes. I'm not as good at whipping up code from scratch. Suggestions and links to resources would be greatly appreciated. (Please don't assume that I know much of anything - I certainly won't get bent out of shape if you're sharing something I already know!)

Thanks,
-- Markus
