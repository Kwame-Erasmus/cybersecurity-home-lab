# Basic Switch Configuration

## Objective
Learn how to perform basic configuration on a network switch.

## Device name
hostname switch-1
***

## Configure passwords
put password on the console management port
console line 0
password password
login


- Enter global configuration mode

configure terminal / config t

- hostname

hostname S1

- Secure console access

line console 0
password cisco
login
