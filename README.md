# Brain-attention-reading-using-brainsense-interfaced-with-MATLAB
This MATLAB code allows reading attention values from the Mindwave Mobile EEG device using the Thinkgear SDK. It establishes a connection, reads attention data packets, and plots the values in a real-time graph. The code requires the Mindwave Mobile device, Thinkgear SDK, and MATLAB. Connect the device, install the SDK, and modify the COM port number if needed. The code continuously reads and displays attention values, updating the graph every second. It provides flexibility for customization and analysis. Remember to refer to the Thinkgear SDK and Mindwave Mobile documentation. Use this code to explore EEG data, analyze attention patterns, and gain cognitive insights. 
This MATLAB code allows you to read the attention values from the Mindwave Mobile EEG device using the Thinkgear SDK. The code connects to the device, reads attention data packets, and plots the attention values in a graph.

**Prerequisites**
MATLAB installed on your computer
Mindwave Mobile EEG device
Thinkgear SDK
**Setup**
Connect your Mindwave Mobile EEG device to your computer.
Install the Thinkgear SDK and make sure the Thinkgear.dll file is available.
Place the provided MATLAB code in a MATLAB script file (e.g., read_attention.m).
Usage
Open MATLAB and navigate to the directory where you saved the MATLAB script.
Modify the portnum1 variable to specify the COM port number to which your Mindwave Mobile device is connected.
Save the changes to the MATLAB script.
Run the MATLAB script by typing read_attention in the MATLAB command window.
**Description**
The code begins by clearing the MATLAB workspace, closing any open figures, and preallocating a buffer for storing attention data.
It sets the COM port number and establishes a connection with the Mindwave Mobile device.
The code reads the attention values from the Thinkgear packets in a loop. It checks if a packet was successfully read and if the attention value is valid.
If a valid attention value is obtained, it is stored in the data_att array and displayed in the MATLAB command window.
The code also plots the attention values in real-time using the plot function and updates the graph every second.
The loop continues until 20 valid attention values are obtained.
Finally, the code releases the connection with the Mindwave Mobile device and displays a completion message.
**Additional Notes**
Make sure to have the Thinkgear SDK properly installed and the Thinkgear.dll file available in the MATLAB search path.
You may need to modify the COM port number (portnum1) based on your specific setup.
This code assumes that the attention value corresponds to the data type with an ID of 2 (TG_DATA_ATTENTION). Modify the TG_DATA_ATTENTION value if necessary.
You can adjust the loop termination condition (i < 20) to collect a different number of attention values.
The attention values are plotted in real-time, allowing you to visualize the changes in attention over time.

