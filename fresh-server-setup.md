# Fresh Server Setup

Here are the steps that can be followed while setting up a new server instance. 

## Setting up new user and SSH

Create new user

```bash
$ sudo adduser aryan
```
Setup superuser permissions for the user:

```bash
$ sudo usermod -aG sudo aryan
```

Generate new SSH keys in your local

```bash
$ ssh-keygen -t ed25519 -C "email.com"
```

Copy the public key and store them in authorised_keys of the instance 

```bash
$ echo "public key" >> ~/.ssh/authorized_keys
```

## Disable SSH on root

## Setup firewall