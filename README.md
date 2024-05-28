# Whoami Helm Chart

## Description

This is a Helm chart for the Whoami application. Whoami is a simple application that displays information about the pod it's deployed in.

## Prerequisites

- Kubernetes 1.12+
- Helm 3.0+

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
helm install my-release ./whoami

A `README.md` file for a Helm chart typically includes the following sections:

1. **Chart Name**: The name of the chart.
2. **Description**: A brief description of what the chart does.
3. **Prerequisites**: Any prerequisites required for installing the chart.
4. **Installing the Chart**: Instructions for how to install the chart.
5. **Uninstalling the Chart**: Instructions for how to uninstall the chart.
6. **Configuration**: A table listing the configurable parameters of the chart and their default values.

Here's an example based on your `Chart.yaml`:

```markdown
# Whoami Helm Chart

## Description

This is a Helm chart for the Whoami application. Whoami is a simple application that displays information about the pod it's deployed in.

## Prerequisites

- Kubernetes 1.12+
- Helm 3.0+

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
helm install my-release ./whoami
```

## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```bash
helm delete my-release
```

## Configuration

The following table lists the configurable parameters of the Whoami chart and their default values.

| Parameter | Description | Default |
| --------- | ----------- | ------- |
| `image.repository` | Whoami image repository | `traefik/whoami` |
| `image.tag` | Whoami image tag | `latest` |
| `image.pullPolicy` | Whoami image pull policy | `IfNotPresent` |
| `service.type` | Kubernetes Service type | `ClusterIP` |
| `service.port` | Kubernetes Service port | `80` |
```

Please replace the values in the table with the actual configurable parameters and their default values from your `values.yaml` file.