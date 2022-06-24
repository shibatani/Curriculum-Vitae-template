## 基本情報

|key|value|
|---|-----|
|Name|柴谷遼太朗|
|GitHub|[@shibatani](https://github.com/shibatani/)|
|Zenn|https://zenn.dev/shibari_yo|
|Wantedly|https://www.wantedly.com/id/ryotaro_shibatani|
|Zenn|https://zenn.dev/shibari_yo|


## スキル
### 言語
|言語|経験年数|レベル|
|---|-------|-----|
|HTML|2年|実務で問題なく使える|
|CSS|2年|実務で問題なく使える|
|SCSS|2年|実務で問題なく使える|
|Ruby|1年|基本的なプログラミングが可能|
|JavaScript|1.5年|実務で問題なく使える|
|TypeScript|1.5年|実務で問題なく使える|

### フレームワーク

|フレームワーク|経験年数|レベル|
|---|-------|-----|
|Ruby on Rails|1年|基本的な使用が可能|
|Vue.js|1.5年|実務で問題なく使える|
|Nuxt.js|1.5年|実務で問題なく使える|

# 職務経歴  

## 2020/12 - 現在 : 株式会社iRidge

## 家具・インテリア用品系アプリのCMS開発

### PJでの主な役割
・家具・インテリア用品系最大手会社様のCMS画面新規開発および既存機能改修
・アプリから呼び出されるWebView画面の既存機能改修

### 環境
- チーム規模: 10人 (フロントエンドエンジニア 1名(自分), バックエンドエンジニア 2名, インフラエンジニア 1名, Androidエンジニア 2名, IOSエンジニア 2名, PM 4名)
- 役割: フロントエンドエンジニア
- 使用技術: TypeScript, Vue.js/Nuxt.js, HTML, CSS, SCSS, Stylus, Pug, AWS(S3), GitLab CI

### 業務内容
- フロント側のメインエンジニアとして参画。
- PMおよび発注側とコミュニケーションを取りながら作成。
- PM側からの技術的相談にも対応。
- 工数見積もりにも対応。
- その他既存機能改修。

#### メンテナンスモード・強制アップデート管理画面の作成
  - 概要

    以前、PM側でモバイルアプリのメンテナンスモード・強制アップデートについてFirebase上で操作する必要があった。それらの作業を管理画面上で完結できように専用の管理画面を作成した。
  - 取り組み

    メンテナンスモード管理機能については、メンテナンス期間・メンテナンス時にアプリ側で表示されるテキストメッセージを設定できるようにした。 強制アップデート機能については、IOSもしくはAndroidの対象Ver・メンテナンス時にアプリ側で表示されるテキストメッセージを設定できるようにした。アプリ側では、対象Ver未満のアプリに対してアップデートを促すダイアログが表示される。
  - 工夫した点

     メンテナンスモードもしくは通常モードか一目でわかるように「状態」欄を作成した。さらにメンテナンスモード時には、赤色基調の文字色を使用し、主張するように工夫した。
       また、初めてシステムを使用した人がわかりやすいように使い方マニュアルリンクをページ内に配置し、モーダルで表示されるよう工夫した。

#### 重要なお知らせ管理画面の作成
  - 概要

    コロナにおける店舗営業時間の変更アナウンスや商品問題など緊急性の高い重要なお知らせをユーザー全体に発信する。CMS側では、それらのお知らせ内容を管理する画面を作成した。
  - 取り組み

    投稿画面では、表示日付・お知らせ内容・お知らせ内容の文字色・サムネイル・Draft状態かどうか・掲載期間・URLなどを設定できるようにした。
また一覧画面では、掲載予定・掲載期間中・過去の画面のように時系列に分けて管理できるようにした。
  - 工夫した点

    一覧画面ではお知らせ数が膨大になることを加味して、ステータスやタイトルなどでの絞り込みや掲載期間順にソートできるように工夫した。追加で顧客の要望に応え、選択した記事をCSV抽出できるようにした。また、同じような画面構成で作成されている既存一覧画面に対して、これらの機能を転用して使いやすくするように努めた。

#### トップバナー管理画面の作成
  - 概要

    アプリのトップ画面で表示される複数のバナーをCMS側で管理できるようにした。
  - 取り組み

    管理画面では、バナーのサムネイル・URL・表示するかどうかなどを設定できる項目を複数作成した。
  - 工夫した点

    サムネイルに表示する画像を大きさ・縦横比に関わらず全体表示できるように既存ライブラリ(Element UI)を使用して工夫した。

#### Node 12系→16系&サードパーティライブラリのアップデート
  - 概要

    Node 12系のLTS終了前にアクティブLTSである16系にアップデートした。またそれらに伴い、サードパーティライブラリのアップデートも行った。
  - 取り組み・大変だったこと

    サードパーティライブラリについては、ほぼ全て最新安定版にアップデートした。その中でも`eslint`、`date-fns`のバージョンが特に遅れており、記述の変更が大変だった。また、他ライブラリの依存関係において最新安定版で機能しないライブラリが存在し、それらの依存関係解消に時間がかかった。

#### リリース・オンボーディング関連のドキュメント作成
  - 概要

    以前はスポット的な対応が多かったため、継続的にPJに参加するフロントエンドエンジニアがおらず、あまりドキュメント類が整備されていなかった。特にリリース・オンボーディング関連のドキュメントが存在せず、次の新規参画者が路頭に迷うと考えたため、開発の合間にドキュメントを作成した。
  - 取り組み

    リリース関連については、フロントエンドのNotionページの中にリリースノート置き場を作成した。また、リリースノート雛形を作成し、テンプレート化させて次回リリースに使いまわせるように工夫した。Gitlab上でもリリースVerのタグ付けを行い、いつでもリリース内容を振り返れるように改善した。
  オンボーディング関連については、環境構築ページを作成してCMS、WebViewの立ち上げに必要な情報を記載した。

## 観光系Web版アプリの開発

### PJでの主な役割
鉄道系会社様が運営する観光系Web版アプリの既存機能改修

### 環境
- チーム規模: 10人 (フロントエンドエンジニア 3名, デザイナー 2名, バックエンドエンジニア 2名, Android/IOSエンジニア 1名, PM 2名)
- 役割: フロントエンドエンジニア
- 使用技術: JavaScript, Node.js/Express, HTML, CSS, SCSS

### 業務内容
- フロント側のメインエンジニアとして参画。
- PMおよび発注側とコミュニケーションを取りながら作成。

#### Web版アプリのレスポンシブ化対応
  - 概要

    以前Web版アプリは、PC画面のみ対応しておりSP画面に対応していなかった。
それらの解消にあたり、対応する画面数が膨大なため3人のエンジニアで担当画面を分割して対応を行った。
    
  - 取り組み

    対応の詳細な流れとしては、以下のように進めた。
    ①PM、デザイナー、エンジニアで対応する画面を決める。
    ②デザイナーがデザイン案をXDにまとめる。
    ③それらを元にエンジニアが対応する。

    エンジニアの具体的な対応方法としては、画面幅768px以上をPC画面、それ以下をSP画面としててスタイルをあてるようにした。また、スタイリングはBEMに準じて行うように共通認識を合わせて案件に取り組んだ。

  - 工夫した点

    エンジニア3人で担当画面を分割して対応するため、共通スタイルが絡むタスクを優先的に片付けるように工夫した。また対応する画面数が膨大なため、実装途中で要件が定まっていない箇所がいくつか出てきた。それらに関してデザイナーさんと直接話し合い、その場で要件を決めて迅速に対応した。

#### Node 12系→16系&サードパーティライブラリのアップデート
  - 概要

    Node 12系のLTS終了前にアクティブLTSである16系にアップデートした。またそれらに伴い、サードパーティライブラリのアップデートも行った。
  - 取り組み・大変だったこと

    サードパーティライブラリについては、ほぼ全て最新安定版にアップデートした。その中で`scss`のバージョンアップデートに伴い、ほぼ全てのscssファイルの記述を変更する作業が発生して苦労した。
    
## 鉄道系アプリのWebView開発

### PJでの主な役割
鉄道系モバイルアプリで表示するWebView作成。

### 環境
- チーム規模: 13人 (フロントエンドエンジニア 2名, バックエンド/インフラエンジニア 1名, モバイルエンジニア 2名, QAエンジニア 2名, デザイナー 2名, PM 4名)
- 役割: フロントエンドエンジニア
- 使用技術: TypeScript, Vue.js/Nuxt.js, HTML, CSS, SCSS, GitLab CI

### 業務内容
- フロント側のメインエンジニアとして参画。
- PMおよびデザイナーとコミュニケーションを取りながら作成。
- 既存機能の修正
  - イベントトラッキング対応

#### キャンペーン・スタンプラリー画面のUI/UX改善
  - 概要

    今後、鉄道会社様の方で多数のキャンペーン・スタンプラリー企画を計画しており、画面内にバナーが乱立することによって、ユーザー自身の興味のあるキャンペーン・スタンプシートに簡単にアクセスすることが出来なくなってしまう恐れがあった。画面のUI/UXを改善することによってこれらの問題を解決した。
  - 取り組み

    以前の画面は、キャンペーン項目とスタンプラリー項目を分ける事なく、上から順番にバナーを並べる構成だった。それらを変更し、画面上部はキャンペーン項目のスペース、画面下部はスタンプラリー項目のスペースに分け、それぞれの項目のバナーをスライダーでスワイプできるようにした。
  - 苦労した点

    スライダー間の幅や次スライダーをはみ出して見せるデザインなどの細かい表現をできるだけXD通りに再現できるように実装した。また、ページネーション部分が画面幅を変えることによってスタイル崩れが起こしていたが、スタイルのあて方を工夫することによって解決することができた。

#### 駅に基づく他社連携画面の作成
  - 概要
 
    ユーザーのお気に入り駅に紐づく他社連携画面を作成した。
  - 取り組み

    他社連携データに応じてボタンリンクを画面内に配置する。他社路線データが存在する場合は、他社アプリの列車走行位置リンクを配置し、バス/2次交通データが存在する場合は、HPリンクを配置するようにした。

## 銀行系Webサイトのデモ開発

### PJでの主な役割
銀行系Webサイトのデモ開発

### 環境
- チーム規模: 2人 (フロントエンドエンジニア 1名,  デザイナー 1名)
- 役割: フロントエンドエンジニア
- 使用技術:  HTML, CSS, JavaScript, jQuery  GitLab

### 業務内容
- メインエンジニアとして参画。
- デザイナーとコミュニケーションを取りながら作成。
- 工数の見積もりを担当。

#### 銀行系Webサイトのデモ開発
  - 概要

    依頼会社様にフロント系・デザイン系の技術に明るい方がおらず、自社で巻き取る形となった。旧態依然のデザインからモダンなデザインへサイトを一新させた。
コーディングについては、主要3画面&部分パーツのみの提供で、それらを依頼会社様の方で使い回して完成させる予定となっていた。
    
  - 取り組み

    依頼会社様が以前使用していたWebサイトのデザインから一新させる予定だったので、共有いただいた既存ソースは参考にならず、ほぼ0からコーディングを行った。

  - 工夫した点

    コーディング期間が3週間とタイトなスケジュールであったため、できるだけ早くアウトプットを出し、より多くのフィードバックを受け、少ない時間で品質が担保されるように工夫した。また、画面幅変更時の挙動が明確になっていない箇所が存在し、デザイナーさんと相談して技術的に可能な範囲で対応した。
作品自体は、非常に完成度が高いと同じPJに関わったデザイナーさん、デザイナー部長に評価いただけた。

## 社外プロジェクト

### 医療アプリ ツイキュアの開発
Twitter上で活動している医師に対し、匿名で医療相談のできるwebサービス「[ツイキュア](https://twicure.com/)」の開発。

#### 環境

- チーム規模: 8人 (フロントエンジニア 1名, バックエンドエンジニア 5名, PM 2名)
- 役割: バックエンドエンジニア
- 使用技術: Ruby, Ruby on Rails

#### 業務内容
- メイン機能となる相談機能の作成を主に担当。
  - 医師に相談機能のテーブル設計
  - 医師に相談機能の作成
  - 指名相談機能の作成
  - チャット相談機能の作成
  - お知らせ機能の作成

## やりたいこと、実現したいこと
- toC・toB問わずユーザーに価値を届けて誰かを幸せにしたい
  - 以下関心のある事業領域
    - 地方創生・地域活性化関連
    - 発展途上国・国内の貧困問題関連
    - 業務改善関連
    - 教育関連
    - 飲食・レシピ関連
    - 音楽・エンタメ関連
    - フィットネス・スポーツ関連
    - 恋愛関連
    - レガシー業界のDX

## なりたいエンジニア像
- まずは、フロントエンド領域で要件定義・設計から任せられるようになりたい。
- ゆくゆくはフロントエンド以外の技術にも守備範囲を広げていきたい。
- 将来はサブリーダー的な立ち位置で組織を支えながらプレイヤーとしても活躍したい。

## 使ってみたい技術
React.js/Next.js、Go、Firebase

## 伸ばしたいスキル
- 保守性を意識したフロント開発
- 要件定義・設計などの上流工程の開発スキル
- UI/UXを意識したフロント開発
- React.js・Angular.jsなど他JSフレームワークの開発
- FireBaseなどを使用したサーバーレスSPA開発
- RESTfulなバックエンド開発

## 言語

- 日本語
  - ネイティブ
- 英語
  - フィリピン語学学校で何とか働ける程度
  - TOEIC: 760点
