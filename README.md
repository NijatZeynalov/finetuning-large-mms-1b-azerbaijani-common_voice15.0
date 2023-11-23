# finetuning-large-mms-1b-azerbaijani-common_voice15.0

This model is a fine-tuned version of [facebook/mms-1b-all](https://huggingface.co/facebook/mms-1b-all) on the common_voice_15_0 dataset.
It achieves the following results on the evaluation set:
- Loss: 0.3188
- Wer: 0.2632

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.001
- train_batch_size: 16
- eval_batch_size: 8
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 100
- num_epochs: 15
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step | Validation Loss | Wer    |
|:-------------:|:-----:|:----:|:---------------:|:------:|
| 7.6471        | 2.0   | 10   | 7.6790          | 1.0658 |
| 5.6745        | 4.0   | 20   | 4.2727          | 1.0088 |
| 3.5016        | 6.0   | 30   | 3.1003          | 1.0    |
| 2.6223        | 8.0   | 40   | 1.8137          | 1.0439 |
| 1.3939        | 10.0  | 50   | 0.6549          | 0.3947 |
| 0.3696        | 12.0  | 60   | 0.3665          | 0.2719 |
| 0.2475        | 14.0  | 70   | 0.3188          | 0.2632 |


### Framework versions

- Transformers 4.35.2
- Pytorch 2.1.1+cu121
- Datasets 2.15.0
- Tokenizers 0.15.0

### Usage

In order to use finetuned mode, you can [click here.](https://huggingface.co/nijatzeynalov/wav2vec2-large-mms-1b-azerbaijani-common_voice15.0) 
