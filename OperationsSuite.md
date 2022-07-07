# Operations Suite

### Cloud Logging
- Cetralized location for logs
  - Application Logs
  - GKE Custom Logs

### Cloud Monitoring
- Overall Health of application/ Infrastructure
  - CPU
  - Memory
  - Health
- Set SLOs and Alerts

### Cloud Trace
- *Open Telemetry* *Open Census*
- Netowork latency 
- API performance
- Distributed system

### Cloud Profiler
- Source code level performance diagnostics
- A function takes up this amount of Memory/CPU

### Cloud Debugger
- Identify Errors in a running application
- **Does not require restarting system**
  - Logpoints
    - Inject log statements into applications
  - Snapshots
    - View the call stack and analyze local variables

### Managed Prometheus
- Google managed version of Prometheus for GKE
  - Promethus is metrics for Kubernetes
- Highly Scalable

### Audit Logs
- Logs about editing resources in Google Cloud

```mermaid

    flowchart LR

        CloudLogging[Cloud Logging]
        CloudTrace[Cloud Trace]
        CloudProfiler[Cloud Profiler]
        CloudDebugger[Cloud Debugger]
        CloudMonitoring[Cloud Monitoring]
        MyApps[My Apps]
        GoogleServices[Google Services]
        CloudStorage[Cloud Storage]
        BigQuery[Big Query]
        PubSub[Pub/Sub]
        AuditLogs[Audit Logs]

          
        MyApps --- CloudProfiler ---> p([Source Code Perfomance])
        MyApps --- CloudDebugger ---> e([Running App debugging])
        MyApps --- CloudTrace ---> n([Network Latency Diagnostic])
        MyApps --- CloudMonitoring ---> m([Health Checks Machine Metrics])    

        GoogleServices --> CloudLogging
        MyApps --> CloudLogging
        AuditLogs ---> CloudLogging

        CloudLogging --> CloudStorage
        CloudLogging --> BigQuery
        CloudLogging --> PubSub
```
