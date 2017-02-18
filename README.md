# Session3-Assign2
Create a file with the name max-temp.txt in the local file system and add
10-15 records with two columns for date and temperature and save it as
max-temp.txt
Example: dd-mm-yyyy, temperature
10-01-1990, 10
10-02-1991, 20

- touch max-temp.txt
- vim max-temp.txt

● Copy the above max-temp.txt file from the local file system to HDFS in the
/user/acadgild/hadoop path.

-hadoop fs -put max-temp.txt /user/acadgild/hadoop

● Change the permission of the file /user/acadgild/hadoop/max-temp.txt,
such that only the owner and the group members should have the r-w-x
permissions. Others should have only read the permission on the above file.

-hadoop fs -ls /user/acadgild/t1.txt
-hadoop fs -chown 660 /user/acadgild/t1.txt     /changing permission for owner

-hadoop fs -chgrp 660 /user/acadgild/t1.txt    // changing permission for group


