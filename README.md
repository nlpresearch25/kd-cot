# kd-cot

Information about the content of the directories:

Data:
- Contains training and evaluation data.

Models:
- The LLMs should be downloaded from HuggingFace and stored in the directories with corresponding names.

Scripts:
- Contains the scripts (training and evaluation) to reproduce the tables in the paper.

Running scripts:

First install the conda environment to run training and evaluation scripts.
Follow the instructions in the INSTALLATION.txt file to install this environment.

After installing the environment, the scripts can be run to reproduce the tables in the paper as follows:

REPRODUCE TABLE 1 IN THE PAPER:
cd reproduce_table_1
# Training of vanilla KD
sh training_vanilla_kd.sh
# Training of KD+CoT
sh training_kd+cot.sh
# Run evaluation of Qwen-1.8B (student) model on BBH
sh run_eval_Qwen_1.8B.sh
# Run evaluation of Qwen-7B (teacher) model on BBH
sh run_eval_Qwen-7B.sh
# Run evaluation of KD model (Change the model directory for either vanilla KD or KD+CoT models and tokenizers)
sh run_eval_Qwen_KD.sh

REPRODUCE TABLE 2 IN THE PAPER:
cd reproduce_table_2
# Training of vanilla KD
sh training_vanilla_kd.sh
# Training of KD+CoT
sh training_kd+cot.sh
# Run evaluation of Llama2-7B (student) model on BBH
sh run_eval_Llama2-7B.sh
# Run evaluation of Llama2-13B-Chat (teacher) model on BBH
sh run_eval_Llama2-13B-Chat.sh
# Run evaluation of KD model (Change the model directory for either vanilla KD or KD+CoT models and tokenizers)
sh run_eval_Llama2-7B_KD.sh

REPRODUCE TABLE 3 IN THE PAPER:
cd reproduce_table_3
# Training of vanilla KD
sh training_vanilla_kd.sh
# Training of KD+CoT
sh training_kd+cot.sh
# Run evaluation of TinyLlama (student) model on BBH
sh run_eval_TinyLlama.sh
# Run evaluation of Llama2-13B-Chat (teacher) model on BBH
sh run_eval_Llama2-13B-Chat.sh
# Run evaluation of KD model (Change the model directory for either vanilla KD or KD+CoT models and tokenizers)
sh run_eval_TinyLlama_KD.sh
