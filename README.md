# battery-soldering-iron-controller
Design of a servo controller built to move battery packs and control electronics in an unmanned airframe to compensate for longitudinal trim. The system is based on a PIC32MX470 microcontroller. The controller controls the DC motors to move the carriage inside the airframe. The controller is capable of driving two motors in parallel. The position of the system is determined by data read from a magnetic encoder. Positon is regulated by PID algorith with consists of an inner loop (regulation of the current flowing through the motors) and an outer loop (position controller). The motors are current-controlled, so control is by torque. The most important systems are duplicated to make the aircraft immune to catastrophe caused by system failure.  Communication with the controller takes place via the CAN bus. In order to test the controller, a smaller-scale test rig was developed, which is a copy of the system from the airframe. The PCB design was created in Altium Designer 21, the software was written in C language using the MPLABX IDE. 

<img src="working.gif" width="800">
<img src="test_stand.PNG" width="800">
<img src="hardware\pcb_3d_model.PNG" width="800">
<img src="hardware\top_and_bottom_layer.png" width="800">
<img src="hardware\pcb_assembled_2.png" width="800">


