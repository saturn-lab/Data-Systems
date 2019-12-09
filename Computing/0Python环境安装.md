# Python环境安装

## Jupyter

使用python-64位3.7.5，勾选环境变量。

```pip install jupyter notebook```

<img src="E:/Database-basics/0计算基础/Python-install-375.png" alt="Python-install" style="zoom:60%;" />/

### 启用jupyter nbextensions

1. 在终端中执行`jupyter nbextensions_configurator enable --system`，使nbextensions生效

2. 然后执行`jupyter contrib nbextension install --system`

3. 然后执行`jupyter contrib nbextension install --sys-prefix`

### 修改Jupyter默认目录和浏览器

1. 首先找到Jupyter的快捷方式，右键-属性-目标中删除“%Userprofile%
2. 打开终端，输入`jupyter notebook --generate-config`，在对应的文件夹中找到jupyter_notebook_config.py
3. 文本打开jupyter_notebook_config.py，查询找到"c.NotebookApp.notebook_dir ="这个字符串，将它前面的“#”号去掉，等号后面赋值默认工作目录，保存退出；
4. 注意 **规避字符常量，比如\0是空字符常量，如果文件夹名称形如“01_APP”，则\要改为\\**
5. Jupyter使用系统默认浏览器，所以打开win10默认应用，修改默认浏览器即可

### 安装和启用nbextensions扩展

1. 使用autopep8，使用`pip install autopep8`安装`autopep8`

2. 打开jupyter，在`edit`-`nbextensions config`中启用`(some) LaTeX environments for Jupyter`,`Collapsible Headings`,`contrib_nbextensions_help_item`,`Equation Auto Numbering`,`Hide input`,`Nbextensions edit menu item`,`Python Markdown`,`Table of Contents (2)`,`Variable Inspector`,`2to3 Converter`,`Autopep8`,`Codefolding`,`Gist-it`,`jupyter-js-widgets/extension`,`Live Markdown Preview`,`Move selected cells`,`Nbextensions dashboard tab`,`Split Cells Notebook`



## Git

### Git Bash

Git-Gui软件



### Github Desktop

用的桌面版Github Desktop

1. 到[Github Desktop](https://desktop.github.com/)下载并安装Github Desktop
2. 登录账号，clone仓库，有更新时pull和push，暂存待定更新不要直接commit到master上……
3. 安装[MathJax Plugin for Github](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima?h1=zh)可以在Github上看到LaTeX代码的数学公式