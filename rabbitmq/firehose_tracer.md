# Firehose Tracer

## Enabling the firehose

1. Enable trace plugin management UI `$ rabbitmq-plugins enable rabbitmq_tracing`
1. Go to the "Tracing" tab under the "Admin" tab
1. Add a new trace (Set pattern to `#` to capture all messages)
1. Bind exchange/queue to be traced to the topic exchange `amq.rabbitmq.trace`
1. Run `$ rabbitmqctl trace_on`

[source](https://www.rabbitmq.com/firehose.html)
