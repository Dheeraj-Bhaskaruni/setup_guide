### Windows installation steps

### adding Python to path

- install python, add that to path.
  - If not getting added to path
      ```bash
        
       ```
    
- install every thing for ML,DL and LLM's
```bash
conda install -c pytorch -c nvidia -c conda-forge \
    pytorch torchvision torchaudio pytorch-cuda=12.4 \
    numpy pandas scipy scikit-learn matplotlib seaborn jupyter jupyterlab ipykernel \
    transformers datasets evaluate accelerate tokenizers sentencepiece \
    plotly tensorboard -y

conda install conda-forge::spacy

pip install pytorch-lightning peft bitsandbytes trl optimum vllm wandb

```

