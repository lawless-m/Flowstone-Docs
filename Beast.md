## Beast

This is the bare metal hardware containing an NVidia 3090 with 24Gb VRAM. 

A server-class machine with a single Haswell Xeon, 64 GB ECC RAM, and a software RAID 5 array across four SSDs.   

Issued IP 192.168.102.74 

[[Wireguard]] endpoint 10.99.0.3

Here's the hardware summary:                                                                                                                                                                                                                                          

CPU                                                                                                                                
- Intel Xeon E5-2660 v3 @ 2.60 GHz                                                                                                 
- 10 cores / 20 threads (Haswell-EP)
                                                                                                                                     
Memory                                                                                                                             
- 64 GB RAM (no swap configured)                                                                                                                                                                                                                                      

Storage
  - 4x SSDs (~112–119 GB each) in a RAID 5 array via 

Linux md                                                                        
- Usable RAID volume: ~334 GB, 221 GB used, 90 GB free                                                                           


Chipset                                                                                                                            
- Intel C610/X99 series (Wellsburg) — server/workstation platform
                                                                                                                                     
