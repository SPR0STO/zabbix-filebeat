# Filebeat Zabbix Template 

Zabbix plugin for basic monitoring a "filebeat" daemon. 

## Features: 

 Alert with a trigger when: 

   - "filebeat" daemon is not active; 
   - "filebeat" version is changed; 
   - no data about "filebeat" daemon status or version. 

## Requirements 

- Linux OS on a filebeat node with zabbix agent installed; 
- Zabbix-server v.3.4. or greater.

## Installation 

This only needs to be setup on the filebeat node and zabbix-server. 

### Zabbix Agent 

Copy [filebeat.conf](./agent/filebeat.conf) to conf.d or add UserParameter to 
your agent config. 

### Zabbix Frontend 

Import the [filebeat.xml](./template/filebeat.xml) template (supports 
zabbix v.3.4 and greater). 
Add node to the newly imported template. 

## Important note 

This is a very little and basic plugin. I just wanted to share this if you also 
need a handy and simple plugin to check some filebeat info. 

## License 

This plugin is published under **GNU General Public License v3.0**. Feel free to
use and modify this as you need. 

Copyright (©) [pr0sto](https://github.com/pr0sto), 2018 
