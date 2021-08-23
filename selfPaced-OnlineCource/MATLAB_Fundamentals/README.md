# MATLAB Fundamentals

## basic

To delete the variables from the workspace, you can use the clear command .
>> clear

To delete only specific variables, specify those after the clear command.
>> clear var1 var2

If you would like to clear the Command Window, you can use the clc command.

| INCORRECT | CORRECT |
|-----------|---------|
|X-Y        |XY       |
|month&year |monthYear|
|1998value  |value1998|
|CO2  conc  |CO2_conc |

* format long: 소수점 15째자리까지
* format short: 소수점 4째자리까지
* format bank: 소수점 2째자리까지 
* help format
* home > preference > commend window 로 format 변경 가능

You can enter
>> doc fcnName
to get information on any MATLAB function.

## matplot

### basic plot
You can use the hold on and hold off commands to add lines to your current plot.
>> plot(x,y1)
>> hold on
>> plot(x,y2)
>> hold off

If you want to change the color of your plot, you can use an additional input to the plot function to do this. The following command will plot y versus x in magenta.
plot(x,y,"m")

Some other color codes are:
* "b" blue
* "g" green
* "r" red
* "c" cyan
* "k" black

You can also change the line style using an optional argument. The following command will plot y versus x as a dotted line.
plot(x,y,":")

Some other line style codes are:
* "–" solid
* "––" dashed
* "–." dash-dot

By default, individual data points are not marked on the line plot. You can mark individual points by changing the marker style. The following command will create a plot of y versus x where the individual points are marked with circles.
plot(x,y,"o")

Some other marker style codes are:
* "+" plus sign
* "*" asterisk
* "." point

You can combine plot options to specify color, marker style, and line style! Generally, the order doesn't matter, so the following two commands produce the same plot using a red dotted line.
* plot(x,y,"r:")
* plot(x,y,":r")

### labels

Labels can be added to plots using plot annotation functions, such as xlabel. The input to these functions must be text, which can be enclosed in quotation marks.
>> xlabel("Text Label for X-Axis")
