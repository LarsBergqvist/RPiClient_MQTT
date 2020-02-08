# RPiClient_MQTT
A Python script for publishing Raspberry Pi cpu-usage, cpu-temperature, memory-usage and disk usage via MQTT. Schedule it with cron to get measurements at regular intervals.

For example, in crontab, specify to execute the script every ten minutes. This will generate messages with MQTT topics on the form HOME/[MACHINENAME]/[METRICNAME] (e.g. HOME/MYPI/DiskUsagePercent):
```
*/10 * * * * /home/myuser/mypath/systemmonitor.py MYPI
```
