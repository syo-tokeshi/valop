# 使用イメージ

オプション(-a or -r or -o) + rubyっぽく引数を渡すと、
- 配列  
- オブジェクト(rubyではハッシュとしても使えます)  

のデータが手に入ります😊

<img width="486" alt="スクリーンショット 2023-03-22 18 37 25" src="https://user-images.githubusercontent.com/54713809/226863033-69e30c31-cf47-44a2-93bc-dfda8f46ec2f.png">  

![demo](https://user-images.githubusercontent.com/54713809/226875881-d6e7350b-1b05-4835-8177-83d618ed7fe3.gif)  

# 概要

本プログラムは手軽に  
・配列  
・オブジェクト(rubyではハッシュとしても使えます)  
を作成する事が出来ます。  

プログラミングの学習で「サクッと」データが欲しい時があると思います。  

その際にご使用ください。    

`-a -r -o`どちらかのオプションを指定してご利用下さい。

# ご利用方法

**ご利用の際は、`-a -r -o`どちらかのオプションを指定してご利用下さい。**
```
# インストール
npm install -g valueop
npm install -g minimist # 依存関係のため必要

# [使用例]

# -aオプションの引数はスペース区切りで渡してください
❯ valueop -a neko inu salu 
[ 'neko', 'inu', 'salu' ]

# -rオプションは
# 1. [1以上の数値]..[2以上の値]を渡す
# 2. [a以上の値]..[z以下の値]を渡す
# でお願い致します。

❯ valueop -r 1..5
[ 1, 2, 3, 4, 5 ]
❯ valueop -r a..e 
[ 'a', 'b', 'c', 'd', 'e' ]

# -oオプションも引数はスペース区切りで渡してください
❯ valueop -o neko inu salu 
{ key1: 'neko', key2: 'inu', key3: 'salu' }
```

**-a or -r: 単純な配列を作成します。**

**-o : オブジェクト(rubyではハッシュとしても使えます)を作成します**
