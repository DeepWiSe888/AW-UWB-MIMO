# AW-UWB-MIMO

1. Folder Notes:
   1. /doc/:Related documentation.
   2. /labs/:Related read data and parse data demo.
      1. "receiving_data_and_save.py",receives and save data from "mimo-udp.exe".
      2. "plot_data_from_file.py",parse data which "receiving_data_and_save.py" save.
   3. /tools/:"mimo-udp.exe",receives data from the FPGA and forwards the data.
2. Using Notes:
   1. Set up the antenna and wire it.
   2. Connect the device to the computer with an Ethernet cable.
   3. Change the Ethernet IP address of the computer to 192.168.0.3
   4. Run the executable program "mimo-udp.exe",then run the python code "receiving_data_and_save.py",and you will see the data save to /datas/.
   5. Run the python code "receiving_data_and_save.py" to parse data.
3. QA:
   1. The FPGA default FPS is 2042-2043.
   2.  Number of antennas the default value is 8 Tx and 8 Rx.
   3. The antennas are switched from Tx 1 to Tx 8,Rx 1 to Rx 8.
   4. So,on the premise of 8 Tx and 8 Rx,the fps is 2042 / 8 / 8.