---------------------------------------------			
About
---------------------------------------------
This repo contains HPE Image Streamer plan scripts and artifact bundles to personalize RHEL 7.2 Operating System
to deploy it on HPE Synergy compute modules

	
Contents of the repo are:
	
	artifact-bundles : contains artifact bundles in zip format. User can import these into Image Streamer
	plan-scripts     : list of scripts to personalize the OS

---------------------------------------------			
Pre-requisites
---------------------------------------------
	
	Access to Synergy platform
	Synergy composer configured with OS Deployment server 'Image Streamer'
	Access to RHEL 7.2 Golden image

-------------------------------------------
Key Inputs
--------------------------------------------
	Interface name to be configured
	Device name mounted on to / ( root system )

---------------------------------------------			
How to use
---------------------------------------------
Option 1: Import artifact bundles as is

	Step1 : Import the artifact bundles into Image streamer and extract
	Step2 : Add golden image to deployment plan
	Step3 : Create the server profile using the deployment plan in OneView and provide attribute required values
	
Option 2: Leverage plan scripts and customize it as per user need

Following are the plans scripts. Depending the use case, use the appropiate plan scripts.
			
	RHEL-7.2-mount-and-validate
	RHEL-7.2-configure-users
	RHEL-7.2-configure-multiple-NICs
	RHEL-7.2-configure-multiple-NIC-teaming
	RHEL-7.2-configure-hostname
	RHEL-7.2-manage-services
	RHEL-7.2-configure-partition-using-LVM
	RHEL-7.2-register-rhel
	RHEL-7.2-unmount
			
Above plan scripts cover use cases like

	Network configuration 
	Configure multiple NICs
	Configure-NIC with NIC teamings
	Host name and alias configuration
	changing root password
	Adding new users
	Configure LVM
	registering OS with Redhat Satellite server
	enabling/disabling services
			
-----------------------------------------------
Summary
-----------------------------------------------
These plan scripts have been tested for personalizing RHEL 7.2
