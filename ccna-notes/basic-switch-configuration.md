# Basic Switch Configuration

## Objective
Learn how to perform basic configuration on a network switch.

---

## Set Device Name

Configure a hostname to easily identify the switch on the network.

```
enable
configure terminal
hostname Switch-1
```

---

## Configure Password on Console Management Port

This secures access to the switch through the console port.  
Users must enter a password before accessing **User EXEC mode**.

```
line console 0
password password_here
login
```

---

## Secure Privileged EXEC Mode

To protect **Privileged EXEC mode**, configure an encrypted password using the `enable secret` command.

```
enable secret your_password_here
```

This ensures that only authorized users can access administrative commands.

---
## Secure Virtual Terminal Lines(vty) Remote access to the switch
To be able to access the switch remotely using ssh, we need to secure this channel of communication<br>
with a password

## Example of Basic Initial Configuration

Below is a simple example combining some basic switch configuration commands.

```
enable
configure terminal

hostname S1

line console 0
password cisco
login

enable secret class
```

---

## Summary

In this configuration we:

- Set the switch hostname
- Secured console access with a password
- Protected privileged EXEC mode with an enable secret
