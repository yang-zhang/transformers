- https://github.com/huggingface/transformers#run_generationpy-text-generation-with-gpt-gpt-2-ctrl-transformer-xl-and-xlnet

```
python ./examples/run_generation.py \
    --model_type=gpt2 \
    --length=50 \
    --model_name_or_path=gpt2-large \

python ./examples/run_generation_repeat.py \
    --model_type=gpt2 \
    --length=20 \
    --model_name_or_path=gpt2 \
```