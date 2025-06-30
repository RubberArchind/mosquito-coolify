# Mosquitto MQTT Broker for Coolify

This repository contains the configuration for deploying Mosquitto MQTT broker on Coolify at **mosquito.wwa.gr**.

## Quick Start

1. Fork this repository
2. Connect to Coolify
3. Deploy as Docker Compose service
4. Configure domain as `mosquito.wwa.gr`

## Connection Information

- **MQTT Endpoint**: `mqtt://mosquito.wwa.gr:1883`
- **WebSocket Endpoint**: `ws://mosquito.wwa.gr:9001`

## For Milesight Devices

Configure your Milesight people counting device with:

- **Host**: `mosquito.wwa.gr`
- **Port**: `1883`
- **Protocol**: MQTT

## Testing

```bash
# Subscribe to test topic
mosquitto_sub -h mosquito.wwa.gr -t test/topic -v

# Publish test message
mosquitto_pub -h mosquito.wwa.gr -t test/topic -m "Hello from mosquito.wwa.gr"
```
