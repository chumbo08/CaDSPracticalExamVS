# VS Practical Exam 1    
(c) 2015 by CaDS Haw Hamburg 

## Info
Includes the files to start with the VS practical exam part 1 @HAW Hamburg Powered by Cads    
   
Contact: Martin.Beche@haw-hmaburg.de   
Visit: http://cads.informatik.haw-hamburg.de   

## Create Basic setup

In this project Eclipse is used with the leJOS Eclipse Plugin.
Please follow the steps described here: http://sourceforge.net/p/lejos/wiki/Installing%20the%20Eclipse%20plugin/

### Download and extract leJOS

Download leJOS EV3 (For the initial Setup, 0.9.1 beta was used)   
Link: http://sourceforge.net/projects/ev3.lejos.p/files/   
Extract leJOS_EV3_X.X.X-YYYY.tar.gz as leJOS
(used in the example scripts) to your root development directory   

### Clone Repo
  
Call git clone https://github.com/Transport-Protocol/CaDSPracticalExamVS to create local repo.  

### Implementation hints
In the source folder JUNIT test can be find as implementation hints.

### Compare to existing solution
For test the student can call a nameservice, consumer and provider
#### Call nameservice
java -cp CaDSRMIProvider.jar:leJOS_EV3_0.9.0-beta/lib/ev3/ev3classes.jar  org.cads.ev3.rmi.CaDSNameServer -h localhost -ID console-I -S true
#### Call provider
java -cp CaDSRMIProvider.jar:leJOS_EV3_9.0-beta/lib/ev3/ev3classes.jar  org.cads.ev3.rmi.CaDSRMIProvider -h localhost -ID console-I -S true
#### Call consumer
java -cp CaDSRMIProvider.jar:leJOS_EV3_0.9.0-beta/lib/ev3/ev3classes.jar    org.cads.ev3.rmi.CaDSRMIConsumer -h localhost -ID console-I -S true
