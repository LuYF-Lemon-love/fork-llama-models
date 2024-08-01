# Llama Models

## [Llama Models](#Llama-Models)

|  **Model** | **Launch date** | **Model sizes** | **Context Length** | **Tokenizer** | **Acceptable use policy**  |  **License** | **Model Card** |
| :----: | :----: | :----: | :----:|:----:|:----:|:----:|:----:|
| Llama 2 | 7/18/2023 | 7B, 13B, 70B | 4K | Sentencepiece | [Use Policy](models/llama2/MODEL_CARD.md) | [License](models/llama2/LICENSE) | [Model Card](models/llama2/MODEL_CARD.md) |
| Llama 3 | 4/18/2024 | 8B, 70B | 8K | TikToken-based | [Use Policy](models/llama3/MODEL_CARD.md) | [License](models/llama3/LICENSE) | [Model Card](models/llama3/MODEL_CARD.md) |
| Llama 3.1 | 7/23/2024 | 8B, 70B, 405B | 128K | TikToken-based | [Use Policy](models/llama3_1/MODEL_CARD.md) | [License](models/llama3_1/LICENSE) | [Model Card](models/llama3_1/MODEL_CARD.md) |

### Access to Hugging Face

```python
import transformers
import torch

model_id = "meta-llama/Meta-Llama-3.1-8B-Instruct"

pipeline = transformers.pipeline(
  "text-generation",
  model="meta-llama/Meta-Llama-3.1-8B-Instruct",
  model_kwargs={"torch_dtype": torch.bfloat16},
  device="cuda",
)
```

## Installations

You can install this repository as a [package](https://pypi.org/project/llama-models/) by just doing `pip install llama-models`

## References

1. [huggingface.co/meta-Llama](https://huggingface.co/meta-Llama)
2. [meta/blog](https://ai.meta.com/blog/)
3. [Website](https://llama.meta.com/)
4. [llama get started](https://llama.meta.com/get-started/)
5. [Responsible Use Guide](https://ai.meta.com/static-resource/responsible-use-guide/)
6. [FAQ](https://llama.meta.com/faq)