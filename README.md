# nmap-bash

Custom nmap command condensed into concise BASH script.


#!/bin/bash 

#This script will run a productive nmap scan against a target IP 
#It initiates service enumeration, syn scan, timing, and OS detection  

echo "Enter the target IP : " 
read TargetIP 

nmap -p1-65535 -sV -T4 -A $TargetIP -oG BestnmapScan

cat BestnmapScan

./bnmap.sh
