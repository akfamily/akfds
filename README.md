# AKFDS 知识库

这是一个关于财经数据科学知识的开源知识库，作者是 [Albert King](https://www.akshare.xyz/)。
本知识库创建的主要目的是为了方便财经数据科学爱好者、数据科学家及相关人士查询相关的财经资料，
能够提高在财经数据科学领域的工作效率，也可以作为茶余饭后学习的园地。

## 搭建运行环境

The conda environment is provided as `environment.yml`. This environment is used for all testing by Github Actions and can be setup by:

1. `conda env create -f environment.yml`
2. `conda activate akfds-dev`

## 本地构建

Run the following command in your terminal:

```bash
jb build akfds/
```

If you would like to work with a clean build, you can empty the build folder by running:

```bash
jb clean akfds/
```

If jupyter execution is cached, this command will not delete the cached folder. 

To remove the build folder (including `cached` executables), you can run:

```bash
jb clean --all akfds/
```

## 发布知识库

This repository is published automatically to `gh-pages` upon `push` to the `master` branch.

```bash
ghp-import -n -p -f akfds/_build/html
```

## 注意事项

This repository is used as a test case for [jupyter-book](https://github.com/executablebooks/jupyter-book) and 
a `requirements.txt` file is provided to support this `CI` application.
