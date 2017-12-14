Encrypt!
===================


Hey! I wrote a project for encrypting a text into bitmap file that human eye cannot recognize that. this program using a cool algorithm that showed below. 

![over view](https://github.com/gsoosk/Encrypt-Bitmap/raw/master/1.png)
----------
## Note: ##
it was one of my first project in c++ and I didn't use classes and object oriented at all! 

it has not make file eighter and it just including one file.


----------

## Algorithm ##
**encrypting :** 
1. read bitmap
2. seperate picture into 8*8 squares and calculate variance of any RGB colors
3. get message from user
4. get key from user and make a random string using that key belong seed 
5. for every square :

6. choose one square using random seed
7. change LSB of pixel that choosed
8. repeat 5 until message ends

![enter image description here](https://github.com/gsoosk/Encrypt-Bitmap/raw/master/2.png)
and save bitmap


**decrypting :**
1. read bitmap
2. seperate picture into 8*8 squares and calculate variance of any RGB colors
3. get key from user and make a random string using that key belong seed 
4. . for every square :

5. choose one square using random seed
6. read LSB and adding to string 
7. repeat 4 until seeing \n

and save message into disk.


-----------

How to use?
-------------


#### <i class="icon-pencil"></i> Input and Output

first line encrypt
second line bitmap file name
third line is your key
forth line Is your message

> encrypt
> image.bmp
> 2132
> I like pizza !

first line decrypt for decrypting
second line bitmap file name
third line is your key

>decrypt
>coded-image.bmp
>21211

***Note :*** bitmap should be in program repository.