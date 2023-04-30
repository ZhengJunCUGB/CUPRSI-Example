This is the case when the input is a single binary file.
You can run the program using the following command:

1. si <in.bin ns=30001 ntr=201 dt=4000 ns_win=5000 outns=1001 StartFldr=1 EndFldr=201 Device=0 threads=256 blocks=128 file_mode=0 RAMSizeMB=20000 VRAMSizeMB=2000 Stack_flag=1 >out.su

2. si <in.bin >out.su par=si.par

The file "si.par" includes all the parameters in 1

Parameters:
 ns=                number of points of input traces 
 ntr=               number of input traces 
 dt=                sample interval; in micro-seconds 
 ns_win=            number of points of time windows in correlation 
 outns=             number of points in output traces 
 StartFldr=         start number of original field record number 
 EndFldr=           end number of original field record number 
 Stack_flag=        0 Not stack 
                    1 Stack causal and noncausal part 
 Device=            Device number 
 threads=           number of threads 
 blocks=            number of blocks 
 RAMSizeMB=         RAM size (MB) 
 VRAMSizeMB=        VRAM size (MB)
 file_mode=         0 A binary file 
                    1 A file list of binary files 
