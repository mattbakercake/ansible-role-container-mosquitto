# Ansible role to install Eclipse Mosquitto MQTT Broker

Install Mosquitto MQTT broker onto host with TLS enabled on port 8883
via self signed certificate

# Variables

see `defaults\main.yaml`

`hostname` - defaults to builtin inventory_hostname
`mqtt_user` - the mosquitto auth username used by clients to talk to broker
`mqtt_password` - the mosquitto auto password used by clients - defaults to letmein <- override this
`docker_dir` - docker dir
`docker_compose_dir` - docker compose dir