# BigData_Session2_Assignment2
**********
Before starting to work upon HDFS, I started all processess, using start-all.sh command

TASK 3 ------->>>>>>>>>

(i) Create a file max-temp.txt in local FS
Put some 10-15 records of date and temperature example:
dd-mm-yyyy, temperature
Example:
10-01-1990, 10
10-02,1991, 20
Move this file to HDFS at /user/acadgild/hadoop.


SOLUTION FOR TASK 3 ------->>>>>>>>>

Screenshot 1.1 : cat command creates max-temp.txt file inside home directory.

Screenshot 1.2 : It shows max-temp.txt is not present in HDFS.

Screenshot 1.3 : put command copies max-temp.txt file from local FS (i.e. /home/acadgild/) to HDFS (i.e. /user/acadgild/home/).

Screenshot 1.4 : cat command now shows contents of max-temp.txt file present in HDFS are as same as max-temp.txt present in local FS.

***********

TASK 4 ------->>>>>>>>>

(i) Change the permission of the file /user/acadgild/hadoop/max-temp.txt, such that only the owner and the group members have full control over the file. Others do not have any control over it.

SOLUTION FOR TASK 4 ------->>>>>>>>>

Screenshot 2.1 : It first shows owner has read and write permissions, group has read permission only, and others have read persmission only,
So using chmod 770, we are permitting read, write, execute persmissions to owner and group (because 7 means all permission (rwe) and 0 means no permission), and no permission to others.
