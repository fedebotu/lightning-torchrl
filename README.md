# Lightning-TorchRL
Experimenting with integrating PyTorch Lightning + TorchRL for differentiable environments running on multiple GPUs!



## Requirements

Since I was most interested in custom environments (this [guide](https://pytorch.org/rl/tutorials/pendulum.html)) given that we can batch and what not, I thought it would be great to try that notebook.

### Installing the `torchrl` nightly version 

But… It looks like with the “stable” release it won’t work. So you can install the `nightly` version with:

`pip install torchrl-nightly`

If you want to install extra dependencies

`pip3 install "torchrl[atari,dm_control,gym_continuous,rendering,tests,utils]"`

### PyTorch 2.0

Going out in early March, it looks like the code has some bugs if we don’t use the latest version. Right now it is still in development, but almost released. To install it, you can follow the [installation instructions](https://pytorch.org/get-started/pytorch-2.0/).

## Known issues

I will open a pull request soon to `torchrl` to fix the `state_dict` problem arising with transformed environments.
