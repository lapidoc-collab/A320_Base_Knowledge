Airbus A318/A319/A320/A321 (CFM56 & V2500) B1+B2 Technical Training
Manual
ATA 46 -- Information Systems Airframe Systems
Contact us Tel: +44(0) 1565 653745 Email: admin@catts.org.uk Web:
www.catts.org.uk Online Training: catts.learnupon.com/store
TRAINING MATERIAL DECLARATION These lecture notes are compiled by Civil
Aviation Technical Training Solutions Ltd (CATTS Ltd). Although
comprehensive in their detail, they are only intended for use with a
theoretical course of instruction and do not constitute a training
programme in their own right. When issued they are as up to date as
possible however, amendments will NOT be forwarded. THEY ARE FOR STUDY
PURPOSES ONLY AND MUST NOT BE USED FOR OPERATIONS OR MAINTENANCE
Click here to visit our new online training portal for HF, SFAR, EWIS
and many more. Contact us Tel: +44(0) 1565 653745 Email:
admin@catts.org.uk Web: www.catts.org.uk Online Training:
catts.learnupon.com/store
ATA Chapters Required in this Training Manual AIRFRAME SYSTEMS ATA 46
Information Systems
Contact us Tel: +44(0) 1565 653745 Email: admin@catts.org.uk Web:
www.catts.org.uk Online Training: catts.learnupon.com/store
Training Ma Manual Airbus A318/319/ A320/A321 (CFM56 & V2500) ATA 46
Airframe Systems; Information Systems Level 3
FOR TRAINING PURPOSES ONLY
INFORMATION SYSTEMS AIR TRAFFIC & INFO MANAGEMENT SYS (ATIMS) ATIMS
Description/Operation (3) . . . . . . . . . . . . . . . . . . . . . . .
. . . . . 2 ATIMS Warnings (3) . . . . . . . . . . . . . . . . . . . . .
. . . . . . . . . . . . . . . . . 6 ATIMS MCDU Menus Description (2) . .
. . . . . . . . . . . . . . . . . . . . . . 8 ATSU Router INIT & Tests
through MCDU (2) . . . . . . . . . . . . . . . . 16 ATIMS Interfaces (3)
. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
. 32
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 5 of 40
FOR TRAINING PURPOSES ONLY
ATIMS DESCRIPTION/OPERATION (3) ATSU The Air Traffic Service Unit (ATSU)
has been designed to take provision of all foreseen evolutions. The
modularity concept for the software (S/W) makes easy data link
capability during all Communication Navigation Surveillance and Air
Traffic Management (CNS/ATM) transitions. The ATSU S/W is partitioned
into two main parts: - aircraft interface/host platform and, - data link
applications.
AIRCRAFT INTERFACE/HOST PLATFORM SOFTWARE
-   hosted AOC applications. For the remote AOC applications, the ATSU
    only routes data to and from AOC peripherals. This routing is in
    charge of receiving ground messages and routing them to the right
    AOC peripheral and acquiring messages or reports from these
    peripherals and sending them to the ground. The hosted applications
    depend on airline definition and uploaded into the ATSU. These
    applications include standard and customized functions. The main
    functions are:
-   AOC menu display,
-   processing, printing and display of received messages,
-   generation, triggering and sending of messages.
The aircraft interface/host platform S/W is composed of four services: -
air/ground communication, used for the management of the air/ground
communication media, - Human-Machine Interface (HMI), used for the
management of the CNS/ATM cockpit interfaces: MCDU, printer and alert
function, - on-board peripherals, used for the management of the
communication with the on-board peripheral units: Data Management Unit
(DMU) part of the Flight Data Interface and Management Unit (FDIMU),
Centralized Fault Display Interface Unit (CFDIU), Flight Management
System (FMS) and cabin terminal, - system management, used for the
acquisition of the aircraft parameters for application S/W use and
monitoring of the system: power supply and BITE functions.
DATA LINK APPLICATION The data link applications include only Airline
Operational Control (AOC) for the pre-Future Air Navigation System
(FANS) configuration. The AOC applications are dedicated to data
communication services between the aircraft and the airline facility.
The AOC is composed of: - remote AOC applications and,
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 6 of 40
FOR TRAINING PURPOSES ONLY
ATSU - AIRCRAFT INTERFACE/HOST PLATFORM SOFTWARE & DATA LINK APPLICATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 7 of 40
FOR TRAINING PURPOSES ONLY
ATIMS DESCRIPTION/OPERATION (3) ATSU SOFTWARE LOADING The ATSU S/W is
uploaded via the Multipurpose Disk Drive Unit (MDDU). If a complete S/W
uploading is required, a de-selection of the ATSU data loading must be
carried out, for each type of S/W, so that a re-initialization of the
ATSU can be made until the DATALINK ATSU FAULT warning goes off on the
EWD.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 8 of 40
FOR TRAINING PURPOSES ONLY
ATSU SOFTWARE LOADING
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 9 of 40
FOR TRAINING PURPOSES ONLY
ATIMS WARNINGS (3) DATALINK ATSU FAULT
VHF3 VOICE
When there is an Air Traffic Service Unit (ATSU) failure, the message
"DATALINK ATSU FAULT" appears on the EWD, in this case, MASTER CAUTion
light and Single Chime (SC) will be activated, and no SD page is called.
When VHF Data Radio (VDR) 3, configured in VHF DataLink (VDL) mode 2, is
not available for data transmission, the right memo "VHF3 VOICE" appears
in green.
NOTE: In the INOP SYS column of the STATUS page, the ATSU fault message
appears.
ATSU STBY When the data link function is lost or unavailable or when
there is an ATSU router configuration failure, the left memo "COMPANY
DATALINK STBY" appears in green.
NOTE: VDR is capable VDL mode 2 when "ATSU installed" pin programming is
activated on the FWC. The VDL mode 2 function is used to reduce channel
saturation. With this function, the rate throughput is increased ten
times through a D8-PSK modulation (31,5 Kbit/s).
HF VOICE
NOTE: "ATSU installed" pin programming is activated on the FWC.
When all the HF Data Radio (HFDR) (if installed) are in voice mode, the
right memo "HF VOICE" pulses in green for 10 seconds and then stays
stable.
ATSU MSG
NOTE: HFDR1 with VDL mode 2 function for datalink is optional.
When an Airline Operational Control (AOC) message is received, the right
memo "COMPANY MSG" appears in green. NOTE: The right memo COMPANY ALERT
is displayed with a continuous buzzer sound, when the crew receives a
high importance message from the company.
ATSU CALL When a call request message is received, the right memo
"COMPANY CALL" appears in green.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 10 of 40
FOR TRAINING PURPOSES ONLY
DATALINK ATSU FAULT ... HF VOICE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 11 of 40
FOR TRAINING PURPOSES ONLY
ATIMS MCDU MENUS DESCRIPTION (2) GENERAL The MCDU gives the following
functions: - Airline Operational Control (AOC) hosted applications
and, - air-ground communication management.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 12 of 40
FOR TRAINING PURPOSES ONLY
GENERAL
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 13 of 40
FOR TRAINING PURPOSES ONLY
ATIMS MCDU MENUS DESCRIPTION (2) COMM MENU The air-ground communications
functions and services are active as soon as their initialization is
complete. NOTE: The AUDIT PRINT PAGE SET OFF function is used to disable
this function directly from this page without having to get access to
the AUDIT page.
COMM CONFIG The initialization through COMM CONFIG menu is considered as
completed when the Air Traffic Service Unit (ATSU) has received a valid
aircraft registration number, airline identification and scan mask. The
aircraft registration number and airline identification are used in the
air/ground communication as aircraft addressing means. The VHF3 SCAN SEL
gives an ordered list of authorized service providers usable for data
communications.
VHF3 DATA MODE The VHF3 DATA MODE page shows the various regions, which
can be selected. Each region is associated with a data link service
provider and a frequency.
VHF3 VOICE DIRECTORY The VHF3 VOICE DIRECTORY page fulfills the
following functions: - display a voice frequency directory, - activate
one of these frequencies, - select the data mode, - activate the voice
frequency contained in the last received CO CALL message, - manually
enter a frequency.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 14 of 40
FOR TRAINING PURPOSES ONLY
COMM MENU - COMM CONFIG ... VHF3 VOICE DIRECTORY
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 15 of 40
FOR TRAINING PURPOSES ONLY
ATIMS MCDU MENUS DESCRIPTION (2) COMM MENU (continued) COMM STATUS The
COMM STATUS pages are used to verify the communication status of ATSU: -
the air/ground communication media status; VHF3, SATCOM (if installed)
and HF 1 only (if HFDR installed), - the communication (router) status
of the on-board peripherals.
MAINTENANCE STATUS The MAINTENANCE menu is composed of three
functions: - TEST, which is used to test the link between the
communication media (VHF3, SATCOM and HF if installed) and the ground, -
STATISTICS used for media and router statistics: number of up linked
messages, number of down linked messages, - AUDIT to print out exchanged
messages per media and router depending on selection.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 16 of 40
FOR TRAINING PURPOSES ONLY
COMM MENU - COMM STATUS & MAINTENANCE STATUS
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 17 of 40
FOR TRAINING PURPOSES ONLY
ATIMS MCDU MENUS DESCRIPTION (2) AOC MENU The AOC MENU can be customized
and gives access to the hosted AOC applications loaded in the ATSU. The
CONFIG function gives access to a SYSTEM CONFIG page to verify that the
correct AOC software (S/W) and data base Part Number (PN) have been
successfully loaded into the ATSU.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 18 of 40
FOR TRAINING PURPOSES ONLY
AOC MENU
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 19 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) INITIALIZATION PROCEDURE OF
THE ATSU ROUTER GENERAL This procedure, called initialization of the Air
Traffic Service Unit (ATSU) router, enables the air-ground
communications functions and services of the ATSU to be activated. Four
essential parameters are required: - A/C ICAO CODE (24bit address sent
by the ATC Transponders), - a valid airline identification (ACARS and
STANDARD A/L ID), - a valid A/C registration number (A/C REGISTR) and, -
a valid scan mask. Otherwise, the DATALINK ATSU FAULT+ ATSU INIT FAULT
amber warnings are displayed on the Engine/Warning Display (EWD). NOTE:
According to the pin programming activated on the Flight Warning
Computer (FWC) ("ACARS installed" or "ATSU installed"), the ACARS STBY
green memo is displayed instead of the DATALINK ATSU FAULT+ATSU INIT
FAULT warning.
A/C REGISTRATION NUMBER AND FLIGHT IDENTIFICATION The A/C registration
number is sent by the Centralized Fault Display Interface Unit (CFDIU).
The ATSU creates the flight identification by concatenating the airline
identification parameter and the flight number parameter coming from the
Flight Management and Guidance Computer (FMGC). The airline
identification is not available and must be entered.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 20 of 40
FOR TRAINING PURPOSES ONLY
INITIALIZATION PROCEDURE OF THE ATSU ROUTER - GENERAL & A/C REGISTRATION
NUMBER AND FLIGHT IDENTIFICATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 21 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) INITIALIZATION PROCEDURE OF
THE ATSU ROUTER (continued) SCAN MASK VALIDATION The last parameter
required is the scan mask validation. The three VHF SCAN SELECT pages
give an ordered list of service providers usable for VHF data
communications. TEST TLS and TEST HAM are activated only for test and
shall not be selected for airline operations. The NEW SCAN SELECT
function is used to erase the previous selection. The VHF3 SCAN MASK is
compulsory for the router operation.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 22 of 40
FOR TRAINING PURPOSES ONLY
INITIALIZATION PROCEDURE OF THE ATSU ROUTER - SCAN MASK VALIDATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 23 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) INITIALIZATION PROCEDURE OF
THE ATSU ROUTER (continued) SCAN MASK VALIDATION (CON'T) The scan mask
must be a prioritized list of VHF service providers contracted by the
airline. Select one or more service providers in the appropriate
priority order to compose the scan mask. SITA EUR/AFR and ARINC AFRICA
are selected as an example. The SCAN SEL ACTIVATE allows the new
selection to be loaded into the ATSU. To finalize the initialization the
CONFIG ACTIVATE LSK in the COMM CONFIG menu must be pressed. When the
initialization of the ATSU router is completed, the DATALINK ATSU
FAULT + ATSU INIT FAULT warning goes off.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 24 of 40
FOR TRAINING PURPOSES ONLY
INITIALIZATION PROCEDURE OF THE ATSU ROUTER - SCAN MASK VALIDATION
(CON'T)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 25 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) INITIALIZATION PROCEDURE OF
THE ATSU ROUTER (continued) VHF3 DATA MODE PAGE A last check in the VHF3
DATA MODE page is required. The VHF3 DATA MODE page displays the data
link service providers selected in the VHF3 SCAN SELECT menu. The
initialization of the ATSU router is completed.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 26 of 40
FOR TRAINING PURPOSES ONLY
INITIALIZATION PROCEDURE OF THE ATSU ROUTER - VHF3 DATA MODE PAGE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 27 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) OPERATIONAL TEST VOICE MODE
TEST This procedure, called operational test of the ATSU, serves to
check the ATSU router configuration and test the voice mode. The
initialization of the ATSU router is completed. The ATSU automatically
controls data frequencies in the order defined in the VHF3 SCAN SELECT
menu, but a service provider can be manually selected. The VHF3 VOICE
DIRECTORY page serves: - to activate one of the displayed frequencies
configured by the Airline Operational Control (AOC) application, - to
activate the voice frequency requested by the ground (CO CALL), - to
manually enter a frequency and, - to go back to data mode. When the OPS
frequency is activated (132.225 given as an example), the ATSU controls
the VHF3 frequency in VOICE mode. On the Radio Management Panel (RMP),
the DATA indication stays in view in the active window. In this mode,
communication tests with the ground can be done.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 28 of 40
FOR TRAINING PURPOSES ONLY
OPERATIONAL TEST - VOICE MODE TEST
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 29 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) OPERATIONAL TEST (continued)
CONFIGURATION CHECK The modified configuration through the VHF3 DATA
MODE is checked. Then, a come back to the DATA MODE is performed. The
COMM STATUS pages are used to verify the communication status of ATSU: -
the air/ground communication media status: VHF3, SATCOM (if installed)
and HF (if HFDR installed), - the communication (router) status of the
on-board peripherals.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 30 of 40
FOR TRAINING PURPOSES ONLY
OPERATIONAL TEST - CONFIGURATION CHECK
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 31 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) VHF3 LINK TEST ATSU
INITIALIZATION CHECK This procedure, called VHF3 link test of the ATSU,
checks the VHF3 link between the A/C and the ground. A check of the ATSU
initialization is done through the VHF3 DATA MODE menu, the VHF3 VOICE
DIRECTORY menu and the COMM STATUS menu. VHF3 must be operational, the
VHF3 link available and in DATA mode.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 32 of 40
FOR TRAINING PURPOSES ONLY
VHF3 LINK TEST - ATSU INITIALIZATION CHECK
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 33 of 40
FOR TRAINING PURPOSES ONLY
ATSU ROUTER INIT & TESTS THROUGH MCDU (2) VHF3 LINK TEST (continued)
TEST The link test is accessible through the MAINTENANCE menu. The
result of this test confirms that the communication link between VHF3
and the ground is operational.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 34 of 40
FOR TRAINING PURPOSES ONLY
VHF3 LINK TEST - TEST
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 35 of 40
FOR TRAINING PURPOSES ONLY
ATIMS INTERFACES (3) AFS/ATIMS INTERFACE The Air Traffic Service Unit
(ATSU) is interfaced with the Flight Management and Guidance Computers
(FMGCs) and the MCDUs for Automatic Flight System (AFS).
Data Radio (HFDR) 1 (if installed) configured in HF DataLink (HFDL)
mode, the ATC Transponders, and the Radio Management Panels (RMPs) for
communication system.
FMGC The ATSU sends data to both FMGCs on an ARINC 429 bus and receives
data from both FMGCs on another one. The ATSU/FMGCs interface is used
for: - Airline Operational Control (AOC) hosted application for
acquisition of operational data: origin/destination airport, flight
number, fuel on board, - remote AOC application to exchange AOC
messages, - air-ground communication functions: flight number, Flight
Management System (FMS), - system management and configuration to
exchange data link communication status and configuration between ATSU
and FMGCs.
MCDU
The ATSU sends and receives data from VDR3 through ARINC 429 links
for: - data block exchanges and, - status transmission. The ATSU sends 2
discrete signals to VDR3 to control: - VDR3 switching between voice and
data mode, - port select for VDR3 frequency selection. NOTE: VDR is
capable VDL mode 2 when "ATSU installed" pin programming is activated on
the FWC. The VDL mode 2 function is used to reduce channel saturation.
With this function, the rate throughput is increased ten times through a
D8-PSK modulation (31,5 Kbit/s).
SDU1
The ATSU sends data to MCDUs on an ARINC 429 bus and receives data from
MCDUs on another one. The ATSU/MCDUs interface is used for: - the AOC
application to select the AOC mode, parameter entry (captain name, fuel
units...), display of AOC specific information (AOC received messages,
scratchpad messages...), and print command, - air-ground communication
functions is used to show the router specific information, crew requests
for router modes of operation and parameter entry, print command.
COMMUNICATION SYSTEMS/ATIMS INTERFACE The ATSU is interfaced with the
VHF Data Radio (VDR) 3 configured in VHF DataLink (VDL) mode 2, the
Satellite Data Unit (SDU), the HF
Airbus A318/A319/A320/A321 (CFM56 or V2500)
VDR3
CATTS LTD
The ATSU sends and receives data from SDU1 through ARINC 429 links
for: - data block exchanges and, - status transmission. NOTE: The
ATSU/SDU interface is optional.
HFDR1 The ATSU sends and receives data from HFDR1 through ARINC 429
links for: - data block exchanges and, - status transmission.
Issue 012 - Revision 000 - Dated 01/07/2023 Page 36 of 40
FOR TRAINING PURPOSES ONLY
NOTE: Based on the existing HF system provision or installation,
additional wiring provision is installed to make HFDR (optional) capable
of datalink mode communication. HF1 (and HF1 only) system will be
connected to the following systems: ATSU (only one HFDR connected).
ATSU acquires Universal Time Coordinated (UTC) time and date from the
clock on an ARINC 429 bus. As back-up of the clock, the MMR2 transmits
the UTC time and date from a GPS source, on an ARINC 429 bus.
ATC XPDR
The ATSU/FDIMU interface is used for flight performance in uplink
request and downlink AIDS reports. The ATSU: - sends uplink requests to
the FDIMU (DMU-part) on an ARINC 429 bus and, - receives downlink
reports from the FDIMU on an ARINC 429 bus. The ATSU/CFDIU interface is
used to transmit the data given below to the CFDIU on an ARINC 429
bus: - information about internal or detected external failures of the
Air Traffic and Information Management System (ATIMS), - uplink
requests. The ATSU acquires downlink reports and data necessary for AOC
application from the CFDIU on an ARINC 429 bus. The ATSU/printer
interface is used to print data. The ATSU: - sends printable data to the
printer on an ARINC 429 bus and, - receives status information from the
printer on another ARINC 429 bus. The ATSU/MDDU interface is used for
loading data. The ATSU: - sends and receives loading data with the MDDU
or a PDL through 2 ARINC 429 buses, - receives status information from
the MDDU on a discrete line. The ATSU/AINS plugs/Laptop (optional)
interfaces are used for loading data through ETHERNET buses. The ATSU: -
sends loading data to the laptop by the AINS plugs for documentation
consultation modules (FCOM, MEL, FCTM, AFM ...) and/or performance
calculation modules (take off, landing, in-flight, weight and
balance), - receives requests from personnel in the cockpit through the
laptop connected to the AINS plugs. The ATSU/CVR interface is used for
data recording from the CVR.
The ATSU uses for the VDL2 function the ICAO code (24 bit address) sent
by the ATC transponders. The ICAO code is first extracted from the ATC
transponder 1 and then from the ATC transponder 2 if the ATC transponder
1 is not available.
RMP The ATSU sends 1 discrete signal to the 3 RMPs to indicate which
entity is controlling the VDR3. The ATSU receives only 1 discrete signal
from the 3 RMPs, which is used to request the mode switching to the
ATSU.
INDICATING AND RECORDING SYSTEMS/ATIMS INTERFACE For the indicating
system, the ATSU is interfaced with the Flight Warning Computers (FWCs),
the System Data Acquisition Concentrators (SDACs), the Display
Management Computers (DMCs), the Multi-Mode Receiver 2 (MMR2) and the
clock. For the recording system, the ATSU is interfaced with the Data
Management Unit (DMU) part of the Flight Data Interface and Management
Unit (FDIMU), the Centralized Fault Display Interface Unit (CFDIU), the
printer, the Multipurpose Disk Drive Unit (MDDU) or a Portable Data
Loader (PDL) and the Cockpit Voice Recorder (CVR).
INDICATING SYSTEMS The ATSU sends warning information to the two FWCs on
ARINC 429 buses. It receives data that are necessary for AOC application
from the FWCs, SDACs and DMCs also on ARINC 429 buses. The
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
RECORDING SYSTEMS
Issue 012 - Revision 000 - Dated 01/07/2023 Page 37 of 40
FOR TRAINING PURPOSES ONLY
NOTE: The AINS plugs are used to connect the Electronic Flight Bag (EFB)
for customers who get the Less Paper in Cockpit (LCP) option. LCP
application will let the customer replace traditional paper by digital
information (Documentation/Performance calculation modules). In a
cockpit environment, it is necessary to purchase hardware (usually a
laptop) to use the LCP application.
CABIN TERMINAL/ATIMS INTERFACE The ATSU sends uplink requests to the
Digital Interface Unit (DIU) on an ARINC 429 bus and receives downlink
reports from the DIU on an ARINC 429 bus. NOTE: The ATSU/DIU interface
is optional.
LANDING GEAR/ATIMS INTERFACE The ATSU receives, from the Landing Gear
Control and Interface Unit (LGCIU), information on a discrete input to
determine if the aircraft is on ground or in flight.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 38 of 40
FOR TRAINING PURPOSES ONLY
AFS/ATIMS INTERFACE ... LANDING GEAR/ATIMS INTERFACE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 39 of 40
FOR TRAINING PURPOSES ONLY
Training Manual Airbus A318/319/ A320/A321 (CFM56 & V2500)
END
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 40 of 40
