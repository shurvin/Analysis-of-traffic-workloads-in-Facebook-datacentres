## Analysis-of-traffic-workloads-in-Facebook-datacentres
svc_ms=1 #average disk I/0 service time,ms 
util_min=0 #range to plot 
util_max=100
ms_min=0 
ms_max=10
#Plot mean response time vs utilization(M/D/1)
x=c(util_min:util_max)
plot(svc_ms*(2-x/100)/(2*(1-x/100)), type="l",lty=1,lwd=1, xlim=c(util_min,util_max), ylim=c(ms_min,ms_max), xlab="Utilization %", ylab="Mean Response Time (ms)")
![image](https://user-images.githubusercontent.com/93541679/150361971-a64fc4ff-030f-48d0-b4d4-54430ad00cc1.png)
