#!/bin/bash

###############################################################
#  AUTEUR:   Xavier
#
#  DESCRIPTION: Top 10 process cpu
###############################################################

# premier cas sans mise en forme
echo "En mode verbeux..."
ps aux | sort -nrk 3,3 | head -n 10

echo ""
echo ""

# avec mise en forme
echo "En mode avec mise en forme"
ps -eo pcpu,pid,user,args --no-headers | \
sort -t. -nk1,2 -k4,4 -r | \
head -n 10 | \
awk '{print "\t"$1"\t"$2"\t"$3"\t    "$4" "$5}'

-------------------------------

# ps -eo rss,vsz,pid,cmd,cputime | sort -n | tail -X

X : pour le nombre 
