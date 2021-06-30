# k8s-webui
Contains for the webui for running docker cluster from browser with simple English instructions.
For video demonstration visit this [link](https://www.linkedin.com/posts/bhardwaj-rahul_summerinternship2021-arth-docker-activity-6816061470271389696-fE69)

## Prerequisites
* This repository uses a pre-setup kubernetes cluster which can be accessed through the system on which the apache webserver is running.
* In the provided video I have used minikube to show the demonstration.
* Give required powers to the apache user and do the settings to by pass SELinux.

## How to use the repo
* Install apache webserver on your computer.
* Have a kubernetes cluster ready with you with the config file in cgi-bin.
* Copy all the files of html in /var/www/htlm and cgi-bin file in /var/www/cgi-bin.
* Change the IPs that has been used in the code with your system's IP.

## About the pages
* Front.html is the main home page for the current repository which works with front.css for css part and uses two images from the html folder. This page is the link to both docker web portal and kubernetes web portal.
* docker.html file works with back.py in cgi-bin folder to give the docker web-portal. 
* k8s.html file is the focus of this repository and provides the kubernetes web portal for the project. The k8s.html works with k8s.css for the animations and k8s.py file in cgi-bin folder.
* k8s.py file is the main backbone of the project which makes the instruction provided to be converted into actual kubernetes commands.
* k8s.html file is linked with k8shelp.html file which provides the instructions to how to enter commands in the portal. This file works with k8shelp.css for graphics.
