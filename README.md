Usage:
For example:
```python
import pickle
dataset = ['kishida_speech', 'yasushi_speech', 'hayashi_speech']
dataset_pk_path = f"{dataset[2]}.pk"
dataset_pk = open(dataset_pk_path, 'rb')
speech = pickle.load(dataset_pk)
dataset_pk.close()
print(speech)
```
数据示例:
[{"source": "https://www.kantei.go.jp/...",
"title": "关于...记者会",
"chinese_content": "中文",
"japanese_content": "日本语"}]
数据:
kishida_speech https://www.kantei.go.jp/cn/101_kishida/statement 47 无日文 中文（官方参考）
yasushi_speech https://www.soumu.go.jp/menu_news/kaiken 64 日文 中文（机器翻译）
hayashi_speech https://www.mofa.go.jp/mofaj/press/kaiken/gaisho 82 日文 中文（机器翻译）
