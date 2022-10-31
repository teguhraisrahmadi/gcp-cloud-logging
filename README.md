# Google Cloud Platform

## Work Instruction for Using Cloud Logging

1. Before we run cloud logging, we need create VM which will be monitored. 
<br> ![Capture](Material/1.png) <br>

2. Then connect to the vm, and run web server (I am using apache web server). 
   Run this command : “sudo apt-get install apache2”
<br> ![Capture](Material/2.png) <br>

3. Run this command for install agent to the vm :
   “curl -sSO https://dl.google.com/cloudagents/install-monitoring-agent.sh”
<br> ![Capture](Material/3.png) <br>
   
4. “sudo bash install-monitoring-agent.sh”
<br> ![Capture](Material/4.png) <br>

5. Run this command for install cloud log to the vm :
   “curl -sSO https://dl.google.com/cloudagents/install-logging-agent.sh”
   “sudo bash install-logging-agent.sh –structured”
<br> ![Capture](Material/5.png) <br>

6. The go to the Cloud Logging menu. You can see all log from your vm. 
<br> ![Capture](Material/6.png) <br>

7. You can choose name log what you want to see. For this case, I want to see apache error log. Go to this and click.
<br> ![Capture](Material/7.png) <br>

8. This view is apache log detail in cloud logging.
<br> ![Capture](Material/8.png) <br>

9. You can export the log, just click create sink.
<br> ![Capture](Material/9.png) <br>

10. Fill the sink name and description. Then click next.
<br> ![Capture](Material/10.png) <br>

11. Fill the sink destination. You can follow this option. For this option I create new bucket just for this log.
<br> ![Capture](Material/11.png) <br>

12. Fill the bucket detail.
<br> ![Capture](Material/12.png) <br>

13. Set the retention date and create the bucket.
<br> ![Capture](Material/13.png) <br>

14. Click next.
<br> ![Capture](Material/14.png) <br>

15. Let it default. Then next
<br> ![Capture](Material/15.png) <br>

16. Then create sink (number 4 is just optional, you can skip for it).
<br> ![Capture](Material/16.png) <br>

17. The sink has been created. You should waiting for this log. Data should available soon.
<br> ![Capture](Material/17.png) <br>

18. You can see, the bucket still 0 mb.
<br> ![Capture](Material/18.png) <br>

19. Done, Thanks






























