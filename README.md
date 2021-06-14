# Open Telemetry

## Executing

```
docker-compose up -d
```
## Consuming

kafka-protobuf-console-consumer --topic otlp_metrics --broker-list localhost:29092 --proto-dir /Users/matiascascallaresfondevila/Desktop/otlp/proto  --file opentelemetry/proto/metrics/v1/metrics.proto --message ResourceMetrics --from-beginning --debug --pretty

kafka-protobuf-console-consumer --topic otlp_spans --broker-list localhost:29092 --proto-dir /Users/matiascascallaresfondevila/Desktop/otlp/proto  --file opentelemetry/proto/trace/v1/trace.proto --message ResourceMetrics --from-beginning --debug --pretty