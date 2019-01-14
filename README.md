# rsh-UDP
### Tools for receiving and interacting with Raspberry Shake UDP data
*written by @ivor and @iannesbitt*

the files in this repo:

1) raspberryShake.py
    library of shake-related functions, to be used in a parent python program wanting to process data off a UDP port

2) rs2obspy.py
    example library that uses raspberryShake.py to process UDP data to obspy stream object with channel-specific traces. can be iterated.

3) shake-UDP-packetLoss.py
    program that will report UDP data packet loss between a shake and a receiving computer 
    to be run on receiving computer

4) shake-UDP-local.py
    program to read data off UDP port, to be run on shake computer directly

5) shake-UDP-remote.py
    program to read data off UDP port, to be run on a computer not the shake

6) obspy_example.py
    program to read UDP data to an ObsPy stream continuously, then plot it when the user presses CTRL+C

7) live_example.py
    reads UDP data and continuously updates a plot, can be used from the command line. run `python live_example.py -h or --help` for details.

TO DO

1) finish library / add any other base functions of interest
	- library has been updated to work with current use cases

2) convert pgm 2 to completely use raspberryShake library

3) add an example program using obsPy library
	- done and working

4) document library

5) document packetLoss program as example of how to use library

6) flesh out the -local and -remote program templates, to use new library, etc.
	- done
    