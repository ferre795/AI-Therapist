# AI Therapist

This is a small project I built to explore AI and natural language processing.
It combines:
- a TensorFlow emotion classifier trained on the [dair-ai/emotion](https://huggingface.co/datasets/dair-ai/emotion) dataset
- a pretrained LLM (TinyLlama-1.1B-Chat-v1.0) fine-tuned with LoRA using PyTorch/Transformers

The idea is to detect a user’s emotion from text, then feed that into a chatbot so its replies are more empathetic.

---

## How to run
The easiest way is to open the notebook in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10tAEyPBPaLfZZNmMueTSKTLXYXgqGv0o?usp=sharing)


## Example

**Input:** I feel completely lost and scared.  

**Detected emotion:** Fear  

**Output:** That's common, but you don't have to keep feeling that way. Here are some things you can do to help calm your nerves and start moving forward.  
1. Practice deep breathing. Take slow, deep breaths in through your nose for about 4 seconds, hold your breath for 8–10 seconds, and then exhale slowly out through your mouth for another 6–7 seconds.  

---

**Note:** Some responses may be cut off if the `max_new_tokens` parameter is set too low. Increasing this value will allow longer replies.

