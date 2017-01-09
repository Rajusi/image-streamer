---------------------------------------------			
About
---------------------------------------------
This repo contains HPE Image Streamer plan scripts and artifact bundles to personalize SLES 12 Operating System
to deploy it on HPE Synergy compute modules

	
Contents of the repo are:
	
	artifact-bundles : contains artifact bundles in zip format. User can import these into Image Streamer
	plan-scripts     : list of scripts to personalize the OS

---------------------------------------------			
Pre-requisites
---------------------------------------------
	
	Access to Synergy platform
	Synergy composer configured with OS Deployment server 'Image Streamer'
	Access to SLES 12 Golden image

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
			
	SLES-12-mount-and-validate
	SLES-12-configure-users
	SLES-12-configure-multiple-NICs
	SLES-12-configure-hostname
	SLES-12-manage-services
	SLES-12-configure-partition-using-LVM
	SLES-12-unmount
			
Above plan scripts cover use cases like

	Network configuration 
	Configure multiple NICs
	Host name and alias configuration
	changing root password
	Adding new users
	Configure LVM
	enabling/disabling services
			
-----------------------------------------------
Summary
-----------------------------------------------
These plan scripts have been tested for personalizing SLES 12
