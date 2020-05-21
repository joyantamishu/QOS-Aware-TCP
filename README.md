# qos_aware_tcp
All convensional TCP congestion variants like RENO, WestWood, DCTCP etc have certain limitations that make it hard to 
achive some of the required objective in data center environment, i.e. no packet drop, differentiated service, etc during the congestion episode. This work presents our attempt to overcome these limitations. This kernel patch contains one kernel module called "qtcp", which tries to address the above mentioned problems. This readme documentation was made obscure intentionally, as this is a ongoing work and long way to go.

To activate:

1)Restore the patch file

2)In the termianl type

*sudo modprobe tcp_qtcp*

*sudo sysctl -w net.ipv4.tcp_congestion_control=qtcp*

*sudo sysctl -w net.ipv4.tcp_ecn_fallback=0*

*sudo sysctl -w net.ipv4.tcp_ecn=1*

3)To verify whether qtcp has been activated type

*cat /proc/sys/net/ipv4/tcp_congestion_control*

4)Run the source code provided in **tutorial** folder.

