# ooby Dashboard

Self hosted dashboard for monitoring the uptime & performance of a DigitalOcean Linux VPS.

The target server hosts an Xray/VLESS VPN service and a couple React websites.

## Project status

Planning and initial setup. No application features are implemented yet.

## Goals

- Build a custom dashboard from the ground up using React and TypeScript.
- Develop a Python API using FastAPI.
- Collect Linux host metrics with Node Exporter and Prometheus.
- Display current performance, historical trends, and monitoring availability.
- Package the application with Docker Compose.
- Add automated tests and continuous integration.

## Planned first release

- CPU, memory, disk, network, and uptime metrics.
- Overview and detail views for one VPS.
- Historical performance charts.
- Basic threshold alerts.
- Documented local setup and deployment.

## Planned architecture

React dashboard → FastAPI → Prometheus → Node Exporter

Prometheus periodically collects metrics from Node Exporter. FastAPI queries Prometheus and provides data to the React dashboard.

## Development approach

Build incrementally, starting locally before connecting the existing VPS. Each milestone should produce working functionality, tests where appropriate, and documentation explaining the decisions.

## Future extensions

- ~~Website availability checks~~.
- Xray service health.
- ~~Authentication and protected management actions~~.
- Support for additional servers?.
