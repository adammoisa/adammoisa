### Hi, I'm Adam 👋

I work on [Magicare](https://magicare.ai), an AI-native operating system for skilled nursing facilities: census, reimbursement and compliance.

#### Open source

- **[vLLM](https://github.com/vllm-project/vllm)**: [`#43424`](https://github.com/vllm-project/vllm/pull/43424) fixes structured output under speculative decoding with a reasoning parser. Bonus tokens sampled on the step where reasoning ends were leaking into the response as garbage before the JSON (e.g. `chunk_0{...}`), because the grammar mask only turns on after the boundary. The PR adds a pre-commit grammar filter that also handles multi-token reasoning markers like gpt-oss's Harmony `<|channel|>final<|message|>`. Root cause written up in [`#43338`](https://github.com/vllm-project/vllm/issues/43338).
- **[Bifrost](https://github.com/maximhq/bifrost)**: [`#10042`](https://github.com/maximhq/bifrost/pull/10042) adds Perplexity's `locate` decision type (`pplx-decider-v1.3`) to the gateway's `/v1/decisions` API end to end: schema, the provider converters, the HTTP handlers, and clear 400s from providers that can't serve it, with benchmarks on the request path.

#### Elsewhere

[magicare.ai](https://magicare.ai) · [x.com/adammoisa](https://x.com/adammoisa)
