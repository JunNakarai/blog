# 概要<!-- omit in toc -->

keyballに関する質問をまとめてみれたらいいかなと思い作成。
現状はGitHubでオープンにされている情報を対象にchatGPTに要約してもらいました。
内容に問題があれば問い合わせ位いただけると幸いです。

以下の目次より気になる質疑に飛んでください。要約した本数は現在6/94です。

## No.221 Keyball39のTRSケーブル接続時の動作不良とトラックボールの動作しない問題

[GitHub discussions 221](https://github.com/Yowkees/keyball/discussions/221)

### 質問の背景と目的<!-- omit in toc -->

Q氏は、TRSケーブルを接続した際に片方が動作せず、またトラックボールが全く動作しない問題が発生しており、対処法を求めています。

### 回答と提案 <!-- omit in toc -->
A氏は、ProMicro本体、ProMicro裏のハンダ付け、TRSコネクタのハンダ付けを確認するよう提案し、TRSケーブルを他のものに変えて試すことを提案しています。また、トラックボール基板や光学センサーの購入については、白銀ラボウェブサイトの問合せよりメールを送るよう提案しています。

### 追加の質問と回答<!-- omit in toc -->
Q氏は、ショートしている部分について対処法を尋ねました。A氏は、ショートしている部分がすべてGNDであるため問題ないと回答し、別の部分がショートしていないか確認するよう提案しました。さらに、Keyball39の基板データを公開しているリポジトリを紹介し、KiCADで表示して参考にするよう提案しています。

## No.218 左手用デバイスのランド修復方法

[GitHub discussions 218](https://github.com/Yowkees/keyball/discussions/218)

### 質問の背景と目的<!-- omit in toc -->

- 左手用デバイスのランドが剥がれた原因と対処法について質問
- ![keyball61 Left](https://user-images.githubusercontent.com/130259394/230749368-94cfa43b-7c13-405a-85ef-373d19d0214b.jpg)

### 回答と提案<!-- omit in toc -->

- Yowkees氏からの回答: 緑点の2箇所をエナメル線やゴム被覆導線でショートさせる
- ![Keyball61L_fix](https://user-images.githubusercontent.com/84209772/231066555-e0085d85-ebae-466f-8972-c3cae21b0d80.jpg)

### 追加の質問と回答<!-- omit in toc -->

- -氏が回答に従って作業し、成功した旨の報告

### 解決策と結論<!-- omit in toc -->

- 白い銅線を使用し、左手側デバイスが機能するようになったことが報告される

## No.215 Keyball61の左右判定と特定キーの反応に関する問題

[GitHub discussions 215](https://github.com/Yowkees/keyball/discussions/215)

### 質問の背景と目的  <!-- omit in toc -->

Q氏はKeyball61を組み立てたものの、左右判定と特定キーの反応に問題があり、対処法を求めています。

### 回答と提案  <!-- omit in toc -->

A氏はダイオードのハンダを追加することで問題が解決したと報告しています。


## No.214 Keyball44がiPad Proで動作しない問題

[GitHub discussions 214](https://github.com/Yowkees/keyball/discussions/214)

### 質問の背景と目的 <!-- omit in toc -->

- Q: Keyball44がノートパソコン（Windows）では動作するが、iPad Proに接続すると動作しない
- 他の利用者と相談しても解決に至らず、助言を求める
- 参照ツイート: [Twitter URL](https://twitter.com/lckisaac/status/1645213731067150336?s=20)

### 回答と提案 <!-- omit in toc -->

- A: Q氏が自己解決したと報告
  - SPLIT_USB_TIMEOUTの値を伸ばすことで動作するようになった
- A: Yowkees氏がipadでの使用経験がないことを説
  - SPLIT_USB_TIMEOUTが関係する可能性があるとコメント

### 追加の質問と回答 <!-- omit in toc -->

- A: Q氏が原因が特定できていないことを報告
  - SPLIT_USB_TIMEOUTとの関係性は不明
  - 考察: iPad Proのバッテリー劣化により給電が不安定になる可能性がある

## No.213 左手用デバイスのランドが剥がれた問題とその対処法

[GitHub discussions 213](https://github.com/Yowkees/keyball/discussions/213)

### 質問の背景と目的 <!-- omit in toc -->
Q氏は、左手用デバイスのはんだ付けでランドが剥がれたと思われる問題に直面し、対処法を求めています。

![keyball61 Left](https://user-images.githubusercontent.com/130259394/230749368-94cfa43b-7c13-405a-85ef-373d19d0214b.jpg)

### 回答と提案 <!-- omit in toc -->
A氏は、添付画像に示した緑点の２箇所をエナメル線やゴム被覆導線でショートさせることを提案し、これによってLEFTジャンパを半田付けしたのと同じ効果が得られると述べています。

![Keyball61L_fix](https://user-images.githubusercontent.com/84209772/231066555-e0085d85-ebae-466f-8972-c3cae21b0d80.jpg)

### 追加の質問と回答 <!-- omit in toc -->

Q氏は、指示通りに銅線を用いてハンダでつなぎ、左手側デバイスが機能するようになったことを報告しています。また、白い銅線が目立たなくて良かったと感謝の意を示しています。

## No.212 Keyball39の左手側認識とキー認識の問題と解決方法

[GitHub discussions 212](https://github.com/Yowkees/keyball/discussions/212)

### 質問の背景と目的 <!-- omit in toc -->

ユーザーは、左手側デバイスが正しく認識されず、また1つのキーが認識されない問題が発生し、解決策を求めています。

![Remap](https://user-images.githubusercontent.com/130230380/230725421-78205a30-3fca-4b87-a54e-46b91596ca1c.png)

### 回答と提案 <!-- omit in toc -->

Yowkeesは、両方の問題がCOL5信号線を使用していることを指摘し、ProMicro側の端子の半田付けをチェックするよう提案しています。

![InkedLeft](https://user-images.githubusercontent.com/130230380/230724586-80a27f1c-205c-4f29-82cb-ea1be540e58d.jpg)

![Keyball39_Left](https://user-images.githubusercontent.com/84209772/231068204-a5bf81ae-c7cb-4473-b035-344c76400f3d.jpg)

### 追加の質問と回答 <!-- omit in toc -->
ユーザーは、再度半田付けをした後、コンスルーピンとProMicroの接触が悪かったことが原因であることが分かり、左手側の認識とキーの認識が改善されました。しかし、新たな問題としてUSBを接続していない側がキー入力を認識しない状況が発生しました。Yowkeesは、ProMicroのDATA線の半田付けやTRSコネクタの半田付けを見直すよう提案しています。ユーザーは、ProMicroの半田付けを修正したことで問題が解決し、Keyballが正常に動作するようになったことを報告しています。
