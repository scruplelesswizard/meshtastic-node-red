# meshtastic-node-red
Node-RED Configuration for Meshtastic Packets

## Features
- Ingestion from MQTT
- Protobufs decoding
- Message deduplication by ID
- Translating integer To/From node ids to hex
- Annotating packets with known NodeInfo
- Split for all current port numbers
- Writing Packet, Device, Environment and Position measurements to InfluxDB
- Debug nodes for all outputs

## Dependencies
The following Node-RED modules need to be added to the palette before importing the workflow:
- [@meshtastic/node-red-contrib-meshtastic](https://flows.nodered.org/node/@meshtastic/node-red-contrib-meshtastic)
- [node-red-contrib-influxdb](https://flows.nodered.org/node/node-red-contrib-influxdb)

## Flow Preview
![meshtastic-flow](./meshtastic-flow.png)

## Known Limitations
- NeighbourInfo payloads are not correctly decoded
