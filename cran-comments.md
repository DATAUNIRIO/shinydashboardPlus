## Test environments
* local OS X install, R 3.4.4
* ubuntu 14.04 (on travis-ci), R 3.5.0 (2017-01-27)
* Windows (via devtools::build_win(), R-devel)

[![Build Status](https://travis-ci.org/DivadNojnarg/shinydashboardPlus.svg?branch=master)](https://travis-ci.org/DivadNojnarg/shinydashboardPlus)

## R CMD check results
There were no ERRORs or WARNINGs. 

There was 1 NOTE:

*checking Rd line widths ... NOTE
 Rd file 'productList.Rd':
  \examples lines wider than 100 characters:
               src = "https://image.darty.com/hifi_video/televiseurs-led/grand_ecran_led/samsung_ue55mu9005_4k_uhd_s1703224306074A_140323143 ... [TRUNCATED]

 Rd file 'userList.Rd':
  \examples lines wider than 100 characters:
               src = "https://d33wubrfki0l68.cloudfront.net/071952491ec4a6a532a3f70ecfa2507af4d341f9/c167c/images/hex-dplyr.png", 

 Rd file 'widgetUserBox.Rd':
  \examples lines wider than 100 characters:
           backgroundUrl = "https://images.pexels.com/photos/531880/pexels-photo-531880.jpeg?auto=compress&cs=tinysrgb&h=350",

These lines will be truncated in the PDF manual.


## Re-submission:

I corrected all notes adressed in the previous build:

- the examples lines are now all lower than 100 characters (in productList.Rd, userList.Rd and widgetUserBox.Rd)
- the title field in description is now in title case

There is a FALSE positive here, nothing is mis-spelled:

Possibly mis-spelled words in DESCRIPTION:
  adminLTE (3:17, 10:41)
  shinydashboard (3:41, 10:21)
