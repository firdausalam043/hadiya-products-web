#!/bin/bash
#system_info.sh - Display basic information

echo "==================================="
echo " SYSTEM INFORMATION (RHEL 8)"
echo "==================================="

#Hostname and OS
echo "Hostname            : $(hostname)"
echo "OS Version          : $(cat /etc/redhat-release)"
echo "Kernel Version      : $(uname -r)"

# Uptime
echo "Uptime              : $(uptime -p)"

#CPU & memory
echo "CPU Info            : $(lscpu | grep 'Model name' | awk -F: '{print $2}')"
echo "CPU Cores           : $(nproc)"
echo "Total Memory        : $(free -h | grep Mem | awk '{print $2}')"

#Disk Usage
echo "Disk Usage          :"
df -h