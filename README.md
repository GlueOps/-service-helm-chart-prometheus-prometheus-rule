# prometheus-prometheusrule

![Version: 0.1.0-alpha1](https://img.shields.io/badge/Version-0.1.0--alpha1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.16.0](https://img.shields.io/badge/AppVersion-1.16.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| description | string | `"This is the default alert description. Please change this to be more useful."` | Description of the alert. Make this informative to the responding team(s) know what this alert is for. |
| duration | string | `"10m"` | Amount of time for the PromQL expression to be true before an alert gets fired. |
| expr | string | `"vector(0)"` | PromQL Expression |
| labels.component | string | `"nil"` | Name of component. Ex. backend, frontend, authentication, database, search. |
| labels.team | string | `"nil"` | Team name that will react to any alerts |
