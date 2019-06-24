# PyTorch Pretrained BERT: The Big & Extending Repository of pretrained Transformers



Fork of https://github.com/huggingface/pytorch-pretrained-BERT, with a modification to the [Openai GPT](https://github.com/epsdg/pytorch-pretrained-BERT/tree/master/pytorch_pretrained_bert/modeling_openai.py#L955-L960) and [GPT-2](https://github.com/epsdg/pytorch-pretrained-BERT/tree/master/pytorch_pretrained_bert/modeling_gpt2.py#L943-L948
) models to support binary classification using the DoubleHeadsModel.  Substitutes BCEWithLogitsLoss instead of CrossEntropyLoss if num_choices == 1.  Targets should be a 1-dimensional array in [0, 1] (int and float both work; targets are cast to float before passing to the loss fn).
