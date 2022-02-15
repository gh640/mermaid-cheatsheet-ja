# Mermaid チートシート

[Mermaid](https://github.com/mermaid-js/mermaid) の日本語チートシートです。

GitHub の Markdown のコードブロックで Mermaid シンタックスが使えるようになりました。

- [Include diagrams in your Markdown files with Mermaid | The GitHub Blog](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/)

## 公式 README のサンプル

## フローチャート

```
flowchart LR
A[ハード] -->|テキスト| B(ラウンド)
B --> C{判断}
C -->|1| D[結果 1]
C -->|2| E[結果 2]
```

```mermaid
flowchart LR
A[ハード] -->|テキスト| B(ラウンド)
B --> C{判断}
C -->|1| D[結果 1]
C -->|2| E[結果 2]
```

## シーケンス図

```
sequenceDiagram
アリス->>ジョン: やぁ、ジョン、調子はどう？
loop ヘルスチェック
    ジョン->>ジョン: 心気症との闘い
end
Note right of ジョン: 合理的な思考
ジョン-->>アリス: いいよ！
ジョン->>ボブ: 調子はどう？
ボブ-->>ジョン: ばっちりよ！
```

```mermaid
sequenceDiagram
アリス->>ジョン: やぁ、ジョン、調子はどう？
loop ヘルスチェック
    ジョン->>ジョン: 心気症との闘い
end
Note right of ジョン: 合理的な思考
ジョン-->>アリス: いいよ！
ジョン->>ボブ: 調子はどう？
ボブ-->>ジョン: ばっちりよ！
```

## ガントチャート

```
gantt
    section セクション
    完了 :done,    des1, 2014-01-06,2014-01-08
    アクティブ        :active,  des2, 2014-01-07, 3d
    並行 1   :         des3, after des1, 1d
    並行 2   :         des4, after des1, 1d
    並行 3   :         des5, after des3, 1d
    並行 4   :         des6, after des4, 1d
```

```mermaid
gantt
    section セクション
    完了 :done,    des1, 2014-01-06,2014-01-08
    アクティブ        :active,  des2, 2014-01-07, 3d
    並行 1   :         des3, after des1, 1d
    並行 2   :         des4, after des1, 1d
    並行 3   :         des5, after des3, 1d
    並行 4   :         des6, after des4, 1d
```

## クラス図

```
classDiagram
クラス01 <|-- 長ーいクラス : イケてる
<<Interface>> クラス01
クラス09 --> C2 : ここはどこ？
クラス09 --* C3
クラス09 --|> クラス07
クラス07 : equals()
クラス07 : Object[] elementData
クラス01 : size()
クラス01 : int chimp
クラス01 : int gorilla
class クラス10 {
  <<service>>
  int id
  size()
}
```

```mermaid
classDiagram
クラス01 <|-- 長ーいクラス : イケてる
<<Interface>> クラス01
クラス09 --> C2 : ここはどこ？
クラス09 --* C3
クラス09 --|> クラス07
クラス07 : equals()
クラス07 : Object[] elementData
クラス01 : size()
クラス01 : int chimp
クラス01 : int gorilla
class クラス10 {
  <<service>>
  int id
  size()
}
```

## 状態図

```
stateDiagram-v2
[*] --> 停止
停止 --> [*]
停止 --> 移動
移動 --> 停止
移動 --> 衝突
衝突 --> [*]
```

```mermaid
stateDiagram-v2
[*] --> 停止
停止 --> [*]
停止 --> 移動
移動 --> 停止
移動 --> 衝突
衝突 --> [*]
```

### パイチャート（円グラフ）

```
pie
"犬" : 386
"猫" : 85
"ネズミ" : 15
```

```mermaid
pie
"犬" : 386
"猫" : 85
"ネズミ" : 15
```

## Git グラフ（試験的）

```
gitGraph:
options
{
    "nodeSpacing": 150,
    "nodeRadius": 10
}
end
commit
branch newbranch
checkout newbranch
commit
commit
checkout master
commit
commit
merge newbranch
```

```mermaid
gitGraph:
options
{
    "nodeSpacing": 150,
    "nodeRadius": 10
}
end
commit
branch newbranch
checkout newbranch
commit
commit
checkout master
commit
commit
merge newbranch
```

## ユーザージャーニー図

```
  journey
    title 私の勤務日
    section 出勤
      お茶をいれる: 5: 私
      上の階にのぼる: 3: 私
      働く: 1: 私, 猫
    section 退勤
      下の階におりる: 5: 私
      座る: 3: 私
```

```mermaid
  journey
    title 私の勤務日
    section 出勤
      お茶をいれる: 5: 私
      上の階にのぼる: 3: 私
      働く: 1: 私, 猫
    section 退勤
      下の階におりる: 5: 私
      座る: 3: 私
```

## Mermaid 公式

- [リポジトリ](https://github.com/mermaid-js/mermaid)
- [ドキュメント](https://mermaid-js.github.io/mermaid/#/)
- [ライブエディタ](https://mermaid-js.github.io/mermaid-live-editor/)
