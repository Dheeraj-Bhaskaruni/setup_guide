### Mac M1 installation steps

### adding Python to path

- Conda installed via Homebrew
```bash
  conda create -n llm311 python=3.11 -y \
  conda activate llm311
```
    
- install every thing for ML,DL and LLM's
```bash
# PyTorch (+vision/audio/text) with Metal (MPS) support, NumPy, SentencePiece
conda install -y -c conda-forge \
  pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 torchtext==0.17.2 \
  numpy==1.26.4 sentencepiece

# Transformers (Python-only is fine via pip)
python -m pip install --upgrade "pip"
pip install "transformers==4.42.1"
pip install torchtext  # stability
# Jupyter (Lab + classic) and kernel registration
conda install -y -c conda-forge jupyterlab notebook ipywidgets nb_conda_kernels
python -m ipykernel install --user --name llm311 --display-name "Python (llm311)"

conda install conda-forge::spacy

python -m spacy download en_core_web_sm
```

