# MELIO Machine Translation ZINDI COMPETITION

This folder contains the instructions to train and deploy a translation model (from Dyula to French) on Highwind.


A Jupyter notebook: `Melio_mt_dyu_fr.ipynb` is provided which has the code to run the entire tutorial from preprocessing -> training -> inference.

## Folder structure

```bash
.
├── deployment
└── models
```

1. The `deployment` folder contains instructions on how to create a Kserve custom predictor to be deployed on Highwind.
    1. The `main.py` contains the inference and deployment code from `Melio_mt_dyu_fr.ipynb`.
1. The `models` folder contains the pretrained Huggingface model with tokenizer configurations.
    1. The `pipeline.py` contains the training code from `Melio_mt_dyu_fr.ipynb`.