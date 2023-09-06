# Python
官方渠道下载 https://www.python.org/downloads/

对于没有提供安装包的历史版本，采用其他方式下载：
- MacOS：`brew install python@3.X`

## VScode 配置
插件安装：
- python语言包（包含pylance）
- Black Formatter
  - 配置 format on save
 
## 包管理器
使用 [Poetry](https://python-poetry.org/) 为包管理器，参考官方文档进行下载，默认安装如果没有加到PATH中，需要手动增加

使用参考 https://blog.kyomind.tw/python-poetry ，调整配置：

`poetry config virtualenvs.in-project true`

> 注意，如果 MacOS 更新了系统的 python，使用 poetry 会出错，这时需要重新安装 poetry，或者参考 https://github.com/python-poetry/install.python-poetry.org/issues/71#issuecomment-1701942693 进行poetry 安装
