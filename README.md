## bareos_exporter
[![Go Report Card](https://goreportcard.com/badge/github.com/dreyau/bareos_exporter)](https://goreportcard.com/report/github.com/dreyau/bareos_exporter)

[Prometheus](https://github.com/prometheus) exporter for [bareos](https://github.com/bareos) data recovery system


### Metrics

- Total amout of bytes and files saved
- Latest executed job metrics (level, errors, execution time, bytes and files saved)
- Latest full job (level = F) metrics
- Amount of scheduled jobs

### Flags

Name    | Description                                                                                 | Default
--------|---------------------------------------------------------------------------------------------|----------------------
port    | Bareos exporter port                                                                        | 9625
endpoint| Bareos exporter endpoint.                                                                   | "/metrics"
u       | Username used to access Bareos PostgreSQL Database                                               | "root"
p       | Path to file containing your PostgreSQL password. Written inside a file to prevent from leaking. | "./auth"
h       | PostgreSQL instance hostname.                                                                    | "127.0.0.1"
P       | PostgreSQL instance port.                                                                        | "3306"
db      | PostgreSQL database name.                                                                        | "bareos"
