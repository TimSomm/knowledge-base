# MoleculerJs 
---

Moleculer js is a microservices framework for Node.js
[Documentation](https://moleculer.services/docs/0.14/)

## Installation

```bash
npm i moleculer --save
```

```bash
npm i moleculer-cli -g
```

## Create new project

```bash
moleculer init project your-project-name
```

## Core concepts

| Name | Function |
| :----- | :---------|
| [Service](https://moleculer.services/docs/0.14/services.html) | Simple JavaScript module, isolated and self contained |
| Node | OS Process running locally or externally, hosting one or more services |
| Local Services | Two (or more) service running on the same node, no latency, and no transporter|
| Remote Services | Services distributed across nodes, transporter is needed for communication |
| [Service Broker](https://moleculer.services/docs/0.14/broker.html) | Responsible for the management and communication between services |
| [Transporter](https://moleculer.services/docs/0.14/networking.html) | Communication bus, services use it to transfer events, requests and responses |
