Airbus A318/A319/A320/A321 (CFM56 & V2500) B1+B2 Technical Training
Manual
ATA 31 -- Indicating/Recording Systems Airframe Systems
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
ATA Chapters Required in this Training Manual AIRFRAME SYSTEMS ATA 31
Indicating & Recording Systems
ATA 31A
Instrument Systems
Contact us Tel: +44(0) 1565 653745 Email: admin@catts.org.uk Web:
www.catts.org.uk Online Training: catts.learnupon.com/store
Training Ma Manual Airbus A318/319/ A320/A321 (CFM56 & V2500) ATA 31
Airframe Systems; Indicating Systems EFIS ECAM and Instruments
Level 3
FOR TRAINING PURPOSES ONLY
INDICATING ELECTRONIC INSTRUMENT SYSTEM (EIS)
MAINTENANCE PRACTICE
EIS Architecture (2) . . . . . . . . . . . . . . . . . . . . . . . . . .
. . . . . . . . . . . . . 2 Engine/Warning Display Presentation (2) . .
. . . . . . . . . . . . . . . . . . . . 6 ECAM Warnings Presentation (2)
. . . . . . . . . . . . . . . . . . . . . . . . . . . 14 Indicating
System Control & Indicating (2) . . . . . . . . . . . . . . . . . . . .
22 EIS ECAM Normal and Manual Mode Description (3) . . . . . . . . . . .
24 ECAM Advisory & Failure Related Modes (3) . . . . . . . . . . . . . .
. . . 38 ECAM Description/Operation (3) . . . . . . . . . . . . . . . .
. . . . . . . . . . . 46 EFIS Description/Operation (3) . . . . . . . .
. . . . . . . . . . . . . . . . . . . . . 58 DMC ARINC BUS
Reconfiguration (3) . . . . . . . . . . . . . . . . . . . . . . 66 EIS
Abnormal Operation (3) . . . . . . . . . . . . . . . . . . . . . . . . .
. . . . . . 76 Indicating System Operation, Control & Indicating (3) . .
. . . . . . . . 108
Computer Removal and Installation (3) . . . . . . . . . . . . . . . . .
. . . . . 190 Pushbutton Removal and Installation (3) . . . . . . . . .
. . . . . . . . . . . . 192
CLOCK Electrical Clock D/O (2) . . . . . . . . . . . . . . . . . . . . .
. . . . . . . . . . . . . 110
CENTRALIZED FAULT DISPLAY SYSTEM (CFDS) CFDS Component location (2) . .
. . . . . . . . . . . . . . . . . . . . . . . . . . . 112 CFDS Fault
Processing (3) . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
. . . 116 CFDS Aircraft System Types (2) . . . . . . . . . . . . . . . .
. . . . . . . . . . . 122 CFDS Failure Classification (2) . . . . . . .
. . . . . . . . . . . . . . . . . . . . . 124 CFDS Reports (2) . . . . .
. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 132
CFDS Phases (3) . . . . . . . . . . . . . . . . . . . . . . . . . . . .
. . . . . . . . . . . 158 CFDIU Functions (3) . . . . . . . . . . . . .
. . . . . . . . . . . . . . . . . . . . . . . 160 Trouble Shooting
Procedure with CFDS (3) . . . . . . . . . . . . . . . . . . 164 Post
Flight Report Filtering Function (3) . . . . . . . . . . . . . . . . . .
. . . 174
PRINTER Printer Description/Operation (3) . . . . . . . . . . . . . . .
. . . . . . . . . . . . 182 Printer Paper Loading (2) . . . . . . . . .
. . . . . . . . . . . . . . . . . . . . . . . . 184
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 5 of 198
FOR TRAINING PURPOSES ONLY
EIS ARCHITECTURE (2) EFIS-ECAM
INPUTS
The Electronic Instrument System (EIS) is shown on 6 identical Liquid
Crystal Display (LCD) units and controlled through the EIS control
panels. The Electronic Centralized Aircraft Monitoring (ECAM) displays
are identical and controlled through the ECAM Control Panel (ECP). The
Electronic Flight Instrument System (EFIS) displays are controlled by
the EFIS control panels and the lighting/loudspeaker control panels.
The inputs received by the FWC are used to elaborate red warnings.
Various items of information for systems like engines, fuel, navigation
and which do not agree with a warning, are directly sent to the DMCs.
The inputs received by the SDACs are used by the DMCs to display system
pages and by the FWCs to generate most of amber warnings.
DMC The Display Management Computers (DMCs) are data concentrators and
receive data from aircraft sensors and systems. They send them to the
Display Units (DUs). The DUs compute and display the images on each
unit. In normal operation DMC1 drives the CAPT Primary Flight Display
(PFD), the CAPT Navigation Display (ND), Engine/Warning Display (EWD)
and System Display (SD). In normal operation DMC 2 drives the F/O PFD
and ND DUs. If DMC 1 fails, it is automatically replaced by DMC 2 for
ECAM only. DMC 2 cannot drive the CAPT PFD and ND; a manual switching to
DMC 3 is required. DMC 3 can drive any of the six DUs. DMC 3 is a hot
spare awaiting the failure of DMC 1 or 2 and can be switched to drive
the DUs linked to the failed DMC. Data loading of the DMC 1 is possible
with Portable Data Loader (PDL).
FWC The Flight Warning Computers (FWCs) monitor the aircraft systems.
Each FWC generates all warning and caution messages, supplies the
attention getters, computes the flight phase and provides aural
warnings.
SDAC The System Data Acquisition Concentrators (SDACs) receive various
signals from the aircraft systems and send them to the FWCs and to the
DMCs.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 6 of 198
FOR TRAINING PURPOSES ONLY
EFIS-ECAM ... INPUTS
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 7 of 198
FOR TRAINING PURPOSES ONLY
EIS ARCHITECTURE (2) COMPONENT LOCATION The EIS computers are located in
the aft avionics rack.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 8 of 198
FOR TRAINING PURPOSES ONLY
COMPONENT LOCATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 9 of 198
FOR TRAINING PURPOSES ONLY
ENGINE/WARNING DISPLAY PRESENTATION (2) GENERAL The Engine/Warning
Display (EWD) is normally on the upper Display Unit (DU), it is divided
into upper and lower areas. The EWD is dedicated to the presentation of
information.
EWD INFORMATION On the upper area are permanently displayed: - Primary
engine parameters, - Slat/flap position indication, - Fuel On Board
(FOB). On the lower area are displayed: - Memos, failure messages and
actions to be performed. During TakeOff (TO) and landing, most of the
warnings are inhibited.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 10 of 198
FOR TRAINING PURPOSES ONLY
GENERAL - EWD INFORMATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 11 of 198
FOR TRAINING PURPOSES ONLY
ENGINE/WARNING DISPLAY PRESENTATION (2) ADVISORY AND STATUS INDICATION
There are conditions when additional symbols are displayed, on the EWD
lower area. The symbols are ADV (Advisory), STS (Status) and a green
arrow (overflow).
ADVISORY INDICATION The symbol Advisory (ADV) located on the lower part
of the EWD is displayed with pulsing in the following cases: - When the
crew has performed a manual selection for a SD page and there is an
advisory on another SD page. - When a failure has been detected by the
FWC and there is an advisory on another SD. - When there are several
advisories on several SD page. In this case, the SD page which contains
the first detected advisory is displayed. However, ADV symbol will be
pulsing in order to indicate to the crew that there are one or several
advisories. NOTE: Note: ADV indication is pulsing for both Dual and
Single EWD display mode for EIS2. For EIS1, ADV symbol is displayed with
pulsing on the EWD, only for Mono Display mode when an advisory has been
detected.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 12 of 198
FOR TRAINING PURPOSES ONLY
ADVISORY AND STATUS INDICATION - ADVISORY INDICATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 13 of 198
FOR TRAINING PURPOSES ONLY
ENGINE/WARNING DISPLAY PRESENTATION (2) ADVISORY AND STATUS INDICATION
(continued) STATUS INDICATION Status (STS) indicates that a status
message is present on the SD STS page. NOTE: Note: Status (STS)
indication is not shown on the EWD when the status page is displayed on
the lower ECAM DU.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 14 of 198
FOR TRAINING PURPOSES ONLY
ADVISORY AND STATUS INDICATION - STATUS INDICATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 15 of 198
FOR TRAINING PURPOSES ONLY
ENGINE/WARNING DISPLAY PRESENTATION (2) ADVISORY AND STATUS INDICATION
(continued) ARROW INDICATION The overflow arrow in green color indicates
that warning messages exceed the capacity of the display on the left
memo area.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 16 of 198
FOR TRAINING PURPOSES ONLY
ADVISORY AND STATUS INDICATION - ARROW INDICATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 17 of 198
FOR TRAINING PURPOSES ONLY
ECAM WARNINGS PRESENTATION (2) ECAM DISPLAY WITH AIRCRAFT SYSTEM FAILURE
In case of aircraft system failure, an aural warning, the Single Chime
(SC), a visual warning and the MASTER CAUTion, attract your attention.
The Engine/Warning Display (EWD) indicates the title of the failure and
the actions to take. On the status and System Display (SD), the
hydraulic page is called automatically. The CLeaR P/Bs come on and as
long as the failure is not cleared, they stay on. On the hydraulic panel
the FAULT lights come on, indicating the P/Bs to release out. NOTE: In
this module, parameters are given for a CFM engine. For an IAE engine,
the parameters will be shown as follows: Engine Pressure Ratio (EPR),
EGT, N1 and N2). The graphics show an example of sequence of Electronic
Centralized Aircraft Monitoring (ECAM) displays in case of green
hydraulic system fault. This may be different to your aircraft
configuration.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 18 of 198
FOR TRAINING PURPOSES ONLY
ECAM DISPLAY WITH AIRCRAFT SYSTEM FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 19 of 198
FOR TRAINING PURPOSES ONLY
ECAM WARNINGS PRESENTATION (2) CREW CORRECTIVE ACTIONS CORRECTIVE
ACTIONS When you press the MASTER CAUT, it goes off. Then, actions
indicated on the EWD have to be done. First, switch OFF the Power
Transfer Unit (PTU) P/B on the hydraulic panel, and then switch OFF the
GREEN ENGine 1 PUMP P/B.
RESULTS The corrective actions have been taken. All the FAULT lights are
off. On the EWD, the messages associated to the corrective action have
disappeared. On the left hand side of the EWD, the result of the failure
appears indicating that it is a primary failure. On the right hand side,
the secondary failures are displayed.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 20 of 198
FOR TRAINING PURPOSES ONLY
CREW CORRECTIVE ACTIONS - CORRECTIVE ACTIONS & RESULTS
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 21 of 198
FOR TRAINING PURPOSES ONLY
ECAM WARNINGS PRESENTATION (2) CLEARING OF THE WARNINGS When you press
CLR, on the left hand part of the EWD the title of the failure
disappears and MEMO messages come back. The system page corresponding to
the first secondary failure is displayed. When you press CLR again, the
title of the first secondary failure disappears. The system page
associated with the next secondary failure is displayed. When you press
CLR a third time, the title of the secondary failure disappears. The
MEMO message comes back on the right hand part of the EWD. The STATUS
page is displayed.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 22 of 198
FOR TRAINING PURPOSES ONLY
CLEARING OF THE WARNINGS
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 23 of 198
FOR TRAINING PURPOSES ONLY
ECAM WARNINGS PRESENTATION (2) STATUS REMINDER AND RECALL FUNCTION When
you press CLR a last time, the STATUS reminder STS on the EWD indicates
that the STATUS page is not empty and the CLR P/Bs go off. On the status
page, the cruise page (related to the present flight phase) comes back.
The warning has been cleared. The ReCalL P/B lets the crew reactivate
the Liquid Crystal Display (LCD) presentation of an alert inhibited
either through the flight phase or by the CLR function.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 24 of 198
FOR TRAINING PURPOSES ONLY
STATUS REMINDER AND RECALL FUNCTION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 25 of 198
FOR TRAINING PURPOSES ONLY
INDICATING SYSTEM CONTROL & INDICATING (2) EIS WARNING PRESENTATION
CLOCK and ND CHRONO CFDS MENU on GROUND PFR PRESENTATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 26 of 198
FOR TRAINING PURPOSES ONLY
This Page Intentionally Left Blank
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 27 of 198
FOR TRAINING PURPOSES ONLY
EIS ECAM NORMAL AND MANUAL MODE DESCRIPTION (3) GENERAL The Electronic
Centralized Aircraft Monitoring (ECAM) gives to the flight crew the
aircraft system displays. The ECAM shows data on two Liquid Crystal
Display (LCD) units, the upper ECAM is the Engine/Warning Display (EWD)
and the lower ECAM is the System Display (SD). These LCDs are fully
interchangeable.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 28 of 198
FOR TRAINING PURPOSES ONLY
GENERAL
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 29 of 198
FOR TRAINING PURPOSES ONLY
EIS ECAM NORMAL AND MANUAL MODE DESCRIPTION (3) ENGINE/WARNING DISPLAY
PRESENTATION The EWD gives the essential data necessary to monitor
engine parameters, warnings, cautions, checklist, and memos to the
flight crew. The upper area is related to engine primary parameters,
fuel on board and slat/flat position. These parameters are given in
analog and/or digital form. The lower area is dedicated to
warning/caution and memo messages. Warnings and memos are automatically
generated by the Flight Warning Computer (FWC). The left memo area is
dedicated to warnings and cautions (primary or independent failures) or
memo information related to procedural pilot actions or memo
information. The right memo area is dedicated to the system affected by
a warning or a caution (secondary failure) or memo information related
to the phase inhibition (takeoff and landing only) or temporary pilot
actions (ANTI ICE ON) or special lines (AP OFF).
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 30 of 198
FOR TRAINING PURPOSES ONLY
ENGINE/WARNING DISPLAY PRESENTATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 31 of 198
FOR TRAINING PURPOSES ONLY
EIS ECAM NORMAL AND MANUAL MODE DESCRIPTION (3) SYSTEM DISPLAY
PRESENTATION The SD is divided into 2 areas: - the upper area displays
system or status pages, - the lower area is dedicated to permanent data.
The SD can display one of 11 system pages, cruise page or status page.
In normal operation, the SD automatically shows the system pages
according to the current flight phase. Nevertheless manual page
selection is always possible. The CRUISE page is automatically displayed
in flight (no manual selection). It displays the main system parameters
to monitor during the flight. Priority is given to automatic display.
The status page is an operational summary of the current aircraft
condition. The information is displayed at the end of an ECAM procedure
or upon crew request. The status page includes: - the limitation,
approach procedures, information and cancelled cautions are displayed in
the left column, - the inoperative systems below the caption "INOP SYS"
and any class 2 system failure below the caption "MAINTENANCE" are
displayed in the right column. At the bottom of the SD, below the grey
line is the permanent data. It is always displayed whatever system page
is present. Total Air Temperature (TAT) and Static Air Temperature (SAT)
are digital values. International Standard Atmosphere (ISA) is in fact a
delta ISA indication that appears only in standard barometric reference
mode only. The captions (TAT, SAT, ISA, GW ) are displayed in white and
the units in cyan. The values are normally displayed in green. Load
factor (G LOAD) is only displayed amber when the value is above 1.4 G or
below 0.7 G for more than 2 seconds. The information remains in view for
5 seconds, when the excessive condition has disappeared. The display of
the load factor is inhibited during flight phases 1 & 2.Feedback to the
flight crew by providing system messages can also be
Airbus A318/A319/A320/A321 (CFM56 or V2500)
displayed in amber above or below the time indication. In case of
degraded value, last 2 digits are dashed, in case of No Computed Data
(NCD), 3 blues dashes replaces the values (on ground). Status, advisory
and overflow are indications on the display. The advisory (ADV), appears
by pulsing in white to indicate that an aircraft system parameter has
drifted out of its normal operating range. In ECAM single display mode,
the related page pushbutton will also flash on the ECAM Control Panel
(ECP) to indicate to the crew which system page is affected by an
advisory. The status (STS) indicates that a status message is on the
ECAM status page. It appears below the grey stripe at the same location
as the overflow arrow provided that this one is away. This message
indicates to the pilot that the status page is no more empty. The
overflow arrow indicates that the warning messages exceed the capacity
of the display on the left memo area (7 lines). In this case, the
heading titles of the warning messages are displayed on the right memo
area.
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 32 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM DISPLAY PRESENTATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 33 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM DISPLAY PRESENTATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 34 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM DISPLAY PRESENTATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 35 of 198
FOR TRAINING PURPOSES ONLY
EIS ECAM NORMAL AND MANUAL MODE DESCRIPTION (3) ECAM MODES The ECAM
operates in four modes for the system page presentation with a priority
order: - the normal mode according to the flight phase is automatically
presented in case of an aircraft configuration change, - the failure
mode is automatically presented when warning/caution is triggered, - the
advisory mode is automatically presented when a parameter is drifting, -
the manual mode, through the ECP. NOTE: Note that the manual mode is
cancelled in case of a warning or an advisory.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 36 of 198
FOR TRAINING PURPOSES ONLY
ECAM MODES
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 37 of 198
FOR TRAINING PURPOSES ONLY
EIS ECAM NORMAL AND MANUAL MODE DESCRIPTION (3) retracted. The TO
INHIBIT message disappears. The CRUISE page disappears when the landing
gear is selected down and ALT below 16000ft.
ECAM MODES (continued) AUTOMATIC MODE In normal operation the ECAM
system pages are displayed according to the current flight phase, this
mode is called automatic mode. A flight is divided into 10 phases
corresponding to an aircraft configuration change. These flight phases
are generated by the FWC and used by the Display Units (DUs) to
automatically call up the system pages. DOOR (phase 1) The APU or engine
pages are displayed in priority if the APU or the engines are started,
in any flight phase. The APU page appears when APU master switch is
switched ON. It disappears when APU master switch is switched OFF or the
APU RPM is above 95% for 10 seconds. The ENGINE page appears at the
beginning of the start sequence, and disappears 10 seconds after this
start sequence.
WHEEL (phase 7,8,9) During these phases, most warnings are inhibited.
"LDG INHIBIT" is displayed on the right memo area of the EWD. "LDG
INHIBIT" message disappears (flight phase 9). DOOR (phase 10) Five
minutes after the last engine shutdown the FWC starts a new flight leg
at phase 1.
WHEEL (phase 2) The WHEEL page is displayed only after the engine start
has been completed, and the Engine Start switch is returned to the
Normal position. The FLighT ConTroL page replaces the WHEEL page for 20
seconds when either sidestick is moved or when rudder deflection is
above 22 degrees. ENGINE (phase 3,4,5) During these phases, most
warnings are inhibited. TO INHIBIT is displayed on the right memo area
of the EWD. CRUISE (phase 6) The CRUISE page appears as soon as the
slats are retracted and the engines are not at take off power, provided
that the landing gear is
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 38 of 198
FOR TRAINING PURPOSES ONLY
ECAM MODES - AUTOMATIC MODE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 39 of 198
FOR TRAINING PURPOSES ONLY
EIS ECAM NORMAL AND MANUAL MODE DESCRIPTION (3) ECAM MODES (continued)
MANUAL MODE When one of the system key is pressed, the corresponding
system page is displayed on the SD and the ECP key light comes on. When
the key is pressed a second time, the key light extinguishes, and the
page corresponding to the flight phase or current warning is displayed
again. In the event of an ECAM control panel failure, due to the built
in redundancy, the system pages are still available through the ALL key.
When the ALL key is pressed and held, all the system pages are displayed
successively in one second intervals. This key, when pressed repeatedly,
will enable the display of the next system page.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 40 of 198
FOR TRAINING PURPOSES ONLY
ECAM MODES - MANUAL MODE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 41 of 198
FOR TRAINING PURPOSES ONLY
ECAM ADVISORY & FAILURE RELATED MODES (3) The level 2 system failure has
no direct consequence on flight safety.
ALERT CLASSIFICATION
LEVEL 1
GENERAL The alerts are classified in three levels. They depend on the
importance and urgency of the corrective actions required. - level 3:
warnings (highest priority) - level 2: cautions - level 1: cautions -
status messages At each level, the alert messages are also classified by
priority order.
LEVEL 3 Level 3 corresponds to an emergency configuration. Corrective or
palliative action must be taken by the crew immediately. These warnings
are associated with: - Continuous Repetitive Chime (CRC) or specific
sound, - warning messages on Liquid Crystal Display (LCD), - MASTER
WARNing light flashing red. Typical level 3 warnings are: - aircraft in
dangerous configuration or limit flight conditions (Stall, overspeed), -
system failure altering flight safety (Engine fire, excess cabin
altitude), - serious system failure (Dual hydraulic failure).
Level 1 agrees with a configuration requiring crew monitoring, mainly
failures leading to a loss of redundancy or degradation of a system. The
attention getters (lights and sounds) are not activated by a level 1
alert.
STATUS Some defects which do not trigger warnings or cautions, but which
require further maintenance actions, will be indicated to the crew by
means of a status indication, pulsing after engine shutdown. It is
necessary to call the status page manually to see the title of the
affected system.
LEVEL 2 Level 2 agrees with an abnormal configuration. Immediate crew
awareness is required, but not immediate corrective action. The crew
must decide when to take the corrective action. These warnings are
associated with: - Single Chime (SC), - MASTER CAUTion light amber, -
warning messages on LCD.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 42 of 198
FOR TRAINING PURPOSES ONLY
ALERT CLASSIFICATION - GENERAL ... STATUS
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 43 of 198
FOR TRAINING PURPOSES ONLY
ECAM ADVISORY & FAILURE RELATED MODES (3) TYPE OF FAILURE
NOTE: This part can be used if necessary to display heading titles of
warnings if the left part of the EWD is full.
GENERAL The failures may be of three different types, independently of
their classification. There are 3 separate types of warnings or
cautions: - those associated with an independent failure, - those
associated with a primary failure, - those associated with a secondary
failure.
INDEPENDANT FAILURE An independent failure is a failure, which affects
an isolated item of equipment or system without affecting another one.
Example: Flight Warning Computer (FWC) 1 failure. NOTE: An independent
failure is displayed with the title underlined.
PRIMARY FAILURE A primary failure is a failure of an item of equipment
or system causing the loss of other equipment. Example: Green hydraulic
system failure may lead to the loss of a pair of spoilers. NOTE: A
primary failure is displayed with a box around the failure.
SECONDARY FAILURE A secondary failure is a loss of an item of equipment
or system resulting from a primary failure. Example: Loss of a pair of
spoilers after a hydraulic system failure. The titles of the system
pages corresponding to the secondary failures are indicated on the lower
right part of the Engine/Warning Display (EWD) by an asterisk.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 44 of 198
FOR TRAINING PURPOSES ONLY
TYPE OF FAILURE - GENERAL ... SECONDARY FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 45 of 198
FOR TRAINING PURPOSES ONLY
ECAM ADVISORY & FAILURE RELATED MODES (3) ADVISORY ADVISORY MODE IN
NORMAL DUAL DISPLAY The value of some critical system parameters is
monitored by an advisory mode. In Electronic Centralized Aircraft
Monitoring (ECAM) normal display, when there is a deviation of a value
from its normal range, the related system page is displayed
automatically to get the crew attention before this value gets to the
warning or caution level. The affected parameter gives pulses. The
related key light on the ECAM Control Panel (ECP) is on steady. The
flashing symbol ADV is displayed on the lower part of the EWD when: -
The crew did the manual selection of an SD page and there is an advisory
on another SD page. - A failure is detected by the FWC and there is an
advisory on another SD. - There are many advisories on different SD
pages. When this occurs, the SD page which contains the first detected
advisory is displayed. But the ADV symbol will flash to indicate to the
crew that there are one or more advisories. Example: The ELEC page will
be displayed if the IDG temperature increases above its normal value,
but is still below the threshold of the warning. NOTE: An advisory can
possibly lead to a failure, but not always. They are totally independent
one from the other.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 46 of 198
FOR TRAINING PURPOSES ONLY
ADVISORY - ADVISORY MODE IN NORMAL DUAL DISPLAY
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 47 of 198
FOR TRAINING PURPOSES ONLY
ECAM ADVISORY & FAILURE RELATED MODES (3) ADVISORY (continued) ADVISORY
MODE IN ECAM MONO DISPLAY In ECAM MONO display mode (one ECAM LCD
remaining), when a value drifts from its normal range, a white ADV
message flashes in the center of the EWD to attract crew attention. As
the corresponding system page cannot be displayed automatically on the
System Display (SD), the pilot has to fetch the information on the ECP:
the associated key light flashes to indicate which system is concerned.
NOTE: The ELEC system page is given as an example.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 48 of 198
FOR TRAINING PURPOSES ONLY
ADVISORY - ADVISORY MODE IN ECAM MONO DISPLAY
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 49 of 198
FOR TRAINING PURPOSES ONLY
ECAM DESCRIPTION/OPERATION (3) GENERAL PRESENTATION The Electronic
Centralized Aircraft Monitoring (ECAM) performs three main functions: -
Data acquisition and concentration, - Data warning computation, -
Warning announcement and data display. Data acquisition is shared
between the System Data Acquisition Concentrators (SDACs),the Flight
Warning Computers (FWCs) and the Display Management Computers (DMCs).
Data warning computation and memo are achieved by the FWCs, warning
announcements and data display are made through loudspeakers and Display
Units (DUs).
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 50 of 198
FOR TRAINING PURPOSES ONLY
GENERAL PRESENTATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 51 of 198
FOR TRAINING PURPOSES ONLY
ECAM DESCRIPTION/OPERATION (3) ECAM SYSTEM ECAM system components are: -
SDACs, - FWCs, - DMCs, - ECAM Control Panel (ECP).
SDAC The two SDACs are identical and interchangeable. \[ The SDACs
acquire A/C systems malfunction/failure data corresponding to caution
situations and send them to the FWCs for generation of the corresponding
alert and procedure messages. \[ The two SDACs also acquire and send to
the 3 DMCs A/C system signals necessary for the display of system
information. The ECP is the user interface to the ECAM system.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 52 of 198
FOR TRAINING PURPOSES ONLY
ECAM SYSTEM - SDAC
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 53 of 198
FOR TRAINING PURPOSES ONLY
ECAM DESCRIPTION/OPERATION (3) ECAM SYSTEM (continued) SDAC DATA
PROCESSING Therefore, each parameter acquired is given to the two SDACs.
All the signals (discrete, analog, digital) entering the SDACs are
converted into digital format and delivered on their output buses under
ARINC 429. The SDACs copy certain parameters to distribute them to other
equipment in digital form (ARINC 429).
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 54 of 198
FOR TRAINING PURPOSES ONLY
ECAM SYSTEM - SDAC DATA PROCESSING
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 55 of 198
FOR TRAINING PURPOSES ONLY
ECAM DESCRIPTION/OPERATION (3) ECAM SYSTEM (continued) FWC The two FWCs
are interchangeable. Each FWC generates alphanumeric codes corresponding
to all texts and messages to be displayed on \[ the ECAM DUs. \[ The
aural warnings and synthetic voices are delivered by the FWCs to the
cockpit loudspeakers. The FWCs compute all warnings and cautions. The
FWCs perform three main functions: - Data acquisition, - Flight phase
computation, - Data warning computation corresponding to warning
situations. The FWCs outputs/inputs are: - Discrete for visual attention
getters, - Analog for audio signals, - ARINC 429 called FWC DATA BUS, -
RS 422 called FWC MESSAGE BUS. Each FWC sends a copy of its own
acquisition through an ARINC 429 bus to the opposite FWC. The FWCs
provide aural and visual information in order to: - Show, in real time,
all the system failures and dangerous configurations with their level of
seriousness, - Identify the systems or circuits affected by a failure, -
Provide the appropriate corrective action.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 56 of 198
FOR TRAINING PURPOSES ONLY
ECAM SYSTEM - FWC
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 57 of 198
FOR TRAINING PURPOSES ONLY
ECAM DESCRIPTION/OPERATION (3) ECAM SYSTEM (continued) DMC The three
DMCs are identical and interchangeable. The DMCs receive data from the
A/C systems, either directly or through the SDACs and FWCs. The 3 DMCs
can be considered as data concentrators and receive data from A/C
sensors and systems in order to merge and send them to the DUs through
ARINC 629 output buses. Moreover, the DMCs insure: - The interface
between EIS and the other A/C computers and systems, - The information
exchange between the displays, - The tele-loading of the operational
software. The DMCs acquire and send several types of signals for ECAM: -
Discrete, - ARINC 629 bus, - ARINC 429 bus, - RS 232 buses for workshop
test, - ARINC 453 bus (just passing through).
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 58 of 198
FOR TRAINING PURPOSES ONLY
ECAM SYSTEM - DMC
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 59 of 198
FOR TRAINING PURPOSES ONLY
ECAM DESCRIPTION/OPERATION (3) ECP INTERFACE The ECAM interface
includes: - ECAM control panel, - The warning and caution lights, - The
loudspeaker, - The DUs. The ECP is a control and display unit. \[ It
transmits selections to the FWCs and DMCs, \[ it receives DMC data to
illuminate the keys lights. \[ The ECP outputs discretes for CLEAR
(CLR), RECALL (RCL), STATUS (STS) and emergency cancel (EMER CANC) keys
are linked to the FWCs. The output discrete for ALL key is directly
linked to the DMCs. \[ It is also linked to the DUs for ON/OFF
brightness control.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 60 of 198
FOR TRAINING PURPOSES ONLY
ECP INTERFACE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 61 of 198
FOR TRAINING PURPOSES ONLY
EFIS DESCRIPTION/OPERATION (3) GENERAL The Electronic Flight Instrument
System (EFIS) consists of two main components: - Display Management
Computers (DMCs), - Display Units (DUs). The DMCs receive Air
Data/Inertial Reference System (ADIRS), navigation systems, Flight
Management (FM), Flight Guidance and Envelope System (FGES), flight
controls, engines and Flight Warning Systems (FWSs) required by the DUs
in order to generate Primary Flight Display (PFD) and Navigation Display
(ND) symbologies.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 62 of 198
FOR TRAINING PURPOSES ONLY
GENERAL
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 63 of 198
FOR TRAINING PURPOSES ONLY
EFIS DESCRIPTION/OPERATION (3) DMC The three DMCs are identical and
interchangeable, they receive A/C system data on ARINC 429 buses,
weather radar information on ARINC 453 high-speed bus, \[ analog signal
for the brightness control, \[ discrete signal for the PFD/ND transfer
and PFD/ND ON/OFF. DMCs send data on an ARINC 629 link to the DUs. \[
When a new DMC 1, 2 or 3 is installed, the relevant software must be
downloaded into it, this is done by cross loading from DMC 1, 2 or 3 via
the MCDU. If a new software must be loaded, it is first done on DMC 1
from the Multipurpose Disk Drive Unit (MDDU), then a cross loading has
to be performed. \[ When a new DU is installed, a cross loading from the
corresponding DMC has to be performed via the MCDU. The DMC BITE test is
performed and the results are stored for later transfer to the
Centralized Fault Display System (CFDS). It is possible to read this
information via the MCDU. NOTE: Note: The software includes DMC (EFIS,
ECAM) and DU (EFIS, ECAM) data.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 64 of 198
FOR TRAINING PURPOSES ONLY
DMC
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 65 of 198
FOR TRAINING PURPOSES ONLY
EFIS DESCRIPTION/OPERATION (3) DISPLAY UNIT (ND) The DUs are identical
and interchangeable. They are Liquid Crystal Displays. Each DU receives
digital signals from \[ its related DMC through an ARINC 629 link, and
also through an ARINC 453 high-speed bus for the weather radar link. The
NDs provide this information according to the modes selected on the EFIS
control panel (part of the Flight Control Unit). The modes are \[
ROSE-ILS, ROSE-VOR, ROSE-NAV, \[ ARC, and \[ PLAN.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 66 of 198
FOR TRAINING PURPOSES ONLY
DISPLAY UNIT (ND)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 67 of 198
FOR TRAINING PURPOSES ONLY
EFIS DESCRIPTION/OPERATION (3) DISPLAY UNIT (PFD) The PFDs provide
flight information for A/C control, including A/C attitude, \[ airspeed,
\[ altitude, \[ heading and \[ Automatic Flight System modes. A METRIC
ALT pushbutton can be installed on the FCU. If you push this pushbutton,
the selected altitude is displayed in meters above the altitude scale.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 68 of 198
FOR TRAINING PURPOSES ONLY
DISPLAY UNIT (PFD)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 69 of 198
FOR TRAINING PURPOSES ONLY
DMC ARINC BUS RECONFIGURATION (3) GENERAL As a general rule, the Display
Management Computer (DMC) uses the active aircraft system source for
display, provided it is valid or selected.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 70 of 198
FOR TRAINING PURPOSES ONLY
GENERAL
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 71 of 198
FOR TRAINING PURPOSES ONLY
DMC ARINC BUS RECONFIGURATION (3) FWC Each DMC receives both Flight
Warning Computer (FWC) 1 and 2 data buses. The DMCs preferably work with
the FWC1 data. If the data is not valid or if FWC 1 is not valid, the
DMCs will automatically switch to the FWC 2 Data bus. NOTE: the RS 422
buses are used by the FWCs to send text messages (warnings, MEMO and
status) to the DMCs.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 72 of 198
FOR TRAINING PURPOSES ONLY
FWC
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 73 of 198
FOR TRAINING PURPOSES ONLY
DMC ARINC BUS RECONFIGURATION (3) SDAC Each DMC receives and processes
the data from each of the two System Data Acquisition Concentrators
(SDACs). The DMCs use SDAC 1 data providing it is valid. All data
transfer is by ARINC 429. If the data is not valid or if SDAC 1 is not
valid, the DMCs will use the data from SDAC 2.The switching is
automatic.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 74 of 198
FOR TRAINING PURPOSES ONLY
SDAC
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 75 of 198
FOR TRAINING PURPOSES ONLY
DMC ARINC BUS RECONFIGURATION (3) DMC OUTPUT BUSES Each DMC transmits
data on two ARINC 429 buses: -One high speed switched bus: FWC, ECAM
Control Panel (ECP), Air Traffic Service Unit (ATSU), Flight Data
Interface Management Unit (FDIMU), -One low speed unswitched bus:
Centralized Fault Display Unit (CFDIU). When the EIS DMC Selector Switch
is set to CAPT 3 (or F/O 3), DMC 1 (or DMC 2) sends through its output
bus the data received from DMC3. The switching is done inside DMC 1 (or
DMC 2).
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 76 of 198
FOR TRAINING PURPOSES ONLY
DMC OUTPUT BUSES
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 77 of 198
FOR TRAINING PURPOSES ONLY
DMC ARINC BUS RECONFIGURATION (3) WEATHER RADAR Each DMC receives the
weather radar (WXR) transceivers (XCVRs) or the Enhanced Ground
Proximity Warning Computer (EGPWC) data via four ARINC 453 data buses
{D1 and D2}. The DMCs retransmit the ARINC 453 bus to the EFIS DUs. As
only one WXR XCVR is in operation at a time, the DMCs process
information from the one in operation. The WXR enable discrete disables
the operation if the plan mode is selected on the EFIS controller.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 78 of 198
FOR TRAINING PURPOSES ONLY
WEATHER RADAR
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 79 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) EIS ABNORMAL OPERATION In order to ensure
reliability of the displayed data, the Electronic Instrument System
(EIS) has three main types of reconfiguration: - In the case of single
or multiple Display Unit (DU) failures, - In the case of single or
multiple Display Management Computer (DMC) failures, - In the case of
external (sensor/computer) source failure.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 80 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 81 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE Many failures
could occur on the EIS like: - Primary Flight Display (PFD), -
Navigation Display (ND), - Electronic Centralized Aircraft Monitoring
(ECAM) Upper or lower DU, - Multiple DU, - ECAM Control Panel (ECP), -
System Data Acquisition Concentrator (SDAC), - Flight Warning Computer
(FWC), - DMC.
PFD DU FAILURE In the case of PFD failure (detected) or if the PFD unit
is switched off by means of its potentiometer, the PFD is automatically
displayed on the ND unit.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 82 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - PFD DU FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 83 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) PFD DU
FAILURE (PFD/ND XFR) The PFD/ND transfer (XFR) P/BSW provides the crew
with the possibility to recover the ND image on the ND unit, if
necessary. Display change is performed by software switching of the
PFD/ND outputs inside the DMC.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 84 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - PFD DU FAILURE (PFD/ND XFR)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 85 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) ND DU
FAILURE In the case of ND unit failure the crew has the possibility to
present the ND image by pressing the PFD/ND XFR P/BSW.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 86 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - ND DU FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 87 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) ND DU
FAILURE (PFD/ND XFR) The ND screen stays instead of the PFD screen until
the PFD/ND XFR P/BSW is pressed again.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 88 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - ND DU FAILURE (PFD/ND XFR)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 89 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) UPPER
ECAM DU FAILURE In the case of an upper display (EWD) failure or if the
upper display control potentiometer is turned to off, the upper display
is automatically transferred on the lower display, this mode is called
ECAM single display mode.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 90 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - UPPER ECAM DU FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 91 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) UPPER
ECAM DU FAILURE (SYSTEM PAGE RECOVERING) In this case a system page can
be recovered by pushing and holding a system key on the ECP or by
rotating the ECAM/ND XFR selector on the switching panel in order to
display the system page on the ND side.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 92 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - UPPER ECAM DU FAILURE (SYSTEM PAGE
RECOVERING)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 93 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) LOWER
ECAM DU FAILURE In case of lower DU failure or if the lower display is
turned to off, no automatic reconfiguration is possible, the ECAM works
in single display mode. Each crew member also has the possibility to
present the SD image on the ND side only, and never on the PFD side, by
rotating the ECAM/ND transfer selector switch on the switching panel.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 94 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - LOWER ECAM DU FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 95 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) BOTH
ECAM DU FAILURE (ECAM ND XFR) In case of EWD unit and SD unit failure,
each crew member has the possibility to permanently present the EWD on
the ND unit by rotating the ECAM/ND transfer selector switch on the
switching panel.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 96 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - BOTH ECAM DU FAILURE (ECAM ND XFR)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 97 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) BOTH
ECAM DU FAILURE (SYSTEM PAGE RECOVERING) It is still possible to recover
a system page by pushing and holding a system key on the ECP.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 98 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - BOTH ECAM DU FAILURE (SYSTEM PAGE
RECOVERING)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 99 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued)
MULTIPLE DU FAILURE (SAME SIDE) In the case of PFD unit and ND unit
failure (on the same side) no reconfiguration is possible.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 100 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - MULTIPLE DU FAILURE (SAME SIDE)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 101 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) ECAM
CONTROL PANEL FAILURE If the ECP fails, the main functions, emergency
cancel (EMER CANC), clear (CLR), recall (RCL), all (ALL) and status
(STS) remain available.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 102 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - ECAM CONTROL PANEL FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 103 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) SDAC
FAILURE In the case of a SDAC failure, there is no operational
consequence due to the redundancy of the EIS, the following message is
displayed on the EWD: FWS SDAC 1 (or SDAC 2) FAULT. In case both SDACs
fail the amber cautions and most of the system displays are lost. The
following message is displayed on the EWD: FWS SDAC 1+2 FAULT. ENG,
FUEL, F/CTL and WHEEL ECAM page data is available because it is already
in ARINC 429 format and not affected by SDAC failure.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 104 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - SDAC FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 105 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) FWC
FAILURE In the case of a FWC failure, there is no operational
consequence due to the redundancy of the EIS, the following message is
displayed on the EWD: FWS FWC1 FAULT or FWS FWC2 FAULT. All attention
getters and loudspeakers remain operative. If the DMCs receive no valid
data from both FWCs, the message FWS FWC1 + 2 FAULT is displayed on the
EWD. All other EWD messages, aural warnings and attention getters are
lost.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 106 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - FWC FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 107 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) SINGLE OR MULTIPLE FAILURE (continued) DMC
FAILURE If DMC1 fails, DMC2 will automatically drive the ECAM DUs. The
CAPT has to switch to DMC3 by rotating the EIS DMC switch on the
switching panel to CAPT3 in order to recover also EFIS DUs through DMC3.
If DMC 2 fails, the F/O has to switch to DMC3 by rotating the EIS DMC
switch on the switching panel to F/O 3. Either the CAPT or the F/O may
select the DMC3.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 108 of 198
FOR TRAINING PURPOSES ONLY
SINGLE OR MULTIPLE FAILURE - DMC FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 109 of 198
FOR TRAINING PURPOSES ONLY
EIS ABNORMAL OPERATION (3) EXTERNAL SOURCE INFORMATION FAILURES In the
case of external source information failures, the lost information
appears in red on the PFD or ND. It is possible to recover certain
information by following the EWD instructions: in this example "ATT HDG
SWTG F/O" on the switching panel. This enables manual source
reconfiguration for attitude and heading data. On the EWD, the failed
component is also displayed.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 110 of 198
FOR TRAINING PURPOSES ONLY
EXTERNAL SOURCE INFORMATION FAILURES
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 111 of 198
FOR TRAINING PURPOSES ONLY
INDICATING SYSTEM OPERATION, CONTROL & INDICATING (3) ADVISORY MODE
INDEPENDENT, PRIMARY and SECONDARY FAILURE FAILURE CLASSIFICATION and
CFDS MENU in FLIGHT SDAC and FWC Failure + ATA Review
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 112 of 198
FOR TRAINING PURPOSES ONLY
This Page Intentionally Left Blank
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 113 of 198
FOR TRAINING PURPOSES ONLY
ELECTRICAL CLOCK D/O (2) CHRONOMETER
AIR PRECISION CLOCK TEST To test the clock, the annunciator light switch
must be set to TEST. Then all the display windows should show eights.
UTC AND DATE When the clock is in normal configuration it displays the
time. The date is displayed by pressing the SET turn and P/B when the
time of the day is displayed. By pressing the SET turn and P/B once more
the time of the day will be displayed again.
UTC SETTING The setting of the Universal Time coordinated (UTC) is done
with the UTC selector. When the selector is in SET position, the second
digits are blanked, the minute digits flash and the hour digits are
frozen. By rotating the SET button clockwise the minutes increase,
anticlockwise the minutes decrease. By pushing the SET button the hours
flash, the minutes are frozen and the seconds are blanked. By turning
the SET button, hours can be adjusted. When the UTC selector is moved
from SET to INT the clock starts running from the adjusted time with the
second digits at 00. When the UTC selector is in Global Positioning
System (GPS) position, the clock is synchronized on the GPS time, if a
GPS signal is present.
A first press on the CHRonometer P/B starts the chronometer, a second
press stops it and freezes the display, and a press on the ReSeT P/B
resets it.
ELAPSED TIME To activate the Elapsed Time (ET) function, the ET selector
must be set to RUN. When set to STP, the ET counter stops, and the
display is frozen. To reset the display, the selector must be set to RST
(spring loaded position) and it returns to STP.
FAILURE With a clock failure or a loss of power supply, the digital
displays are no longer available. With a loss of main electrical power
supply, the time is still counted in memory through the A/C battery
supply, except for the CHR and ET functions.
DATE SETTING The setting of the date is done with the UTC selector. By
pressing the SET button, the date is displayed. By setting the UTC
selector in SET position, the year digits flash and the month and day
digits are frozen. By turning the SET button clockwise or anticlockwise,
years can be modified to obtain the chosen value. By pushing the SET
button, the months and days can be adjusted in the same way.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 114 of 198
FOR TRAINING PURPOSES ONLY
AIR PRECISION CLOCK - TEST ... FAILURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 115 of 198
FOR TRAINING PURPOSES ONLY
CFDS COMPONENT LOCATION (2) SYSTEM OVERVIEW The Centralized Fault
Display Interface Unit (CFDIU) centralizes and memorizes all information
concerning A/C system failures. Reading or printing of the failure
information is done in the cockpit with any MCDU or the printer. Most
A/C system computers have a BITE. The BITE permanently monitors the
system operation. When a failure is detected, it is stored in the BITE
memory and is transmitted to the CFDIU. The ECAM, which generate warning
and status messages, delivers these data to the CFDIU as well.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 116 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM OVERVIEW
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 117 of 198
FOR TRAINING PURPOSES ONLY
CFDS COMPONENT LOCATION (2) COMPONENT LOCATION The Centralized Fault
Display System (CFDS) computers are located in the aft avionics rack.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 118 of 198
FOR TRAINING PURPOSES ONLY
COMPONENT LOCATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 119 of 198
FOR TRAINING PURPOSES ONLY
CFDS FAULT PROCESSING (3) (LAST) LEG REPORT and the CURRENT (LAST) LEG
ECAM REPORT. In flight the CFDS always operates in the normal mode.
BITE Most aircraft system computers are equipped with a Built-In Test
Equipment (BITE). The BITE, which is an electronic device (hard + soft),
monitors permanently the system operation. When a failure is detected,
it is stored in the BITE memory and is transmitted to the Centralized
Fault Display Interface Unit (CFDIU). Memorization of the 64 previous
legs report is done by most of the BITEs.
MENU MODE In this mode, the CFDIU dialogues with one computer at a time
in order to read the contents of its BITE memory and to initiate various
tests. This mode can only be selected on ground and interrupts the
normal mode of operation.
MEMORIZATION Memorization of failures is different when the aircraft is
on ground or in flight. The full BITE functions and memorization operate
in flight. On ground, the memorization is done only in the BITEs. The
BITEs are provided with flight and ground memory zones.
CFDIU The CFDIU centralizes all information concerning aircraft system
failures. Reading or printing of all the failure information is done in
the cockpit. The Centralized Fault Display System (CFDS = CFDIU + BITEs)
functions are accessed through the MCDUs. The Flight Warning Computers
(FWCs) send the ECAM messages to the CFDIU by ARINC429 data busses. The
CFDIU will memorize these messages to generate the CURRENT LEG/LAST LEG
ECAM REPORT.
CFDS MODES Two CFDS modes are available: NORMAL and MENU modes. The MENU
MODE is available only on ground.
NORMAL MODE In this mode, the CFDIU scans all the connected system
outputs and memorizes the failure messages in order to generate the
CURRENT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 120 of 198
FOR TRAINING PURPOSES ONLY
BITE ... CFDS MODES
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 121 of 198
FOR TRAINING PURPOSES ONLY
CFDS FAULT PROCESSING (3) REPORTS LAST/CURRENT LEG REPORT A CURRENT LEG
REPORT is elaborated during the flight. After the flight, its title
becomes LAST LEG REPORT. The purpose of this item is to present the
failure messages, concerning all systems, occurred during the
last/current flight. Each message contains the test of the failure, the
ATA reference and the flight phase and time at which the failure
occurred. A function correlates the "SOURCE" failure message with the
"resulting" failure messages. SOURCE: Name of system affected by a
failure. IDENTIFIER: Name of system affected by an external failure,
which is correlated with the "SOURCE" failure. The CFDIU capacity for
failure messages memorization is up to 40 lines.
MESSAGES with the associated time, flight phase and ATA reference allow
the maintenance crew to make a correlation for easier trouble-shooting.
Beginning of PFR recording: - if flight number inserted prior to first
engine start, first engine started + 3 minutes. - if not, aircraft speed
\> 80 knots. End of PFR recording: Aircraft speed \< 80 knots + 30
seconds.
LAST/CURRENT LEG ECAM REPORT A CURRENT LEG ECAM REPORT is elaborated
during the flight. After the flight, its title becomes LAST LEG ECAM
REPORT. The purpose of this item is to present the warning messages
displayed on the upper ECAM display unit during the last/current flight.
These are primary or independent warnings. Each message contains the
ECAM warning, the ATA reference and the flight phase and time at which
the warning was triggered. When several identical and consecutive
warnings are transmitted, the CFDIU memorizes the first occurrence only
and carries on counting with a maximum of 8. The occurrence counter is
displayed between brackets at the end of the message. The CFDIU capacity
for warning messages memorization is up to 40 lines.
POST FLIGHT REPORT The Post Flight Report (PFR) is the sum of the LAST
LEG REPORT and of the LAST LEG ECAM REPORT. The PFR can only be printed
on ground. The list of ECAM WARNING MESSAGES and FAULT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 122 of 198
FOR TRAINING PURPOSES ONLY
REPORTS - LAST/CURRENT LEG REPORT ... POST FLIGHT REPORT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 123 of 198
FOR TRAINING PURPOSES ONLY
CFDS FAULT PROCESSING (3) INTERNAL/EXTERNAL FAILURES Each BITE can make
the difference between an internal and an external failure. Let us
suppose that an Angle-Of-Attack (AOA) sensor failure has been detected
and that systems A, B and C are affected by this failure. The Air Data
System (ADS) will transmit an internal failure while systems A, B and C
will transmit an external failure.
FAILURE GRAVITY The failures are classified according to their
importance: - class 1 failures are the most serious ones and require an
immediate maintenance action subject to the Minimum Equipment List
(MEL). - class 2 failures may have consequences if a second failure
occurs. A class 2 failure must be repaired within 10 days. - class 3
failures can be left uncorrected until the next scheduled maintenance
check.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 124 of 198
FOR TRAINING PURPOSES ONLY
INTERNAL/EXTERNAL FAILURES & FAILURE GRAVITY
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 125 of 198
FOR TRAINING PURPOSES ONLY
CFDS AIRCRAFT SYSTEM TYPES (2) TYPE 1 SYSTEMS Most systems are type 1
systems. These systems can memorize failures, which occurred in the last
64 flight legs. Type 1 systems are connected to the Centralized Fault
Display Interface Unit (CFDIU) via an ARINC 429 input bus and an ARINC
429 output bus.
The discrete input permits to initiate the test or reset. The discrete
output indicates if the system is OK or not. Example: Transformer
Rectifier Unit (TRU)
SINGLE COMPUTER The first configuration in TYPE 1 is a single computer.
Example: VHF 1 Transceiver.
MULTI COMPUTER The second configuration in TYPE 1 includes several
computers in the same aircraft system. One computer concentrates the
maintenance data of the other computers. Example: Flight Management and
Guidance Computers (FMGC) and Flight Augmentation Computer (FAC) with
FMGC 1 as A, FMGC 2 as B and FAC 1 as C.
DUPLICATED SYSTEM A duplicated system includes two different subsystems
in the same computer. Example: Air Data Inertial Reference Unit (ADIRU)
with ADR as subsystem 1 and IR as subsystem 2.
TYPE 2 SYSTEM Type 2 systems memorize only failures from the last flight
leg. The discrete signal is provided to initiate the test of the system.
Example: Avionic Electronic Ventilation Computer (AEVC).
TYPE 3 SYSTEM Type 3 systems are simple systems linked to the CFDS by
only two discrete signals. Type 3 systems cannot memorize failure
messages.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 126 of 198
FOR TRAINING PURPOSES ONLY
TYPE 1 SYSTEMS ... TYPE 3 SYSTEM
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 127 of 198
FOR TRAINING PURPOSES ONLY
CFDS FAILURE CLASSIFICATION (2) CLASS 1 Class 1 failures have an
operational consequence on the flight. You can display the class 1
failures on the MCDU: - in the LAST (or CURRENT) LEG REPORT. - in the
LAST (or CURRENT) LEG ECAM REPORT. These faults are also indicated to
the crew in flight: - by the ECAM system (upper and/or lower Display
Unit (DU)). - by local warning in the cockpit. Refer to the Minimum
Equipment List (MEL): "GO", "GO IF" or "NO GO".
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 128 of 198
FOR TRAINING PURPOSES ONLY
CLASS 1
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 129 of 198
FOR TRAINING PURPOSES ONLY
CFDS FAILURE CLASSIFICATION (2) CLASS 2 Class 2 failures have no
immediate operational consequence and can be displayed on request on the
ECAM STATUS page, under the MAINTENANCE title. You can display the class
2 failures on the MCDU: - in the LAST (or CURRENT) LEG REPORT. - in the
LAST (or CURRENT) LEG ECAM REPORT. A class 2 failure has to be repaired
within 10 days. Refer to the MEL: "GO" without condition. The example
given here concerns the Cabin Intercommunication Data System (CIDS)
fault.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 130 of 198
FOR TRAINING PURPOSES ONLY
CLASS 2
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 131 of 198
FOR TRAINING PURPOSES ONLY
CFDS FAILURE CLASSIFICATION (2) CLASS 3 Class 3 failures have no
operational consequence. All aircraft systems remain available. These
faults are not indicated to the crew but you can display the name of the
systems affected by at least a class 3 failure in the AVIONICS STATUS
(only available on ground). Do not refer to the MEL. Class 3 failures
have no fixed time for correction. However, correction is recommended to
improve the dispatch reliability. Class 3 failures may be corrected
during the A CHECK programmed maintenance operations.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 132 of 198
FOR TRAINING PURPOSES ONLY
CLASS 3
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 133 of 198
FOR TRAINING PURPOSES ONLY
CFDS FAILURE CLASSIFICATION (2) SYNTHESIS Class 1 and 2 failures are
displayed in the LAST (or CURRENT) LEG REPORT and in the LAST (or
CURRENT) LEG ECAM REPORT. AVIONICS STATUS displays, on ground, the title
of the systems currently affected by any failure class.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 134 of 198
FOR TRAINING PURPOSES ONLY
SYNTHESIS
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 135 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) GENERAL On ground, all the functions are available. In
flight, only CURRENT LEG REPORT and CURRENT LEG ECAM REPORT are
available. NOTE: Note: The Centralized Fault Display System (CFDS) menu
comprises two pages.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 136 of 198
FOR TRAINING PURPOSES ONLY
GENERAL
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 137 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) LAST/CURRENT LEG REPORT The LAST LEG REPORT shows
failure information delivered by the Built-in Test Equipments (BITEs) of
the aircraft systems. It can store up to 40 failures occurred during the
last leg. Pressing the Slat Flap Control Computer (SFCC) channel 1 (3L)
line key allows access to the related IDENTIFIERS page. The LAST LEG
REPORT shows the internal failures (class one and two) only. The
SOURCE/IDENTIFIERS page shows the list of systems affected by the source
failure, which is an external failure for them. On the ground, the title
of this item is LAST LEG REPORT. In flight, it is CURRENT LEG REPORT.
When the report is shown on several pages, an arrow appears on the top
right-hand corner. The key helps you to see the following pages. If you
select the key on the last page, you come back to the first page. When
you select the PRINT line key, all the LAST LEG REPORT is printed, even
if it contains several pages.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 138 of 198
FOR TRAINING PURPOSES ONLY
LAST/CURRENT LEG REPORT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 139 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) LAST/CURRENT LEG ECAM REPORT The LAST LEG ECAM REPORT
shows the list of Electronic Centralized Aircraft Monitoring (ECAM)
warning messages sent to the Centralized Fault Display Interface Unit
(CFDIU) by the Flight Warning Computers (FWC). It can store up to 40
warnings occurred during the last leg. On ground, the title of this item
is LAST LEG ECAM REPORT; in flight it is CURRENT LEG ECAM REPORT.
Documentary data appears on the print report: - the A/C
identification, - date and Greenwich Mean Time (GMT), - the flight
number, - the city pair. When you select the PRINT line key, all the
LAST LEG ECAM REPORT is printed.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 140 of 198
FOR TRAINING PURPOSES ONLY
LAST/CURRENT LEG ECAM REPORT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 141 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) PREVIOUS LEGS REPORT At each new flight leg, the
content of the LAST LEG REPORT is transferred into the PREVIOUS LEGS
REPORT. This report can store up to 200 failures over the last 64 flight
legs. The PREVIOUS LEGS REPORT is displayed only on ground. Each failure
message contains the same kind of data as the LAST LEG REPORT. For
example: FEB 22 1312 22-00-00 NO FAC 1 DATA (INTM) It also contains a
flight leg counter relative to the previous flight. XX is the number of
flight legs before the last flight leg. For example: 01 (previous leg).
NOTE: As the leg number changes at ground/flight transition, the content
of the LAST LEG REPORT is stored and identified in the PREVIOUS LEGS
REPORT under the LEG -01. At flight/ground transition, the LAST LEG
REPORT in the PREVIOUS LEGS REPORT is identified as 00. "INTM" means
that the failure has occurred intermittently. When you make a print of
the PREVIOUS LEGS REPORT, only the displayed page is printed.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 142 of 198
FOR TRAINING PURPOSES ONLY
PREVIOUS LEGS REPORT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 143 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) AVIONICS STATUS The AVIONICS STATUS presents the list
of systems, which are currently affected by a failure. This function is
only available on ground. The information presented is permanently
updated. The message contains the name of the system presently affected
by a failure, i.e. VHF3, or a NO X DATA message when the related system
bus is not active. For example: NO ILS 2 DATA The AVIONICS STATUS also
indicates the class 3 failures. (CLASS 3) means that the system is
affected by at least one class 3 failure. Note that there could also be
class 1 or 2 failures. When you make a print, all the AVIONICS STATUS
report is printed even if it contains several pages.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 144 of 198
FOR TRAINING PURPOSES ONLY
AVIONICS STATUS
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 145 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) PREVIOUS LEGS REPORT
SYSTEM REPORT/TEST The SYSTEM REPORT/TEST function is available on the
ground only. It enables a dialogue between the CFDS and one system
computer. The SYSTEM REPORT/TEST menu page presents the list of all the
systems connected to the CFDIU, in ATA chapter order. An example of each
system type is available: - in Landing Gear (L/G) for type 1 systems, -
in Air Conditioning (AIRCOND) for type 2 systems, - in Electrical (ELEC)
for type 3 systems.
This function presents the internal and external failure messages
concerning this system that appeared during the previous 64 flights. The
failure messages contain the name of the failed LRU associated with the
time and date at which the failure occurred, the flight number (-00 to
-63) and the ATA reference.
LRU IDENTIFICATION This function presents the Part Number (PN) of the
LRUs.
SYSTEM REPORT/TEST-BSCU A (Type 1 system) Type 1 systems are the most
common systems. The menu they present depends on the system itself. In
the MENU mode, the menu is transmitted by the system itself. You talk
directly with the system. The menu includes three basic functions: - the
LAST LEG REPORT, - the PREVIOUS LEGS REPORT, - the LRU IDENTIFICATION,
and optional functions, depending on the system for example: - TROUBLE
SHOOTING DATA, - CLASS 3 FAULTS, - TEST, - GROUND SCANNING.
LAST LEG REPORT This function presents the internal and external failure
messages concerning this system that appeared during the last flight.
These failure messages contain the name of the failed Line Replaceable
Unit (LRU) associated with the time at which the failure occurred and
the ATA reference.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 146 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM REPORT/TEST & SYSTEM REPORT/TEST-BSCU A (TYPE 1 SYSTEM)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 147 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) SYSTEM REPORT/TEST-BSCU A (Type 1 system) (continued)
TROUBLE SHOOTING DATA This item presents complementary information
concerning the failures for trouble shooting at level 3 (engineering
maintenance). These messages contain data constituting a snapshot of the
system environment at the moment of the failure or contain parameters
internal to the computer (Aircraft configuration, valve positions,...).
This information is presented on MCDU in hexadecimal language. When
required, the Trouble Shooting Manual (TSM) gives the interpretation of
the message.
CLASS 3 faults This item presents class 3 failure messages concerning
this system that appeared during previous flights. These failure
messages contain the name of the equipment affected by a class 3 fault
associated with the time, the date, the flight number and the ATA
reference.
TEST This item initiates system tests and shows the test results on the
MCDU. The CFDIU transmits the code of the line key (TEST) to the system.
The system BITE executes its test and may display a wait message to the
CFDIU when the test lasts for a long time. At the end of the test, the
BITE transmits the test results to the CFDIU for display.
GROUND SCANNING This item presents the internal and external failures
concerning this system and which are present when the request is made
(on ground only). This report is established by forcing the operation of
the BITE in system normal mode (same BITE operation as in flight).
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 148 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM REPORT/TEST-BSCU A (TYPE 1 SYSTEM) - TROUBLE SHOOTING DATA ...
GROUND SCANNING
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 149 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) SYSTEM REPORT/TEST-AEVC (Type 2 system) Type 2 systems
present a menu with one basic function, the LAST LEG REPORT and optional
functions depending on the system. Unlike Type 1 systems, Type 2 systems
do not have a Menu Mode. These functions are presented on the MCDU by
the CFDIU: you are in PSEUDO-MENU mode. You do not talk directly to the
system. The system permanently transmits its data on the system bus, and
the CFDIU reads them, except for the test. The menu includes one basic
function: - the LAST LEG REPORT, and optional functions depending on the
system, for example here - TEST, - CLASS 3 FAULTS.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 150 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM REPORT/TEST-AEVC (TYPE 2 SYSTEM)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 151 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) SYSTEM REPORT/TEST-GCU EMER (Type 3 system) Type 3
systems present only one function on their menu. Type 3 systems have no
MENU mode. The available functions are shown by the CFDIU. The only
possible functions are TEST or RESET. When you make a test or a reset,
the CFDIU initiates the test or the reset, receives the result and shows
it on the MCDU.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 152 of 198
FOR TRAINING PURPOSES ONLY
SYSTEM REPORT/TEST-GCU EMER (TYPE 3 SYSTEM)
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 153 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) POST FLIGHT REPORT The POST FLIGHT REPORT (PFR) is the
sum of the LAST LEG REPORT and of the LAST LEG ECAM REPORT. It is only
available on the printer. ECAM WARNING MESSAGES show/give the LAST LEG
ECAM REPORT. FAULT MESSAGES show/give the LAST LEG REPORT.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 154 of 198
FOR TRAINING PURPOSES ONLY
POST FLIGHT REPORT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 155 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) GMT/DATE INIT The GMT/DATE INIT function is available
only in case of clock failure and CFDIU power interrupt. In normal
operation, the CFDIU receives the time from the clock. In the event of
main clock failure, the CFDIU transmits the time and the date using its
internal clock. The CFDIU shows the time on the ECAM Display Unit (DU).
Re initialization of the time and the date will be only necessary after
a power cut-off. It shall be carried out on MCDU through the GMT/DATE
INIT function. GMT and date are entered by using the scratchpad.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 156 of 198
FOR TRAINING PURPOSES ONLY
GMT/DATE INIT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 157 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) REPORTS PROGRAMMING This item sends the automatic
transmission, via the Air Traffic Service Unit (ATSU), or printing of
the following functions: - PFR, - real time failures, - real time
warnings and, - avionics data. If "YES" is selected for the send and
print columns, the CFDIU will automatically transmit or print the PFR at
the end of the flight or the failures and warnings in real time. For
avionics data, "YES" in the send column, means that the system pages
will be sent to the ground when the operator requests a print. A star
beside "YES" or "NO" means that these items are modifiable. The
programming of the send column is given by the ATSU and the programming
of the print control for the avionics data is given by the system
itself.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 158 of 198
FOR TRAINING PURPOSES ONLY
REPORTS PROGRAMMING
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 159 of 198
FOR TRAINING PURPOSES ONLY
CFDS REPORTS (2) PFR FILTER PROGRAM The purpose of this function is to
improve the operational use of the PFR, CURRENT/LAST LEG ECAM REPORT and
LAST LEG REPORT, by filtering all the spurious or unjustified
failures/messages. It concerns the PFR printed at the end of the flight
as well as the real-time failure and warning information transmitted by
the ATSU.
FILTER ACTIVATED The filter database is activated after correct
uploading. It can be deactivated then activated again through the second
page of the main maintenance menu by pushing line key 4L then 2L. This
database is adapted from Service Information Letter (SIL) 0028 under
diskette form. It must be periodically updated.
PRINT FILTER CONTENT Action on line key 3R starts the printing of the
maintenance filter database.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 160 of 198
FOR TRAINING PURPOSES ONLY
PFR FILTER PROGRAM - FILTER ACTIVATED & PRINT FILTER CONTENT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 161 of 198
FOR TRAINING PURPOSES ONLY
CFDS PHASES (3) LEG REPORT is renamed under the title LAST LEG REPORT
and is stored in the PREVIOUS LEGS REPORT.
GROUND/FLIGHT TRANSITION Transition to flight (Event 1) is defined at
the soonest or at the latest depending on whether the flight number has
been entered by the crew before take-off or not: - at the soonest: First
engine start + 3 minutes if flight number entered prior to first engine
start. - at the latest: Aircraft speed \> 80 knots if flight number not
entered prior to first engine start. At event "1", the leg number is
incremented.
IN FLIGHT PHASE From event 1 until aircraft speed has been below 80
knots for 150 seconds, type 1 and 3 systems are considered in flight.
NOTE: As the leg has not changed, the content of the LAST LEG REPORT is
identified in the PREVIOUS LEGS REPORT under the LEG -00.
ON GROUND PHASE On ground, the system BITEs ensure: - detection (Type
1/2/3 systems) and memorization in their ground memory (Type 1/2
systems) of internal faults only, - transmission to the CFDIU of
internal faults for monitoring and establishment of the AVIONICS STATUS.
All Centralized Fault Display System (CFDS) functions (e.g. PFR
printing) are available on request through the MCDUs.
NOTE: Type 2 systems are only considered in flight from 30 seconds after
lift off up to touch down. In flight, the system Built-In Test Equipment
(BITE) ensures: - detection (Type 1/2/3 systems) and memorization in
their flight memory (Type 1/2 systems only as type 3 system BITEs do not
have any memory) of internal and external faults, - transmission to the
Centralized Fault Display Interface Unit (CFDIU) of internal and
external faults for memorization and establishment of the CURRENT LEG
REPORT. This in flight phase corresponds to the Post Flight Report (PFR)
recording time (Beginning and end of fault and Electronic Centralized
Aircraft Monitoring (ECAM) warning message memorization in the CFDIU).
FLIGHT/GROUND TRANSITION Transition to ground occurs when, after touch
down, the aircraft speed has been below 80 knots for 150 seconds. At
this time, the CURRENT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 162 of 198
FOR TRAINING PURPOSES ONLY
GROUND/FLIGHT TRANSITION ... ON GROUND PHASE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 163 of 198
FOR TRAINING PURPOSES ONLY
CFDIU FUNCTIONS (3) INTERFACES
MAIN FUNCTIONS MEMORY
CLOCK
The Centralized Fault Display Interface Unit (CFDIU) stores the failure
messages and the Electronic Centralized Aircraft Monitoring (ECAM)
warning messages in a Non Volatile Memory (NVM).
The CFDIU permanently receives the UTC and the date from the aircraft
clock and then sends these two parameters to all type 1 systems. The UTC
and date are used by the system Built-in Test Equipments (BITEs) as well
as the CFDIU for the various maintenance reports.
MANAGEMENT The CFDIU manages failure information and adds data such as
Universal Time Coordinated (UTC), DATE, ATA chapter, LEG, FLIGHT PHASE
to elaborate reports.
FAC
CORRELATION If a computer internal failure is detected, the CFDIU
achieves a correlation function that means it isolates or ignores the
malfunctions of systems relating to this failure. Example: ADC FAILURE
causes NO DATA FROM ADC in other computers. The Centralized Fault
Display System (CFDS) will present only the initial failure in the last
leg report. The function IDENT will then present the systems affected by
this failure.
MONITORING The CFDIU scans permanently all input buses in order to
detect a transmitted failure message. The CFDIU detects intermittent
operation of the systems and adds INTM to the failure message.
DETECTION The CFDIU can detect the nature of the failure by reading the
ARINC words. Nature of failures: - internal (i.e. SDAC FAULT) - external
(i.e. FWC 1: NO DATA FROM ADIRU1) - intermittent; (INTM) added - class
3; (CLASS 3) added.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
The CFDIU receives the flight number and city pair from the Flight
Augmentation Computer (FAC). The city pair (FROM/TO airport) is sent to
the Air Traffic Service Unit (ATSU) and to the Data Management Unit
(DMU)-part of the Flight Data Interface and Management Unit (FDIMU). The
CFDIU counts the number (maximum 8) of identical and consecutive ECAM
warning messages and records in the LAST LEG ECAM REPORT.
FDIMU The CFDIU receives the aircraft identification from the Flight
Data Interface Unit (FDIU)-part of the FDIMU and sends this parameter to
all type 1 systems. The CFDIU is used as an interface between the FDIU
part and the Flight Warning Computer (FWC) to send some FDIU class 2
failures to the FWC in order to constitute the maintenance status. The
CFDIU is used as an interface between the DMU-part of the FDIMU and the
FWC to send some DMU class 2 failures. DMU class 2 failures are used for
the maintenance status on the ECAM.
FWC The CFDIU receives the flight phases and ECAM warnings from the FWC.
The ECAM warnings are used by the CFDIU to generate the LAST or CURRENT
LEG ECAM REPORT. Only PRIMARY
Issue 012 - Revision 000 - Dated 01/07/2023 Page 164 of 198
FOR TRAINING PURPOSES ONLY
failures, INDEPENDENT failures and CLASS 2 failure messages (Maintenance
status) are received.
DMC The CFDIU receives the engine serial number from the Display
Management Computer (DMC) and sends this parameter to the Engine
Vibration Monitoring Unit (EVMU).
ATSU The ATSU receives the city pair from the FAC through the CFDIU. The
CFDIU can send real time failures and ECAM warning messages to the ATSU.
It can also send the Post Flight Report (PFR) to the ATSU at the end of
the flight.
EVMU The EVMU receives the engine serial number from the DMC through the
CFDIU. The DMC receives it from the Engine Control Unit (ECU) for CFM
engines, or Electronic Engine Control (EEC) for IAE and PW engines.
ABNORMAL OPERATION CLOCK BACKUP If the aircraft clock fails, the CFDIU
takes over and its internal clock sends UTC and date on the output bus
to all type 1 systems. Upon power-on after A/C clock failure, the item
GMT/DATE INIT is added to the CFDS menu. This option enables UTC and
date initialization.
CFDIU FAILURE When the CFDIU is affected by an internal failure, the
message CFDIU is displayed on the ECAM MAINTENANCE STATUS page.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 165 of 198
FOR TRAINING PURPOSES ONLY
MAIN FUNCTIONS ... ABNORMAL OPERATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 166 of 198
FOR TRAINING PURPOSES ONLY
This Page Intentionally Left Blank
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 167 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCEDURE WITH CFDS (3) COCKPIT EFFECT After a
malfunction, the crew reports the cockpit effect in the log book. The
fault symptoms, relative to the cockpit effect, can be as follows: - a
WARNING/MALFUNCTION + Centralized Fault Display System (CFDS) FAILURE
message (with possible associated warnings and system IDENTIFIERS). - a
WARNING/MALFUNCTION alone. - a CFDS FAULT message alone.
PFR For the class 1 and 2 failures of CFDS monitored systems, the Post
Flight Report (PFR) permits an access to the concerned list of faults in
Airn@v. For this purpose, it gives the following information:
WARNING/MAINT status messages (if it exists), FAILURE message with its
SOURCE, ATA reference and IDENTIFIERS list. When the PFR print is not
available, this information can be retrieved through the MCDU (in Normal
mode or Menu mode). Service Information Letter (SIL) 00-028, made of
"spurious maintenance messages", and the maintenance knowledge let the
airlines create a specific data base to filter the messages to be
displayed on the PFR. Once loaded into the Centralized Fault Display
Interface Unit (CFDIU), this maintenance filter data base can be
activated through the MCDU.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 168 of 198
FOR TRAINING PURPOSES ONLY
COCKPIT EFFECT & PFR
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 169 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCEDURE WITH CFDS (3) TROUBLE SHOOTING PROCESS AIRN@V
ENTRY The CFDS report information gives a direct access to the fault
isolation procedure task numbers through Airn@v. You have to select the
Troubleshooting documentation to get access to the fault symptoms, which
are the association of a warning/malfunction and/or CFDS fault message.
The fault symptoms are divided into the five following sections: -
ECAM, - Electronic Flight Instrument System (EFIS), - LOCAL warning, -
Crew & Maintenance Observation and, - CFDS.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 170 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCESS - AIRN@V ENTRY
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 171 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCEDURE WITH CFDS (3) TROUBLE SHOOTING PROCESS
(continued) WARNING/MAINT. SELECTION To find the reported problem (ELEC
BCL 1 FAULT in this example), you have to select ECAM Warning and enter
the name of the WARNING/MAINT. STATUS MESSAGES, which appears on the PFR
(or on the ECAM Display Unit). You can also enter the ATA chapter to
have a list of Warnings/malfunctions, and then you select the related
WARNING/MAINT status messages. NOTE: If required, additional
Warnings/malfunctions must be selected.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 172 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCESS - WARNING/MAINT. SELECTION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 173 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCEDURE WITH CFDS (3) TROUBLE SHOOTING PROCESS
(continued) CORRELATION A Warning/malfunction with its correlated CFDS
fault could have several associated fault isolation procedure tasks
according to the systems, which have detected the fault. The PFR gives a
SOURCE item, which must be compared with the SOURCE item of the CFDS
Fault messages list in Airn@v. By selecting the appropriate fault
message, the Airn@v system gives the right access to the fault isolation
procedure.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 174 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCESS - CORRELATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 175 of 198
FOR TRAINING PURPOSES ONLY
TROUBLE SHOOTING PROCEDURE WITH CFDS (3) FAULT ISOLATION PROCEDURE The
related fault isolation procedure task in Airn@v (task number
24-30-00-810-805) has a presentation of possible causes and the fault
confirmation (for example by an operational test, power-up test or
GROUND SCANNING). It also gives the fault isolation procedure including
Line Replaceable Unit (LRU) removal/installation, wiring check, etc....
In addition, the procedure gives access to the useful aircraft
documentation references knowing that all manuals contained in AirN@v
are interconnected by hyperlinks, and all the schematics can be found
and printed easily.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 176 of 198
FOR TRAINING PURPOSES ONLY
FAULT ISOLATION PROCEDURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 177 of 198
FOR TRAINING PURPOSES ONLY
POST FLIGHT REPORT FILTERING FUNCTION (3) PURPOSE The purpose of the
filtering function is to reduce the number of spurious maintenance
messages. So the filtered Post Flight Report (PFR) contains only the
messages needing a maintenance action.
FILTER DATA BASE CUSTOMIZATION AND LOADING Using the feedback data from
the airlines or the data from laboratory or flight tests, Airbus
establishes, keeps up to date and transmits to the airlines a document
called Service Information Letter (SIL) 00-028. SIL 00-028 consists of a
"spurious maintenance messages data base". This is an envelope data
base, including the spurious messages concerning every possible Part
Number (PN) from every vendor. The airline is responsible for
customizing this envelope data base to its fleet configuration using a
compatible personal computer and dedicated software. The customized
maintenance filter data base is first stored on a floppy disk, and then
uploaded into the Centralized Fault Display Interface Unit (CFDIU) by
means of the data loader.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 178 of 198
FOR TRAINING PURPOSES ONLY
PURPOSE & FILTER DATA BASE CUSTOMIZATION AND LOADING
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 179 of 198
FOR TRAINING PURPOSES ONLY
POST FLIGHT REPORT FILTERING FUNCTION (3) FILTER DATA BASE
IDENTIFICATION Each filter is identified by a 15-character data base
number. The data base number is written on the filtered PFR and can be
displayed on the MCDU.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 180 of 198
FOR TRAINING PURPOSES ONLY
FILTER DATA BASE IDENTIFICATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 181 of 198
FOR TRAINING PURPOSES ONLY
POST FLIGHT REPORT FILTERING FUNCTION (3) ACTIVATION The filtered PFR is
activated through the MCDU with the function called PFR FILTER PROGRAM.
When FILTER ACTIVATED is set to NO: The complete PFR can be manually or
automatically printed or sent through the Air Traffic Service Unit
(ATSU). When FILTER ACTIVATED is set to YES: The filtered PFR can be
manually or automatically printed or sent through the ATSU. With the
PRINT FILTER CONTENT function, the maintenance filter data base can be
printed.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 182 of 198
FOR TRAINING PURPOSES ONLY
ACTIVATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 183 of 198
FOR TRAINING PURPOSES ONLY
POST FLIGHT REPORT FILTERING FUNCTION (3) EXAMPLES These examples show a
PFR not filtered, the maintenance filter data base and the PFR filtered.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 184 of 198
FOR TRAINING PURPOSES ONLY
EXAMPLES
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 185 of 198
FOR TRAINING PURPOSES ONLY
PRINTER DESCRIPTION/OPERATION (3) PRINTER CAPABILITY The printer
provides onboard printouts concerning various aircraft systems one at a
time. The printer is capable to print 80, 64 or 40 characters per line
format. It provides a storage capability of 8 Kilobytes (Kb) and is able
to generate 120 forty-character lines per minute.
USERS Data to be printed is formatted within the various system users.
The printer determines which input is active and switches on each system
in order of their priorities.
MANUAL PRINT In manual mode, prints are triggered from the MCDU. The
MCDU initiates printing of data displayed on MCDU screen or data stored
in system reports.
AUTOMATIC PRINT Some reports are automatically printed provided that the
automatic printing function has been programmed in the corresponding
system computer. Example: Automatic printing of the Centralized Fault
Display System (CFDS) POST FLIGHT REPORT upon engine shutdown.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 186 of 198
FOR TRAINING PURPOSES ONLY
PRINTER CAPABILITY ... AUTOMATIC PRINT
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 187 of 198
FOR TRAINING PURPOSES ONLY
PRINTER PAPER LOADING (2) JOB SET-UP Energize the aircraft electrical
circuits. Push the SLEW P/BSW to remove the remaining paper from the
printer.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 188 of 198
FOR TRAINING PURPOSES ONLY
JOB SET-UP
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 189 of 198
FOR TRAINING PURPOSES ONLY
PRINTER PAPER LOADING (2) PROCEDURE Turn the locking system to release
the door. Lift the door and discard the empty roll. Clean the remaining
paper off the paper cutter. Install a new roll of paper on its support
and check that the paper roll turns correctly. Engage the paper under
drive roller and check that paper is held tight. Close and lock the
printer door.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 190 of 198
FOR TRAINING PURPOSES ONLY
PROCEDURE
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 191 of 198
FOR TRAINING PURPOSES ONLY
PRINTER PAPER LOADING (2) CLOSE-UP De-energize the aircraft electrical
circuits. Make sure that work area is clean and clear of tools and other
items. NOTE: Using the SLEW P/B move the paper out of the slot of the
paper cutter and cut off the unwanted paper.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 192 of 198
FOR TRAINING PURPOSES ONLY
CLOSE-UP
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 193 of 198
FOR TRAINING PURPOSES ONLY
COMPUTER REMOVAL AND INSTALLATION (3) Computer removal/installation
Before starting a computer removal/installation procedure, the A/C has
to be set-up for maintenance. The first task is to make sure that the
ground service network is energized and the access door is open and
accessible. Then make sure that the C/Bs listed in the removal of the
computer procedure of Aircraft Maintenance Manual (AMM) is open. The
first action is to loosen the nut and then to lower the nut. When the
nut is lowered, pull the computer on its rack to disconnect the
electrical connectors and remove the computer from its rack. Before
starting a computer installation procedure, clean and do a visual
inspection of the component interface and of the adjacent area. First
remove the blanking caps from the electrical connectors and make sure
that the electrical connectors are clean and in the correct condition.
Then install the computer on its rack and push it on its rack to connect
the electrical connectors. Now you can engage the nuts on the studs and
tighten them. The installation is finished. You can close the C/B. The
last actions of the computer installation are to do a test through the
MCDU and to close the access. Make sure that the work area is clean and
clear of tools and other items, close the access door and remove the
access platform.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 194 of 198
FOR TRAINING PURPOSES ONLY
COMPUTER REMOVAL/INSTALLATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 195 of 198
FOR TRAINING PURPOSES ONLY
PUSHBUTTON REMOVAL AND INSTALLATION (3) Pushbutton removal and
installation Before starting a P/B removal installation procedure, make
sure that the lamp capsule is in the delatched (up) position when you
remove it from an alternate action switch. If the lamp capsule is not
delached (up) when you remove it the switch cannot operate. Then open
the C/B of the circuit related to the P/BSW. Put the removal tool lamp
capsule extractor in the notches on the side of the head of the P/BSW.
Carefully pull the tool to remove the head of the P/BSW. The head stays
attached to the body of the P/BSW by the rods that turn. Now you have to
remove the body of the P/BSW. First, fully loosen the two screws of the
body but do not lock them. After, pull the head to remove the body.
Before starting the installation of a P/BSW, clean and make an
inspection of the component interface and of the adjacent area. Now, put
the TOP mark in the up position and push the body of the P/BSW fully
into its housing. Torque the two screws of the body of the P/BSW. Now,
install the head in the body of the P/BSW. To do this, push the head
until it touches the stop. To finish the installation task close the C/B
of the circuit related to the P/BSW. After that, make sure that the work
area is clean and clear of tools and other items.
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 196 of 198
FOR TRAINING PURPOSES ONLY
PUSHBUTTON REMOVAL AND INSTALLATION
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 197 of 198
FOR TRAINING PURPOSES ONLY
Training Manual Airbus A318/319/ A320/A321 (CFM56 & V2500)
END
Airbus A318/A319/A320/A321 (CFM56 or V2500)
CATTS LTD
Issue 012 - Revision 000 - Dated 01/07/2023 Page 198 of 198
