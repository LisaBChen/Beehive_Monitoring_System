# Code for Beehive Monitoring System Project for EPICS UTD Beehive Project

The code is used to monitor Beehive Activity (including weight, temperature and humidity) for the hives located in the UTD apiaries.

ESP32_Data_Collection_and_Web_Hosting.ino is uploaded into the ESP32's but before that you must select a network and a name for the hive.
At that point ESP32Scraper.py will be used on a machine on the same network to scrape the data from the hive. Inorder to tell it what the hive IP is the Beehive_IP.txt is used for that purpose. From the scraping process a file name {Hive Name}.txt will store all the data. the compressed version of  {Hive Name} Compressed.txt is all the data being compressed at the end of the day. It can be mostly ignored.

MainWebHost.py is the file that is constantly run just as ESP32Scraper.py and its job is to host the webpage to anyone that requests it.

To use this code you must run the weather.py code. You must also have flask
https://flask.palletsprojects.com/en/1.1.x/installation/

A hardware prototype has been built and is in the testing phase as of Fall 2021. 

Questions are to be directed to the Spring/Fall 2021 Beehive Monitoring System team. 
