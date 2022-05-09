Starting from the stack that you can find at the following repository
https://github.com/ansjin/docker-compose-influxdb-v2-grafana
I have added mosquitto and telegraf images to have a full IOT STACK, to collect data from any MQTT client.

The repository is working also on raspberry pi, tested with dietpi os (https://dietpi.com/).

Prerequisites: docker and docker-compose installed on the host.

You can use the MQTTX app https://mqttx.app/ to test the stack simulating differnt clients.
You can send plain text messages like: sensor_name field1=value1, field2=value2.
For example, if you want ot track the gas (mc=cubic meters) consumed by a boiler using a plc sensor you can send a message like: myboiler mc=25