# qos_aware_tcp
All convnesional TCP congestion variants like RENO, WestWood, DCTCP all have certain limitation that makes it hard to 
achive some of the required objective in data center environment,i.e. no packet drop, differtiated service, etc during the congestion episode. This work presents our attempt to overcome these limitations. This kernel patch presents one kernel module called "qtcp", which tries to address the above mentioned problem. This readme documentation was made obscure intentionally, as this is a ongoing work and long way to go.

