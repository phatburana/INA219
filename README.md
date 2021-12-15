# Introduction
This repository is created to support the power consumption test, measuring load power consumption through Arduino's serial plotter using INA219 module.

# Wiring Diagram
The INA219 is a High Side DC Current Sensor, in order to measure the load's consumption profile, the module is connected to the high side of the component that powers the load.


![image](https://user-images.githubusercontent.com/58856852/146151011-2de5da26-1b45-400e-8d67-ec35aedebe55.png)

# The code
## INA219
INA219 supports various measurements read out including; Shunt voltage, Load voltage, Load current, Load power. This example will only measure the load power.


![image](https://user-images.githubusercontent.com/58856852/146155417-fd419ad0-cfc3-4df7-b2e7-9593f4489d87.png)

## Serial plotter

![image](https://user-images.githubusercontent.com/58856852/146159296-e70497f0-516a-4298-a107-4fa3c5b775fc.png)


Serial plotter is a tool in Arduino IDE which plot the printed serial value into a graphic data, several things should be noted;
* X axis represents the number of data point.
* Y axis will auto scale to the highest and lowest data value. Fixating the axis range by printing out the upper and lower value along with the measured value.
* Serial plotter only allows 500 values maximum to be displayed within the plot. Any more then the oldest value will be discarded first (FIFO).
* Label the plotted value by printing the "Label_name:" before the labeled value (Label_name = your label name).

# Run
After uploading the code into your Arduino, simply open the serial plotter similar to the serial monitor.


![image](https://user-images.githubusercontent.com/58856852/146154740-952799bb-416d-4b6c-9d95-b9e77b963913.png)

![TXzoom](https://user-images.githubusercontent.com/58856852/146160094-3688e76b-b367-43b0-aa99-03601b97debd.jpg)
