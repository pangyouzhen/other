这里以jieba分词的源代码进行解析，进而明白一个源代码解析的步骤

- jieba分词的目录结构
  - `analyse`:
  - `finalseg`:
  - `posseg` ：词性标注
  - `__init__.py`: 主函数，入口函数
  - `__main__.py`: jieba 的命令行，模式，使用  argparse
  - ` _compat.py`： python2与python3 的兼容性
  - `dict.txt`：默认使用的词典
- `__init__py`
  1. 编码和日志的问题
  2. 定义了`Tokenizer` 即分词的类，这个类中主要内容有：定义词典的问题如`initialize` 函数，`load_userdict`函数，