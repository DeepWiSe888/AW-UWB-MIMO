##### Quick Start 


1. Install the antenna. One antenna has a "V" and the other has an "H", both of which have direction indication. As shown in the picture:  

   <img src=".\天线安装示意图.jpg" alt="天线安装示意图" style="zoom:25%;" />


2. After the antenna is installed, connect TX and RX with SMA. Note that the lines of TX and RX should be the same length when connecting, so as to ensure that the signal transmission delay of each group of TX and RX is the same. As shown in the picture:
   <img src=".\天线接线示意图.jpg" alt="天线接线示意图" style="zoom:25%;" />


3. The radar and the laptop computer are connected by network cable, and the IP address of the wired NIC is modified as required.



4. Run "tools\mimo-udp.exe",you can see the radar initialization and collected frame rate and other relevant information.

5. Run "labs\plot_datas\receiving_data_and_save.py" and store the data locally.
   
6. Run "labs\plot_datas\plot_data_from_file.py",you can parse the data.
Dimensions of data: frame_cnt * tx_cnt * rx_cnt * bin_cnt


##### Test

1. Modify SEC = 20 of "labs\plot_datas\libs\conf.py" to increase the window and make it easier to observe data.

2. The tester moves in front of the radar, from near to far, and from far to close. As shown in the figure, the track of human activities can be seen after the background is removed. The data quality of each group of transceiver antennas can be observed by cyclic enumeration of Tx and Rx.

   <img src=".\运动图.jpg" alt="运动图" style="zoom:80%;" />

3. Sit still in a fixed position. On the timeline, you can see basically evenly spaced bright spots, which represent breathing

   <img src=".\静息图.jpg" alt="静息图" style="zoom:80%;" />

4. Support to calculate the horizontal Angle and elevation Angle of the target.