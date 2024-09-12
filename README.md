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
	- 2024.09.12 @ 10:08 AM EST:
		- autobrr: v1.45.0 --> v1.46.0
		- fluidd: v1.30.3 --> v1.30.4
		- plex: v1.40.5.8921 --> v1.41.0.8992
		- qbitrr: v4.9.2 --> v4.9.3
		- satisfactory: v1.7.4 --> v1.8.1
	- 2024.09.11 @ 09:23 PM EST:
		- unifi: v8.4.59 --> v8.4.62
	- 2024.09.11 @ 04:18 PM EST:
		- ipfs: v0.29.0 --> v0.30.0
		- ispy-agent-dvr: v5.7.5.0 --> v5.7.6.0
		- komga: v1.12.1 --> v1.13.0
		- metube: v2024.8.22 --> v2024.9.11
		- n8n: v1.58.1 --> v1.59.0
		- satisfactory: v1.7.3 --> v1.7.4
		- wordpress: v6.6.1 --> v6.6.2
	- 2024.09.11 @ 01:57 AM EST:
		- docuseal: v1.5.6 --> v1.7.1
		- ghostfolio: v2.106.0 --> v2.107.0
		- grafana: v11.0.0 --> v11.2.0
		- linkding: v1.31.1 --> v1.32.0
		- metabase: v0.50.24 --> v0.50.25
		- pingvin-share: v0.24.1 --> v1.0.4
		- prometheus: v2.52.0 --> v2.54.1
		- satisfactory: v1.7.1 --> v1.7.3
		- scrypted: v0.118.0 --> v0.119.0
		- semaphore: v2.9.75 --> v2.19.10
		- slskd: v0.20.1 --> v0.21.3
		- snapshot-controller: v7.0.1 --> v8.0.1
		- teslamate: v1.29.1 --> v1.30.1
		- vaultwarden: v1.30.5 --> v1.32.0
		- victoriametrics: v1.99.0 --> v1.103.0
	- 2024.09.10 @ 07:17 PM EST:
		- audiobookshelf: v2.13.3 --> v2.13.4
		- cloudflared: v2024.8.3 --> v2024.9.1
		- cops: v2.8.1 --> v3.1.2
		- docker: v27.2.0 --> v27.2.1
		- homepage: v0.9.6 --> v0.9.9
		- jenkins: v2.475.0 --> v2.476.0
		- minio: v2024.08.29 --> v2024.09.09
		- netdata: v1.47.0 --> v1.47.1
		- portainer: v2.21.0 --> v2.21.1
		- redisinsight: v2.54.0 --> v2.56.0
		- satisfactory: v1.6.2 --> v1.7.1
		- solr: v9.6.1 --> v9.7.0
	- 2024.09.09 @ 05:53 PM EST:
		- alist: v3.36.0 --> v3.37.1
		- authentik: v2024.8.0 --> v2024.8.1
		- game-server-watcher: v3.1.17 --> v3.1.18
		- ghostfolio: v2.105.0 --> v2.106.0
		- healthchecks: v3.6.20240904 --> v3.6.20240909
		- ispy-agent-dvr: v5.7.4.0 --> v5.7.5.0
		- jellyfin: v10.9.10 --> v10.9.11
		- maintainerr: v2.1.0 --> v2.1.1
		- memcached: v1.6.30 --> v1.6.31
		- meshcentral: v1.1.27 --> v1.1.29
		- ollama: v0.3.9 --> v0.3.10
		- paperless-ngx: v2.11.6 --> v2.12.0
		- plextraktsync: v0.31.12 --> v0.31.13
		- prowlarr: v1.23.1.4708 --> v1.24.0.4721
		- scrypted: v0.117.3 --> v0.118.0
		- tinymediamanager: v5.0.10 --> v5.0.11
		- watchyourlan: v2.0.1 --> v2.0.2
		- whisparr: v3.0.0.607 --> v3.0.0.610
		- zigbee2mqtt: v1.40.0 --> v1.40.1
	- 2024.09.08:
   		- Updated all apps to match truecharts versions. You can check the commmits for the full list
