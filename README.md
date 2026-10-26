# 万代和歌集（まんだいわかしゅう）

雲居の文庫（くもゐのふみぐら）の一作品です。著作権の保護期間が満了した刊本から起こした本文を、誰でも読み・使い・直せるように置いています。

**サイトで読む：[万代和歌集（雲居の文庫（くもゐのふみぐら））](https://informanellica.com/kumoi-no-fumigura/read.html?work=mandai)**（修正案の送信ができます）

| | |
|---|---|
| 分類 | 私撰集 |
| 分量 | 3886段落・99,047字 |
| 状態 | 校正前（版本の画像を OCR したもの。誤りが多い）。作者名の一部は OCR のまま |

## 底本

- [万代和歌集１・２](https://www.digital.archives.go.jp/item/731019)（）
- [万代和歌集３・４](https://www.digital.archives.go.jp/item/730587)（）
- [万代和歌集５・６](https://www.digital.archives.go.jp/item/730310)（）
- [万代和歌集７・８](https://www.digital.archives.go.jp/item/731018)（）
- [万代和歌集９・１０](https://www.digital.archives.go.jp/item/731607)（）
- [万代和歌集１１・１２](https://www.digital.archives.go.jp/item/731606)（）
- [万代和歌集１３・１４](https://www.digital.archives.go.jp/item/730436)（）
- [万代和歌集１５・１６](https://www.digital.archives.go.jp/item/730717)（）
- [万代和歌集１７・１８](https://www.digital.archives.go.jp/item/731609)（）
- [万代和歌集１９・２０](https://www.digital.archives.go.jp/item/731612)（）

底本は上の URL のテキストです。

## 本文の作り方

人が入力・校正したテキスト（パブリックドメイン）を取り込み、プログラムで歌ごと（詞書・作者・左注を分けて）に段落に分けました。振り仮名は本文から外し、JSON の ruby に残しています。それ以外は手を加えていません。

## ファイル

| パス | 中身 |
|---|---|
| `honbun/` | 本文。1 行が 1 首で、`段落ID<TAB>国歌大観の番号<TAB>詞書<TAB>作者<TAB>歌<TAB>左注` の形です。50段落ごとにファイルを分けています（78ファイル）。 |
| `mandai.json` | 本文・底本・作品の説明・作中歌のデータをまとめた JSON（訳は入れず、`yaku/` だけに置いています）。 |

段落ID（例: `mandai-000001`）は、本文を直しても変わりません。

## 誤りを見つけたら


- **Issue で知らせる**：[「本文の誤り」の Issue を作る](https://github.com/kumoi-no-fumigura/mandai-wakashu/issues/new?template=teisei.yml)。段落ID・いまの本文・直した本文・根拠を書いてください。
- **直接直す**：`honbun/` の該当行を直して Pull Request を送ってください。段落IDと行の順番は変えないでください。

受け取った修正は、底本と照らして確かめてから取り込みます。

## ライセンス

[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/deed.ja)。自由に使えます。出典として「雲居の文庫（くもゐのふみぐら）」と、底本の刊本を書いてもらえると助かります。
