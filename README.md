# AppDynamics Azure Monitor with Ansible

This repository is intended to provide a way to install the Azure Monitor extension on a new VM using Ansible, very easily.


## Getting Started

1. Copy `ansible/inventory.ini.dist` to `ansible/inventory.ini`, and set variables for your target machines.
2. Copy `ansible/variables.json.dist` to `ansible/variables.json`, and set variables for your azure instance and configuration specifics.
3. Run `bin/ap`, and watch the playbook run!

## Information

- The AppDynamics Machine Agent is installed and configured in systemd as `appdynamics-machine-agent`.
- You can edit the `AzureMonitor/config.yml.j2` file to your liking, including the necessary services and format.

## Metrics Bench

- TBD

## Links

- [Azure Monitoring Extension](https://www.appdynamics.com/community/exchange/extension/azure-monitoring-extension/)
- [Azure Monitor - Metrics Supported](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/metrics-supported)
