Car Black Box 

The concept of Black Box is mainly heard by us in case of Aero-planes. Upon a catastrophe the Black Box is used to analyze the root cause of the issue. However, the purpose of Black Box can go beyond catastrophe analysis. Also known as an event data recorder (EDR) or Accident data recorder (ADR) the Black Box can be installed in some automobiles to record various events. These events which are electronically sensed can often pro-actively detect any issue in the vehicle (ex: Engine fault) or monitor the fleet (ex: Drive over speeding), thereby doing pro-active maintenance of the Automotive vehicle.
By considering today’s busy life, every one wants to reach the destination as soon as possible by ignoring the rules and regulations. By implementing a Black Box which would log critical activities on the car and take appropriate actions in case of rash driving. As mentioned above the root cause of the negligence in the driving would be meeting the daily schedule and go off duty, or to earn extra money by illegal trips etc… So by implementing the mentioned solution it would be easy to keep track of how the vehicle is being used, handled and control the efficiency of the vehicle.
The proposed solution is to log all the critical events like the gear shifts with current speed, the engine temperature, fuel consumption per trip, trip distance etc., The system should allow a password based access to the transport managers to view or download the log to PC if required. Here is a video which gives a working idea about this solution.
As an extension of this idea, the data can be exported continuously to a Cloud based server where a centralized monitoring can be done. This means the black box implementation is extendible as a IoT based solution as well. The goal of this project is to implement a Black Box using the given Micro-controller (PIC in our case) and simulate various events by interfacing the Micro Controllers with sensors etc.

Requirement:

1.Default Screen:
  When the system is in Operation Mode, it would act like a dashboard which 
  would show the current time, speed of vehicle and the latest occurred event.

2.Login Screen:
   1.On press of the UP or DOWN (User Keys) keys the system should prompt for 
     password
   2.The password would be the combination of 4 presses (User Keys).
     Each press should be denoted a “*” symbol
   3.Every wrong entry would, re prompt for password (Max 3 times for every 15 
     minutes)
   4.Incomplete key press (pause of 3 seconds) would lead to Default Screen

3.Main Menu:
  1.The main menu should contain 2 option
     View Log
     Set Time
  2.The UP / DOWN keys are used to navigate
  3.A long press of UP Key should enter the selected menu
  4.A long press of DOWN Key should log out
  5.Idle screen for more than 5 secs should log out  

4.View Log:
  1.Should display all the events captured with log index starting from 0, like
    “EVENT NUMBER” “EVENT SIGNATURE” “EVENT TIME” “SPEED AT THE EVENT”
  2.The UP and DOWN key will be used to scroll the entries
  3.Rollover on reaching the max log entries
  4.The system should be live (capture events occurred) even while viewing the 
    log
  5.A long press of UP Key should take you back to main menu 

5.Set Time:
  1.Should show the current time. The Secs field should blink indicating the 
    field to be changed
  2.The UP key should be used to increment the time. Rollover on reaching max
  3.The DOWN key will be used to choose the field.
  4.A long press of UP Key should take you back to main menu  

 6.Event Capture
   1.Required events have to be captured and stored in the memory
   2.Every event should have a format as
     “EVENT SIGNATURE” “EVENT TIME” “SPEED AT THE EVENT”
   3.memory
   4.The events should be captured real time, no matter which mode you are in  



