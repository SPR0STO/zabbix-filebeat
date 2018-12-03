# Filebeat Zabbix Template

Basic filebeat monitoring plugin for zabbix

## Features:

- Check filebeat version; 
- Check filebeat service status; 
- Check if filebeat service is not active on the machine and alert with a trigger; 

## Requirements

- Linux OS on a filebeat node with zabbix agent installed.

## Installation

This only needs to be setup on the filebeat node.

### Zabbix Agent

Copy filebeat.conf to conf.d or add UserParameter to your agent config.

### Zabbix Frontend

Import the filebeat.xml template (supports zabbix 3.4 and greater).
Add node to the newly imported template.

## Important note

This is a very little and basic plugin I wrote to monitor my resources. I just 
wanted to share this if you also need a handy and simple plugin to check some 
filebeat info.

## License

This plugin is published under GNU General Public License v3.0. Feel free to use 
and modify this as you need.

Copyright (©) [pr0sto](https://github.com/pr0sto), 2018
