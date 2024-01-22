# generative-adversarial-networks
A GAN (Generative Adversarial Network) using PyTorch

**SETTING UP NEW ENV FOR TORCH**
 
Steps for setting up conda env to avoid conflicts in packaging while setting up PyTorch:

`conda create --name gan`

`conda activate gan`


`conda install -c pytorch pytorch=2.0` (The latest version of PyTorch)
Or

`conda install pytorch torchvision torchaudio -c pytorch`

We may get this error:
`RemoveError: 'packaging' is a dependency of conda and cannot be removed from conda's operating environment`

If that is the case, then use 
`conda update --force conda`

on your new conda env and try again.

Once all packages are installed, we install matplotlib in this new environment:
`conda install matplotlib jupyter`

Before opening Jupyter Notebook, we need to register the conda gan environment so that we can create Notebooks using it as the kernel. To do that, with the gan environment activated, we run:
`python -m ipykernel install --user --name gan`

Now we can open Jupyter Notebook by running on the shell:
	
`jupyter notebook`
