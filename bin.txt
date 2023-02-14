#!/bin/bash


for run in {1..10}
do
	date +“%H:%M:%S”
	ps -ef | tail -n+2 | wc -l
sleep 1

done

cat /proc/cpuinfo > /opt/47_48_evening_b/kseniya_egorova/proc

cat /etc/os-release | awk '{print substr($1,7,6)}' | grep Amazon > /opt/47_48_evening_b/kseniya_egorova/os

for file in {50..100}
do
	touch $file.txt
done
