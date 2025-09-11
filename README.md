# gcp-info-metrics

> PS: These metrics have been manually created on 3rd of June 2025 and I do not guarantee they are up to date or otherwise free of errors. Use at your own risk.

This repository contains some static Prometheus-formatted metrics for various Google Cloud Platform (GCP) metrics, such as Persistent Disk performance numbers.

If you have Prometheus Operator (or something similar, like VictoriaMetrics Operator) you can deploy a prefilled ScrapeConfig directly like this (replace `my-namespace`):

    kubectl apply --namespace my-namespace -f https://raw.githubusercontent.com/signicat/gcp-info-metrics/refs/heads/main/scrapeconfig.yaml

And metrics should start flowing!

The metrics available are all listed (surprise, surprise) in https://github.com/signicat/gcp-info-metrics/blob/main/metrics_gcp_info_pd.txt .
