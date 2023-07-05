
# nano_aim

This is a fork of [nanoGPT](https://github.com/karpathy/nanoGPT) that adds integration with the [Aim experiment tracker](https://aimstack.io/).

## Code Changes

See [this diff](https://github.com/karpathy/nanoGPT/compare/master...nfergu:nano_aim:master#diff-ed183d67207df065a11e1289f19d34cc2abbc5448dea952683cfe9728c342b95) for the code changes made to nanoGPT to track experiments in Aim.

## Getting Started

1. Install Aim and Plotly: `pip install aim plotly`
2. Install this repo per the instructions in the [nanoGPT readme]([https://github.com/karpathy/nanoGPT/README.md](https://github.com/karpathy/nanoGPT/blob/master/README.md)).
4. Train a model as normal. For example: `python train.py config/train_shakespeare_char.py --device=cpu --compile=False --eval_iters=20 --log_interval=1 --block_size=64 --batch_size=12 --n_layer=4 --n_head=4 --n_embd=128 --max_iters=2000 --lr_decay_iters=2000 --dropout=0.0 --eval_interval=100`
5. Run `aim up` and your results will be available in Aim.

## Demo

![Screen Recording 2023-07-05 at 00 17 36](https://github.com/nfergu/nano_aim/assets/1291583/9a2f783f-8511-4475-96bb-b5bb6711e5aa)

