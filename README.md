# IT用語説明,AWS用語説明(DMM WEBCAMP クラウド教養カリキュラムで使用・紹介している用語)
## IT 用語
### TCP/IP
#### インターネット環境の通信を実現するためのプロトコル群(通信規約)の総称。TCP/IPプロトコルスイートやインターネットプロトコルスイートと呼ばれる。

### Cookie(クッキー)
#### Web サーバーが発行し、ブラウザで保持されるテキストデータのこと。ただし、ひとつのサーバーでシステムが稼働している場合は問題無いが、
複数のサーバーで構成されているシステムでは、どこにSessionを保持するのかが課題。その場合、セッション用のデータベースを用意する、サーバー間でセッション情報を共有するなどが必要となる。

### Session(セッション)
#### 一連の処理の始まりから終わりまでを表す概念のこと。Session は、Web サーバーで保持されるデータになる。

### ロードバランサー
#### 負荷分散をするためのもので、アクセスを複数のサーバーに分割して処理ができるようになる。

### ドメイン（domain）
#### IPアドレスをわかりやすい名前に変換したもの。例：「example.com」「〜.co.jp」。

### キーペア
#### 公開鍵・秘密鍵のペアのこと。AWSではEC2にSSH接続でログインするために使用。

### JSON(JavaScript Object Notation)
#### テキストベースのデータ交換フォーマット。クライアントとサーバ間で「リクエストとレスポンス」を行うには、クライアント（人間）もサーバ（マシン）も互いに理解できるデータ形式にする必要がありその際に使用します。

### API(Application Programming Interface)
#### サービス提供者がそのサービスを利用するためのインタフェース。

### Web API	
#### WebサーバやWebブラウザ用のAPI。API提供者とAPI利用者のやり取りをWeb上で行うので、プログラミング言語が異なるアプリケーションでも連携できるのが特徴。

### DR(ディザスタリカバリ)
#### 自然災害やサイバー攻撃などでデータセンターやシステムの稼働に問題が発生した場合に損害の軽減や機能の維持、回復や復旧のための対策のこと。例：「ホットスタンバイ」「コールドスタンバイ」。

### オンプレミス
#### サーバーやネットワークなどシステムのインフラ環境を、自社保有や他社運営のデータセンター設備を借りて機器を設置し自社にて管理や運営を行う形態。自社運用とも訳される。

### CORS(Cross-Origin Resource Sharing)
#### 日本語では「オリジン間リソース共有」。対象のサイトにおいて特定サイトへの通信を許可する仕組み。


## IPアドレス
### パブリックIPアドレス
#### インターネットからアクセスすることが可能なIPアドレス。パブリックIPアドレスはインターネット上で必ず一意に割り振られる。

### プライベートIPアドレス
#### インターネットからはアクセスが不可能なIPアドレス。

### CIDR(Classless Inter-Domain Routing)
#### ネットワーク部やホスト部（IPアドレスの範囲）を決める方法の1つ。


## 使用プロトコル一覧
### TCP(Transmission Control Protocol)
#### コネクション型で信頼性のあるトランスポート層のプロトコル。

### UDP
#### コネクションレス型で信頼性のないトランスポート層のプロトコル。

### HTTP(Hyper Text Transfer Protocol)
#### ポート番号　80番ポートが標準。HTML,CSSファイル、メディアファイルなどを送受信するためのプロトコル。
「http://xxxxx.com」といったURLはHTTPで通信している。
現在では利用者の認証が必要な用途ではHTTP通信自体を丸ごと暗号化するSSL/TLSを用いるのが一般的となっており、認証機能もアプリケーション側で実装するようになったため、HTTP自体の認証機能はあまり使われなくなっている。

### HTTPS(Hypertext Transfer Protocol Secure)
#### ポート番号　443番ポートが標準。HTTP通信を TLS/SSL という仕組みで暗号化しHTML,CSSファイル、メディアファイルなどを送受信をするプロトコル。
「https://xxxxx.com」といったURLはHTTPSで通信している。

### SSH(Secure SHell)
#### ポート番号　２２番ポートが標準。暗号化技術を使い、安全に他のコンピュータを遠隔操作するためのプロトコル。主にLinuxなどのUNIX系OSで利用される。

### DNS(Domain Name System)
#### ポート番号 53番ポートを利用。ドメインをIPアドレスに変換するためのプロトコル。

### ICMP/ICMPv6(Internet Control Message Protocol)
#### 通信状態の診断を行うためのプロトコル。pingコマンド・tracerouteコマンドがこれに該当。

### ポート番号
#### ポート番号とは、コンピュータが通信を行うために通信先のアプリケーションを特定するための番号のこと。
コンピュータ間の通信で通信する宛先のIPアドレスが分かれば、そのIPアドレスにデータを送信できるが
そのデータを受信したコンピュータが、どのアプリケーションでそれを受信するのか判断するために必要。


## 使用ソフトウェア・言語
### Nginx
#### オープンソースのWebサーバー。

### Amazon Linux2	
#### AWSが提供するLinux OS。
Red Hat 7 というLinux OSをベースに作成されている。

### Node.js	
#### ブラウザ上でしか動作することが出来なかったJavaScriptをサーバー上で動かせるようにするための実行環境。
npm というパッケージ管理ツールがある。

## AWS用語
### リージョン
#### AWSがサービスを提供しているエリア（国・地域）のこと。
各リージョンは、他のリージョンと完全に分離されるように設計されている。これにより、最大限の耐障害性と安定性が達成される。

