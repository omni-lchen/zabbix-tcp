# Zabbix-TCP

TCP socket states and connection stats are collected by ss and netstat commands, then sent by zabbix sender.

**Installation**

1. Import the TCP stats template to zabbix and link it to the zabbix host.
2. Copy the TCP stats script to the host in /usr/local/bin .
3. Copy TCP stats zabbix agent configuration to /etc/zabbix-agent/zabbix_agentd.d and restart zabbix agent.

Note: The script may take longer to run on a busy server, increase the timeout limit "timeout=" on zabbix agent configuration "/etc/zabbix/zabbix_agentd.conf" will allow the script to finish.
