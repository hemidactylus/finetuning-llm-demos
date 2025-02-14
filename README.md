# LLM Fine-tuning exercises

Exercises to build experience and map the territory about fine-tuning of LLMs.

> [!IMPORTANT]  
> Pay attention to the first instruction in the notebooks, which instructs you to switch runtime -- otherwise the rest may not work.

## Exercise 1

Fine-tune a LLM downloaded from HuggingFace with a handful of question/answer pairs. Uses LoRA.

[Open in Colab](https://colab.research.google.com/github/hemidactylus/finetuning-llm-demos/blob/main/finetuning1_tiny_hf_lora.ipynb), [view here](finetuning1_tiny_hf_lora.ipynb)

(Adapted from [this](https://medium.com/@rschaeffer23/democratizing-llm-fine-tuning-a-step-by-step-tutorial-for-optimizing-models-without-high-end-41815966e8de))

Todo for this notebook:

- Figure out a clean way to replace `onnxruntime` with `onnxruntime-gpu` (specifying it as an extra does not seem to work).
- Preserve `use_cache=True` all the way to the ONNX reloading: somewhere this setting is lost despite being explicitly set prior to saving the pretraining model.
