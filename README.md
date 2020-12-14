# [ANONYMOUS BOX](https://tryhackme.com/room/anonymous)

(Replace with your own)
IP = 10.10.223.23

## Detailed Report in the ![report.pdf](report.pdf) file

##### You can use the linpeas.sh to find the weaknesses instead, just upload it on the victim machine using wget or curl and run it
#### If you want to be more creative you can upgrade to a meterpreter shell to make it easier.


## Update
#### If we actually use exif on the images we can get some interesting data

```
exif puppos.jpeg

EXIF tags in 'puppos.jpeg' ('Intel' byte order):
--------------------+----------------------------------------------------------
Tag                 |Value
--------------------+----------------------------------------------------------
Image Width         |5616
Image Length        |3744
Bits per Sample     |8, 8, 8
Photometric Interpre|RGB
Image Description   |Three Pembroke Welsh Corgis side by side outdoors. Approve
Manufacturer        |Canon
Model               |Canon EOS 5D Mark II
Orientation         |Top-left
Samples per Pixel   |3
X-Resolution        |300.0000
Y-Resolution        |300.0000
Resolution Unit     |Inch
Software            |Adobe Photoshop CC 2018 (Macintosh)
Date and Time       |2019:02:18 12:24:51
Artist              |Photographer: Tatyana Panova
Corrupt data
The data provided does not follow the specification.
ExifEntry: The tag 'YCbCrSubSampling' contains an invalid number of components (1, expected 2).
```

##### This could contain some password or hint to a password for the ssh server, or could be completely missleading. I leave that up to you to figure out!

## QUESTION 1
#### Enumerate the machine. How many ports are open?
4

## QUESTION 2
#### What service is running on port 21?
ftp

## QUESTION 3
#### What service is running on ports 139 and 445?
smb

## Question 4
#### There's a share on the user's computer. What's it called?
pics

## Question 5 & 6
#### User's and root's flag will not be disclosed in this write-up
