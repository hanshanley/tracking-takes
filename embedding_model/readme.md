## Model for embedding News Article Passages

We utilize [`e5-base-v2`](https://huggingface.co/intfloat/e5-base-v2) as a base and fine-tune it utilizing LoRA. We note that when utilizing this model, it requires appending the “query: ” as a prefix.
