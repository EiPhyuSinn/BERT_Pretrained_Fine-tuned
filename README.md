# Fine-Tuning BERT in Three Ways

This project explores three simple and effective ways to fine-tune a pre-trained BERT model using a custom dataset.

## Fine-Tuning Methods

1. **Full Fine-Tuning**  
   All layers of the BERT model are trained. This method works best when you have enough labeled data and computational resources.

2. **Transfer Learning (Freezing Layers)**  
   Most layers of BERT are frozen, and only the final pooling or classification layers are trained. This is useful for smaller datasets and faster training.

3. **LoRA (Low-Rank Adaptation)**  
   LoRA introduces trainable low-rank matrices to adapt the model while keeping most parameters frozen. It's highly efficient and requires fewer resources.

## Requirements

- `transformers`
- `datasets`
- `torch`
- `peft` (for LoRA)

Install with:

```bash
pip install -r requirements.txt
```