# Countdown Clock

This script emulates a big red digital clock with each digit being 
represented by 7 LED segments using HTML and the Canvas element.

# TO DO 

* Organize how segmenets are turned on and off 
* Store digits as array of activated segments
* CSS for look
* Display a specific digit in a specific place 
* Step forward every 1 second
 * Handle rollovers to new hour etc

# Scratchpad

Questions/thoughts:
------

* What about implementing a 'flicker' effect?
* Post-apocalyptic design

* What is the format of the input time? 
Maximum time can be be 99 Hours 99 minutes 99 seconds


displayTime(string time);
displayTime(int hours, int minutes, int seconds)
displayTime(array(hours, ninutes, seconds))

differentiate between empty

e.g. displayTime("10:45:20"); 
e.g. displayTime(10, 45, 20); 

Time has to be converted into segments 

Place 0-5 and Integer 0-9 + empty

"10:45:20"
place   integer
0       1
1       0
2       4
3       5
4       2
5       0


Store an array of on segmenets for each integer 0-9 + empty
e.g. 
empty = []
0 = [1, 2, 3, 5, 6, 7] 
...
9 = [...]

.--. 
|  |
'--'
|  |
'--'

Segment class
-----
constructor params: 
    int place (0-5)
    int position (0-7)
    int state (0,1)

<div class="clock">
    <span class="digit">
        <span class="segment" data-value="0"></span>
        <span class="segment" data-value="1"></span>
        <span class="segment" data-value="0"></span>
        <span class="segment" data-value="0"></span>
        <span class="segment" data-value="1"></span>
        <span class="segment" data-value="1"></span>
        <span class="segment" data-value="1"></span>
    </span>
    <span class="digit">
        <span class="segment" data-value="0"></span>
        <span class="segment" data-value="1"></span>
        <span class="segment" data-value="0"></span>
        <span class="segment" data-value="0"></span>
        <span class="segment" data-value="1"></span>
        <span class="segment" data-value="1"></span>
        <span class="segment" data-value="1"></span>
    </span>
    <span class="divider">
    ...
</div>
         

