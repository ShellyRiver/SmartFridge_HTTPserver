# SmartFridge_HTTPserver
CS 598 Smart X Final Project

### Introduction:
An HTTP server that is supposed to be run on Raspberry Pi inside the fridge. It simply sends the information of all the items in the fridge whenever it receives a get request. The post method can be implemented in the future to manipulate the items from the APP.

Supports 6 types of items: apple, banana, orange, tomato, broccoli, green pepper.

Other items are not recognizable by our model and do not have corresponding pictures in the APP.
### Explanation of data:
- type: type of item
- in_time: the date that the item is put inside the fridge
- expire_dates: the total number of days that the item would expire
- level: the level of shelf the item is located inside the fridge
- status: 
    + 1: food is fresh
    + 0: food is going bad
    + -1: food is expired
    

### How to run:

1. Replace the variable IP_address with ip address of the Raspberry Pi (whatever the sever is). 
    - To get the ip address of the server, run the command ifconfig in Raspberry Pi or other other Unix-like operating systems, run ipconfig on windows. 
2. Replace the sever ip address in android app with the same ip address
3. If the port number is occupied, change to other port number. The port number here and the port number in the app has to be the same. 

### Example APP result:
![2c6facfdd4adb659c819de5978e1797](https://user-images.githubusercontent.com/109195884/207746378-dd05480e-1a26-4123-883f-30c6025ac50f.jpg)
