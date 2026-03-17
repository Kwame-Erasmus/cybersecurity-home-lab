# Basic Switch Configuration

## Objective
Learn how to perform basic configuration on a network switch.

## Device name
hostname switch-1
***

## Configure password on console management line/port
put password on the console management port

After this, connection to the console management port will require password to enter the user EXEC mode

- console line 0

- password password

- login
  ***
  ## Secure privilege EXEC mode with password
  - enable secret password


- Enter global configuration mode

configure terminal / config t

- hostname

hostname S1

- Secure console access

line console 0
password cisco
login
