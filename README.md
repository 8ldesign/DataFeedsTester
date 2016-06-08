# DataFeedsTester

## Overview
This is targeted to test any data feed file having urls - for the validity of the URLs. 

##Features
1. It can test multiple datafeed files - with filenames that comply to the patterns in FileConstants.py
2. The tester can pick up any file name from any location - under the "DataFeedsTester" folder structure

## Pre-requisites
1. Replace the http:// with https:// in the files - in order to avoid the 301 redirect outputs.
  1.1 Replace can be done using 'vi' editor - :%s/http:/https:/g
2. Place the files in folder in or below DataFeedsTester for the tester program to pick it up
3. Make sure you have the necessary packages - requests, re, os, logging, fnmatch in your python site packages- using pip install.
4. The current code is compatible for both python 2.7 and 3+ versions. If you're using a python version less than 3, replace the  
   #! /usr/bin/env python3 line with #! /usr/bin/env python
   
## Steps to do
1. Execute the 'feedTester' in the src folder with python
    Ex: python feedTester


## Known Bugs
1. The current tester doesn't eliminate duplicates in few of the top level feeds

## Scope of improvements
1. This program can be made to run and send an email with 5x errors and 4x errors as a list
