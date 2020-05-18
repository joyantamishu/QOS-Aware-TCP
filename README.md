# qos_aware_tcp
All convnesional TCP congestion variants like RENO, WestWood, DCTCP all have certain limitation that makes it hard to 
achive some of the required objective in Data center environment,i.e. no packet drop, differtiated service, etc. This work presents our attempt 
to overcome these limitations. This kernel patch presents one kernel module called "qtcp", which tries to address the problem.
