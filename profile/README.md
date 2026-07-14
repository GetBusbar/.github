# Busbar

**[Busbar](https://getbusbar.com)** is a native-protocol LLM gateway — one endpoint
that speaks six wire protocols (OpenAI, Anthropic, Gemini, Bedrock, Cohere,
Responses), routes across weighted pools, translates losslessly between protocols,
and stays up through provider failures with circuit breaking and in-flight failover.
A single static Rust binary.

## Hooks

Your own code on Busbar's normalized request path — observe, steer, or rewrite a
request across all six protocols. Each hook is its own repo:

- **[headroom-hook](https://github.com/GetBusbar/headroom-hook)** — context
  compression: shrink chat history before it reaches the model.
- **[hindsight-hook](https://github.com/GetBusbar/hindsight-hook)** — long-term
  memory: recall and retain context as a gateway service *(beta)*.

## Links

- Website & docs — **[getbusbar.com](https://getbusbar.com)**
- Hooks guide — [getbusbar.com/docs/hooks](https://getbusbar.com/docs/hooks/)
