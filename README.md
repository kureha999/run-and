# サービス概要
* 毎日の散歩を楽しく記録してシェア
* お散歩の時のお気に入りの場所を写真でシェア
* 散歩に行く時間にLINEなどで通知してくれる

# このサービスへの思い・作りたい理由
* 祖母が犬と暮らしていて散歩をしたか忘れていて何回も行っていたので何か解決できるのは、無いかなと思い作ろうと思っています。
> スマホアプリは、苦手ですけどLINEは、スマホに入っていてよくみているのでそこで通知して記録が取れるアプリがいいと思いました
* 私自身も犬の散歩が好きでドッグランなどいくのですが色々な方のお気に入りスポットを共有したいと思いがありました。

# ユーザー層について
* ユーザー層は、私の祖母と同じ年齢が高く犬を飼っている方。
* 子供にも使ってもらいたいと思っています。
> 20代などは、アプリをするならゲームのできるドラクエウォーク、ポケモンGOがあるのでなしです

# サービスの利用イメージ
小学生以下と60~70歳以上を狙っているのでUIは、わかりやすく見やすいものにして、
PCよりスマホで見やすいものを作成しようと思っています。

気軽に記録をして色んな人とシェアする楽しさ、忘れないようにするため

# ユーザーの獲得について
X(Twitter)で拡散して知ってもらってそこから知り合いや家族に勧めて広まる想定です。

# サービスの差別化ポイント・推しポイント
敢えてサービスを沢山入れないことで分かりやすく使いやすい様にしようと思ってます。

# 機能候補
現状作ろうと思っている機能、案段階の機能をしっかりと固まっていなくても構わないのでMVPリリース時に作っていたいもの、本リリースまでに作っていたいものをそれぞれ分けて教えてください。
###### MVP-before
* LINEログイン機能
* LINE通知機能(餌,散歩時間を設定したら通知がなる)
* 画像加工・合成
* お散歩をした時間と餌をあげた時間記録スペース
> 投稿、編集、削除
> スマホを持って散歩に行かない想定ですので帰ってから記録する流れ
###### MVP-after
* お気に入りのスポット&愛犬の写真共有機能
> > 投稿、編集、削除
* コメント機能
* いいね機能
* データ共有機能(家族で同じアカウントにアクセスできるように。例えば孫が祖母の散歩記録を確認するなど)

# 機能の実装方針予定
###### 'CarrierWave' 'MiniMagick'
投稿された画像の画質を落とさずに画像サイズを固定するだけ
###### line-bot-sdk-ruby
LINEでのプッシュ通知
###### 'devise' 'omniauth-line' 'omniauth-rails_csrf_protection'
LINEログイン機能

