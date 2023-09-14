# Stable Diffusion Lora Finetuning with OpenVINO

This repo contains experimental code to finetune stable diffusion using LoRA (Low Rank Adaptation) technique with torch.compile OpenVINO backend. 

Below are the instructions to set up and experiment with this feature:
* Create and activate a Python virtual environment:
  ```
  python -m venv lora_env
  source lora_env/bin/activate
  ```
* Clone this repository:
  ```
  git clone https://github.com/ynimmaga/lora_fine_tuning
  ```
* Install the prerequisites:
  ```
  pip install -r requirements.txt
  ```
* Set up the environment variable to use Torch FX based OpenVINO backend:
  ```
  export PYTORCH_TRACING_MODE=TORCHFX
  ```
* Configure the HuggingFace CLI and login by entering the HuggingFace token:
  ```
  huggingface-cli login
  ```
* Run the script:
  ```
  ./sd_lora.sh
  ```
  
  
