- https://github.com/huggingface/transformers/blob/master/CONTRIBUTING.md#start-contributing-pull-requests

```
Fork the repository by clicking on the 'Fork' button on the repository's page.
$ git clone git@github.com:<your Github handle>/transformers.git
$ cd transformers
$ git remote add upstream https://github.com/huggingface/transformers.git
$ pip install -e ".[dev]"
Right now, we need an unreleased version of isort to avoid a bug:
$ pip install -U git+git://github.com/timothycrosley/isort.git@e63ae06ec7d70b06df9e528357650281a3d3ec22#egg=isort
```

- https://docs.python.org/3/tutorial/venv.html
```
➜  transformers git:(master) python -m venv ./venv
➜  transformers git:(master) source venv/bin/activate
(venv) ➜  transformers git:(master) which python
/Users/yang.zhang/git/yztransformers/transformers/venv/bin/python
(venv) ➜  transformers git:(master) pip install ipykernel
(venv) ➜  transformers git:(master) python -m ipykernel install --user --name yztransformers
Installed kernelspec yztransformers in /Users/yang.zhang/Library/Jupyter/kernels/yztransformers
```