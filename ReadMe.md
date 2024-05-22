# Ansible role to install Eclipse Mosquitto MQTT Broker

Install Mosquitto MQTT broker onto host with TLS enabled on port 8883
via self signed certificate

# Variables

see `defaults\main.yaml`

* `hostname` - defaults to builtin inventory_hostname
* `mqtt_anonymous` - allow broker access without username/password (defaults false)
* `mqtt_user` - the mosquitto auth username used by clients to talk to broker
* `mqtt_password` - the mosquitto auto password used by clients - defaults to letmein <- override this
* `mqtt_enable_tcp` - allow insecure tcp mqtt on port 1883(e.g. for legacy devices)
* `mqtt_enable_tls` - allow secure tls connection on port 8883
* `cert_dir` - certificate directory where ca and server certs are stored
* `key_dir` - key directory where server private key is stored
* `docker_dir` - docker dir
* `docker_compose_dir` - docker compose dir