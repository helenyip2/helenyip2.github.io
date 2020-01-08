---
layout: post
title: How to work Jupyter notebook with `virtualenv` in Linux
---

When working for different projects, I try to set up a different virtual environment for each one.

This is how I do it when working in a Linux environment

Make sure that jupyter notebook is installed globally
```bash
sudo install pip3 install jupyter
```

Make sure you're in the `Environment` folder of your VM

```bash
source proj_env1/bin/activate
```

Use `pip3` to install the packages that you want in your environment.

After you've installed everything that you need, install
```bash
pip3 install ipykernel
```

If you want to get your virtual environment to be linked to your jupyter notebook, you need to add another kernel to it.

[] Explain what jupyter kernel means.

1. First install `ipykernel` in order to add kernels to your jupyter notebook environment
```bash
pip3 install ipykernel
```

2. With your virtual environment open, set the following thing in your thing.
```bash
python -m ipykernel install --user --name proj_env1 --display-name "project_env"
```
What you put under `--name` is the actual name of your virtual environment.
`--display-name` is what's shown as the name of the kernel in Jupyter notebook.

3. Go into your project file & open jupyter notebook
```bash
jupyter notebook
```

4. Under kernel, change your kernel to the one you created. (Remember the display name you inputted earlier on.)

5. Run notebook to see if your imports work.


