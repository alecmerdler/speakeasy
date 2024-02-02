# speakeasy

### Usage

1. Start Ollama
```sh
$ ollama serve
```

2. Start Benthos
```sh
$ benthos -c benthos.yaml
```

3. Subscibe to NATS topic:
```sh
$ nats sub "messages.*.response"
```

4. Publish to NATS topic:
```sh
$ nats pub "messages.1234.prompt"
```

The Ollama LLM response should be sent to the NATS subscriber and also printed to stdout in the Benthos teminal.
