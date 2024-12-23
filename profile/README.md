# Ben Strobel Master Thesis
This is the GitHub organisation containing all repositories for my masters thesis. Its purpose is to provide a single entry point for accessing all code and documentation that was created as part of my thesis.

The thesis is available as a [pdf](https://cdn.benstrobel.de/master-thesis/thesis.pdf)

## Thesis Abstract

Cell Broadcast is a system that many countries use to warn their citizens of severe threats like environmental disasters or nuclear attacks. It uses cell towers to broadcast messages to devices in their range. However, these cell towers can be affected by the same disasters they are supposed to warn about. This can lead to regions in the disaster area where no emergency broadcasts can be received and where people could, therefore, be unaware of the warning or information provided by the broadcast. <br>
This thesis proposes the "Emercast" system to augment Cell Broadcast. The system establishes an opportunistic network between end-user devices by forwarding emergency broadcasts via peer-to-peer connections. We present and discuss a prototype implementation and demonstrate that the proposed system can significantly improve broadcast dissemination within the affected area. We simulate emergency scenarios and evaluate how Emercast acts to spread emergency broadcasts to the devices in affected areas. The thesis aims to serve as a baseline for a discussion about implementing such a system in major smartphone operating systems. Furthermore, the thesis highlights additional topics of research that could be instrumental to adequately assess the viability of such a system.

## Repositories

### [Android Application](https://github.com/ben-strobel-master-thesis/emercast-android)
Installed on end user devices. Is notified by backend when new emergency notifications have been dispatched. Spreads emergency notifications to other instances of the Android Application via a Bluetooth Low Energy peer to peer exchange.

### [Backend](https://github.com/ben-strobel-master-thesis/emercast-backend)
The central component that allows authorities to manage other authorities and create emergency notifications

### [Frontend](https://github.com/ben-strobel-master-thesis/emercast-webinterface)
Provides a user interface for the backend. Primary entry point for authorities.

### [Api Specification](https://github.com/ben-strobel-master-thesis/emercast-api)
Specifies the REST interface for the backend and the protobuf definitions used for serialization. Is used for generating server stubs in the backend, api connectors in the frontend and api connectors and serializers in the Android Application.

### [Simulator](https://github.com/ben-strobel-master-thesis/emercast-simulator)
Simulates the behavior of the Emercast system in a city center emergency scenario.

### [Script Utils](https://github.com/ben-strobel-master-thesis/script-utils)
Contains scripts for running batch simulations with a variety of parameters and for analyzing the logs and creating graphs out of them.

### [Bluetooth Low Energy Analysis Instructions](https://github.com/ben-strobel-master-thesis/emercast-ble-sniffer-analysis)
Contains documentation how to sniff/intercept the BLE communication of the Android Application for analysis.
