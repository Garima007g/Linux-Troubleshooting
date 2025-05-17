# Linux-Troubleshooting

1. Fixed alarm for disk space issue.
   Received a system generated alarm for /disk usage is above threshold limit. First we connected with server with sudo 
   access and checked the current status of particular disk for which we got an alarm.

   df -h /disk_name // to find the details of disk size usage and available space
   du -h /disk_name // to check detailed usagae of disk to find which folder is taking more memory under this disk. And 
   accordingly we will check what excatly happning in this disk and will take action accordingly

2. Fixed alarm for memory and CPU utilization.
   Received a system generated alarm for memory usage or CPU usage of server is above threshold limit. First we connected        with server with sudo access and checked the current status of server memory.

   free -mh // will get the details of memory. How much memory allocated to this server and How much memory in used and 
   available and will get the swap memory details as well.

   If the available memory and CPU utilization is looking good than we will wait for sometime and monitor the usage. If we       find we don't have enough available memory and CPU utilization and may lead to server hang or rebbot. Which can do the        service impact.
   
   top command will provide the details of which process talking more memory or CPU utilization and will restart that process    to become normal usages. Sometimes we need to take confirmation from DEV team if we can do the restart of that service or     not. We will capture all the insights of issue and will share with DEV team for further analysis to avoid the similar         issue in future.
    

   
