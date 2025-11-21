# Compose File

You'll notice a chirpstack env var called 'MQTT_BROKER_PASSWORD'. Set this to any sensible password. Also create an env var called 'CHIRPSTACK_BROKER_PASSWORD' within the MobiusFlow container, and set this to the same value.

# Configuration Folder

Copy the configuration file in this repository to an external volume. We normally put it inside ./config/chirpstack/
You can see the volume mapping in the compose file. Just make sure this is mapped correctly to the internal containers.

# Container names

Make sure Mosquitto is called 'mosquitto'
Make sure Chirpstack is called 'chirpstack'