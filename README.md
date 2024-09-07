# TrueNAS SCALE catalog

This is a fork of the archived TrueCharts App Catalog for TrueNAS SCALE.

Since iX-Systems will deprecate their Kubernets/Helm-based GUI app plattform in Q4 2024, TrueCharts already deprecated their TrueNAS catalog. Thus, you cannot update your already installed applications anymore although there's currently no migration to another Kubernetes plattform available. There will be a migration to their new Kubernetes-based plattform(s).  
But for now, you have to wait.

Therefore I decided to fork their archived chart repository and manually push some updates for applications I personally use. Feel free to use this chart to update your own TrueCharts applications on TrueNAS SCALE.

&nbsp;

### **Be aware that I won't continue pushing updates as soon as there's a stable migration to a new Kubernetes/Helm plattform available!**

### **!!! I am not responsible for any issues that might occur. Always backup your data! !!!**

&nbsp;

- ### How to change your TrueCharts catalog:
    
    1.  Remove your already old/deprecated TrueCharts catalog: *Apps* --> *Discover Apps* --> *Manage Catalogs* --> *TRUECHARTS* --> *Delete* (don't worry, this won't delete any of your already installed applications)
    2.  Add this repository as a new Catalog:
        1.  *Add Catalog* --> *Continue*
            - **Catalog Name:** TrueCharts
            - **Repository:** https://github.com/hey101/truecharts_archive
            - **Preferred Trains:** incubator, premium, stable, system
            - **Branch:** main

Now you should be able to update your applications again.

- ### I made a script that automatically updates all applications based on the manual update method that v3DJG6GL used on his chart. I can't guarantee that something will not break, but it at least works for the apps I use and saves the manual update time. This does not account for using other images instead of the ones truechart uses. I need to add a method for working around this if there are issues. If you have any problems, just create a new issue and I will see what I can do. 


- ### Changelog:
- ### Changelog:
	- 2024.09.07 @ 05:58 PM EST:
		- authentik: v2024.8.0 --> v2024.8.1
		- game-server-watcher: v3.1.17 --> v3.1.18
		- tinymediamanager: v5.0.10 --> v5.0.11
		- watchyourlan: v2.0.1 --> v2.0.2
		- zigbee2mqtt: v1.40.0 --> v1.40.1
