# python-projects-for-beginners
Alarm Clock with GUI

1. First, we import all the necessary libraries and modules:

Explanation:
Tkinter module belongs to a standard library of GUI in Python. It helps us to create a dialog box with any information that we want to provide or get from the users.
Datetime and time modules in python help us to work with the dates and time of the current day when the user is operating python and to manipulate it too.
Winsound module provides access to the basic sound playing machinery provided by Windows platforms. This is useful to generate the sound immediately when a 
function is called.


2. Create a while loop:

Explanation:
Define a function named as alarm() which takes the argument of (set_alarm_timer).It contains a while loop with a Boolean function True which makes the program 
automatic to work.
time.sleep(1) halts the execution of the further commands given until we get the time value from the user later in the code and returns the background thread of the 
clock time going on at a regular interval.
Get the current time using current_time which takes the argument of datetime.datetime.now().
now is used to print the time and date is used to print the current date by string conversion using strftime().
Define another function here named actual_time() which takes in the user value for setting the alarm in the string format. The same argument of (set_alarm_timer) as 
alarm before to execute the while loop which we further use while making GUI.
If loop suggests that if the user input time set_alarm_timer matches with the while loop ongoing time now, the message is printed as” Time to Wake up”.
winsound.SND_ASYNC plays the system generated sound as soon the condition satisfies, acting as a reminder for the alarm clock.


3. Creating GUI using tkinter:

Explanation:
To Initialize tkinter, we pass a command under the name clock as Tk().
The dialog box has the title as DataFlair Alarm Clock with a geometry of (400*200). We pass on the heading to mention the time format for 24 hours using time_format.
The second heading is given above the user input boxes for the labeling to be “Hour Min Sec” using addTime.
Just to make the dialog box look funkier, adding another label as “when to wake you up” using setYourAlarm.
As we have already converted the current time in the string before (actual time), the variables we initialize for the user input dialog boxes are in StringVar().
Finally make the input boxes such as hourTime, minTime, and secTime which takes the entry of the time the user wants to set the alarm on in 24-hour format.
Submit takes the command of the defined function actual_time and executes the clock as it acts as a set button to start the program.
Clock.mainloop() is the basic and the last command was given to compile all the previous commands with their basic settings of color, font, width, axis, etc. and 
displays the window as soon as the program is run.

Summary
With this project in Python, we have successfully made the Alarm Clock. We used the popular GUI library for rendering graphics on a display window. 
We learned how to extract the current time from the computer and to use it for manipulation using the DateTime library. This way we can set an alarm in the 
computer interface using python programming which rings with the default machine sound for Windows.

