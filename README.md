# golang_kafka_client_benchmark

Copied and modified from [https://github.com/bigwhite/experiments/tree/master/kafka-clients/benchmark](https://github.com/bigwhite/experiments/tree/master/kafka-clients/benchmark)

Clients included:
- [IBM/sarama](https://github.com/IBM/sarama)
- [confluentinc/confluent-kafka-go](https://github.com/confluentinc/confluent-kafka-go)
- [twmb/franz-go](https://github.com/twmb/franz-go)
- [segmentio/kafka-go](https://github.com/segmentio/kafka-go)

### Benchmark Result

```
goos: darwin
goarch: arm64
pkg: kafka_client_benchmark
cpu: Apple M2
BenchmarkSaramaAsync-8                           1389248               870.9 ns/op           294 B/op          1 allocs/op
BenchmarkSaramaAsyncInParalell-8                 1301533               823.7 ns/op           294 B/op          1 allocs/op
BenchmarkKafkaGoAsync-8                          3095522               432.9 ns/op           393 B/op          5 allocs/op
BenchmarkKafkaGoAsyncInParalell-8                1588862               694.4 ns/op           399 B/op          5 allocs/op
BenchmarkConfluentKafkaGoAsync-8                 3309720               340.0 ns/op           126 B/op          3 allocs/op
BenchmarkConfluentKafkaGoAsyncInParalell-8       1781802               663.6 ns/op           227 B/op          5 allocs/op
BenchmarkFranzGoAsync-8                          3069508               409.8 ns/op           101 B/op          5 allocs/op
BenchmarkFranzGoAsyncInParalell-8                1846957               569.6 ns/op           272 B/op          6 allocs/op
```
