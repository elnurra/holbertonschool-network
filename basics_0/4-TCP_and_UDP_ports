#!/bin/bash

# Display listening TCP ports
echo "Active Internet connections (only servers)"
echo "Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name"
sudo netstat -tuln | awk '$1 == "tcp" && $NF != "0.0.0.0:*" && $NF != ":::*" {print}'

# Display listening UDP ports
echo "Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name"
sudo netstat -uln | awk '$1 == "udp" && $NF != "0.0.0.0:*" && $NF != ":::*" {print}'

