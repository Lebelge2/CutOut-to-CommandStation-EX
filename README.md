# CutOut-to-CommandStation-EX
CutOut to CommandStation-EX for RailCom

For this example the Pins are numbered

Main IN1: 12   
     IN2: 14
Prog IN1: 33
     IN2: 27

#define STANDARD_MOTOR_SHIELD F("STANDARD_MOTOR_SHIELD"),    \     
  new MotorDriver(13, 12, 14, UNUSED_PIN, 25, 4.88, 2000, UNUSED_PIN), \
  new MotorDriver(32, 33, 27, UNUSED_PIN, 36, 0.80, 2500, UNUSED_PIN)


In the DCCRMT.h file declare:
   void StarTimerCutOutMain();             
   void StarTimerCutOutProg();             
