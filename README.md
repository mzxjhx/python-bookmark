## python-bookmark
python给pdf编辑书签



#### 环境配置

```python
Python 3.9.6 (tags/v3.9.6:db3ff76, Jun 28 2021, 15:26:21) [MSC v.1929 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.

pikepdf 8.8.0
```



#### 使用方法

bookmark.py 是给pdf添加书签，在pycharm中的命令如下
```python
#命令需要四个参数
python .\bookmark.py pdf_path bookmark.txt page_offset
# 示例
python .\bookmark.py "D:\\123.pdf" "D:\\123.txt" 18
```



四个参数说明如下

| .\bookmark.py | 要运行的python文件                                           |
| ------------- | ------------------------------------------------------------ |
| pdf_path      | pdf路径。当前目录下，如pdf文件名123.pdf，则pycharm工具里可以直接 '.\123.pdf' |
| bookmark.txt  | 书签使用txt编辑，保存成utf-8编码格式。缩进使用tab或空格      |
| page_offset   | pdf页码和书的实际书签页码会有一个差值，这个参数补这个差值    |

delbookmark.py 是删除pdf书签

```python
python.exe .\delbookmark.py '.\123.pdf'
```

