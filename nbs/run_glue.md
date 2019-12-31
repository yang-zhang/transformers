- https://gist.github.com/W4ngatang/60c2bdb54d156a41194446737ce03e2e
- https://gist.githubusercontent.com/W4ngatang/60c2bdb54d156a41194446737ce03e2e/raw/17b8dd0d724281ed7c3b2aeeda662b92809aadd5/download_glue_data.py

```
wget https://gist.githubusercontent.com/W4ngatang/60c2bdb54d156a41194446737ce03e2e/raw/17b8dd0d724
281ed7c3b2aeeda662b92809aadd5/download_glue_data.py
python download_glue_data.py --data_dir /tmp/glue_data --tasks STS
```

https://github.com/huggingface/transformers#run_gluepy-fine-tuning-on-glue-tasks-for-sequence-classification

```
export GLUE_DIR=/tmp/glue_data
export TASK_NAME=STS-B

python ./examples/run_glue.py \
    --model_type roberta \
    --model_name_or_path roberta-base \
    --task_name $TASK_NAME \
    --do_train \
    --do_eval \
    --do_lower_case \
    --data_dir $GLUE_DIR/$TASK_NAME \
    --max_seq_length 128 \
    --per_gpu_eval_batch_size=8   \
    --per_gpu_train_batch_size=8   \
    --learning_rate 2e-5 \
    --num_train_epochs 1.0 \
    --output_dir /tmp/$TASK_NAME/
```