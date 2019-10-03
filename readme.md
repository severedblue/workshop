# Workshop Portfolio

This portfolio describes work that I've done in Python and GoLang as portfolio items for my Curriculum Vitae.  For my current day job I develop in a specific python framework for a monitoring system.  The framework itself is 90% python with 10-30% vendor specific scaffolding depending on the type of monitoring application or automation written.  While the intellectual property developed there is the property of my employer and unique to that monitoring system, this portfolio is a display of my capability as a technical developer.  


### Prerequisites

To run this code, you will have to have Oracle Virtualbox, Vagrant and the vagrant box, hashicorp/precise64 installed on your machine.  This code is meant to be a demonstration of test-driven development for both Python and Go.  

```
vagrant up
```

Note that the initial "vagrant up" will include updating the base ubuntu OS for hashicorp/precise64, then downloading go and python3.6


## A love-hate relationship with Linux

I recall starting on Linux and Unix and how difficult the initial learning curve was.  I use my primary desktop rig for gaming so am used to running Windows 10 and Steam games.  I haven't dipped my toe in running a native linux-boot setup.  Instead I run Linux virtual machines using Oracle VirtualBox and Vagrant.  This is to allow me to use capabilities I am familiar with such as cron jobs and, with a bent to running **infrastructure as code** so that I can rebuild a vagrant instance anywhere with my code base.  It does take a while to download, deploy and update, but theoretically as long as Oracle VB, Vagrant and hashicorp/precise64 is there, cloning my repo and simply typing "vagrant up" will bring my codebase online.  

Initially I wanted to run ansible but installing ansible on a Windows Machine using the Windows 10 Ubuntu subsystem is a challenging ask.  This is the surface of my love/hate relationship with linux in that the well-worn paths make sense, but sometimes striking out and getting something to work with a cut-and-paste from stack overflow means it could be for multiple versions of linux that may not line up, and the chance of failure is high.  That's why it's important to maintain cheat sheets of the most common commands I use for programs like git and vagrant.  In addition, Vagrant itself has some challenges like installing ssh keys for vagrant ssh, and the outdated hashicorp/precise64 box being the only one with virtual editions installed.  Trying to get virtual editions installed onto a box to allow shared folders (to complete the "stored as code" cycle) without guest editions or the vagrant toolkit was its own little nightmare.  That's why trying to get coding languages like "ruby on rails" working on hashicorp/precise64 is its own challenge.  

The way to learn with Linux is to work through these problems and learn something about how it all fits together.  That being said, if time after my day job is finite then every minute I spend debugging linux virtual machines is time I could have spent writing better code in Go and Python.  Hence I have chosen the latter as a demonstration, while using Vagrant as a vehicle to provide a linux development box for development.  

