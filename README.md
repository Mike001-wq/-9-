Usage:

For example:

```python
import pickle
usernames = [
    "", # 0
    "", # 1
    "kishida230", # 岸田文雄 2
    "matsunohirokazu", # 松野博一 3
    "nekotanchan", # 金子恭之 4
    "hayashi09615064", # 林芳正 5
    "_suzukitakako_", # 铃木贵子 6
    "SSS_suematsu", # 末松信介 7
    "goto_shigeyuki", # 后藤茂之 8
    "", # 金子原二郎 9
    "saitotetsuo", # 齐藤铁夫 10
    "KishiNobuo", # 岸信夫 11
    "", # 山东昭子 12
    "hosodahiroyuki", # 细田博之 13
    "", # 铃木俊一 14
    "yamagiwa001", # 山际大志郎 15
    "", # 萩生田光一 16
    "244yamaguchi", # 山口壮 17
    "ninoyu_satoshi", # 二之汤智 18
    "NishimeKosaburo", # 西铭恒三郎 19
    "makishimakaren", # 牧岛花莲 20
    "noda_seiko93", # 野田圣子 21
    "wakamiya7788", # 若宫健嗣 22
    "kobahawk" # 小林鹰之 23
]
tweets_pk_path = f"{usernames[0]}_with_translation.pk"
tweets_pk = open(tweets_pk_path, 'rb')
tweets = pickle.load(tweets_pk)
tweets_pk.close()
print(tweets)
```

数据示例:

```python
[{'created_at': '2022-06-01T12:59:18.000Z', 
'id': '1531983729425776640', 
'text': 'マクロン大統領と電話会談し、再選をお祝いしました。特別なパートナーである日本とフランスが、ロシアによるウクライナ侵略に対して、法の支配に基づく国際秩序を守り抜くため、引き続き連携して取り組んでいくことで一致しました。🇫🇷🇯🇵', 
'chinese_content': '我与马克龙总统通了电话，祝贺他再次当选。 日本和法国作为特别伙伴，同意继续共同努力，维护以法治为基础的国际秩序，反对俄罗斯对乌克兰的侵略。 🇫🇷🇯🇵'}]
```
