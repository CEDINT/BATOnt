# BATOnt
Ontology for Building Automation Technology, an IoT-centric ontology.

BATOnt is created based on the analysis of different existing ontologies, the demand of IoT industry and the requirements of hardware manufactures, software architects, application developers and data scientists. 

The vocabulary provided by BATOnt is for describing not only the Things, but also the related concepts that could be involved in an IoT project implementation, which are about people, spaces, control and authorization. In general, BATOnt can be interpreted from four main perspectives:
* Things perspective, with a focus on which communication protocol is selected, how the devices are deployed and how the Things sense and actuate.
* Control perspective, with a focus on how to control the Things through applications and how to coordinate the collaboration among different Things.
* Spatial perspective, with a focus on where the Things are placed, either in the sense of geographical location or of architectural construction.
* User perspective, with a focus on the interaction of Things with human beings, i.e. who can access and control the Things and what are the characteristics of these people. 

To facilitate the exchange and synchronization of information about the functionality, status and semantic data of Things among users, devices and applications, a concept "Parameter"is used as a core concept in BATOnt. "Parameter" is defined as "an object which wraps a
physical magnitude and the information about its presentation, available actions, access type and permissions". Parameter is used to describe the functional behaviour of devices, i.e. Things. From the point of view of functionality, the functional behaviour of Things can be classified into two kinds, sensor or actuator. By using parameter to represent it, the sensor and actuator can be regarded equally:
* A sensor is interpreted as a non-modifiable parameter. Accordingly, "read a sensor" is performed by query the value of a parameter.
* An actuator is interpreted as a modifiable parameter. Accordingly, "actuate an actuator" is performed by "modify the value of a parameter".

A device can be interpreted as a set of parameters, i.e. "access and control a device" is performed by "read and/or modify the values of a set of parameters". In this way, the integration of new type of devices can be performed by interpreting their functional behaviour as parameters. Furthermore, this mechanism allows to compare the same function of different devices regardless the technologies used.

In addition, the parameter includes the humanreadable information for the understanding of users.In this way, the parameters work as intermediate objects to wrap both of the machine-readable and human-readable information.
