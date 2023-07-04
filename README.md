
# nano_aim

This is a fork of [nanoGPT](https://github.com/karpathy/nanoGPT) that adds integration with the [Aim experiment tracker](https://aimstack.io/).

## Code Changes

See [this commit](https://github.com/nfergu/nano_aim/commit/a64d9513d8ceee81874e529e5e633d5a61eeef99) for the code changes required to track training in Aim.

## Getting Started

1. Install Aim and Plotly: `pip install aim plotly`
2. Install this repo per the instructions in the [nanoGPT readme]([https://github.com/karpathy/nanoGPT/README.md](https://github.com/karpathy/nanoGPT/blob/master/README.md)).
4. Train a model as normal. For example: `python train.py config/train_shakespeare_char.py --device=cpu --compile=False --eval_iters=20 --log_interval=1 --block_size=64 --batch_size=12 --n_layer=4 --n_head=4 --n_embd=128 --max_iters=2000 --lr_decay_iters=2000 --dropout=0.0 --eval_interval=100`
5. Run `aim up` and your results will be available in Aim.

## Demo

![Screen Recording 2023-07-05 at 00 17 36](https://github.com/nfergu/nano_aim/assets/1291583/9a2f783f-8511-4475-96bb-b5bb6711e5aa)

