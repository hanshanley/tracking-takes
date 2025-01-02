## Model for embedding News Article Passages

We utilize [`e5-base-v2`](https://huggingface.co/intfloat/e5-base-v2) as a base and fine-tune it using LoRA. We note that this model requires appending the “query: ” as a prefix.

The base contrastive model contains code for loading our model and the   `embedding.py` file contains code for embedding texts. As previously noted, if using the e5-base model, it requires appending the “query: ” as a prefix.

The LoRA weights are within the `model_weights` folder. 
