# Golang
Go言語/GOBOT　環境構築

※構築環境のOSはUbuntu18.04

※ベース環境やアップデートにより版数やコマンドが変わる可能性あります

----
■golangインストール
----

$ sudo apt-get update

（Linuxの最新版をダウンロード）
https://golang.org/dl/

$ wget https://dl.google.com/go/go1.11.2.linux-amd64.tar.gz

$ sudo tar -C /usr/local -xzf go1.11.2.linux-amd64.tar.gz

$ echo '# golang'                            >> ~/.bashrc

$ echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc

$ source ~/.bashrc

$ go version

⇒go version go1.11.2 linux/amd64

----
■gobotインストール
----

https://gobot.io/documentation/platforms/tello/

$ sudo apt-get install git

$ cd 

$ go get -d -u gobot.io/x/gobot/...

----

$ ソースファイル作成

$ go build "ファイル名.go"

$ ./"実行ファイル"

または

$ go run   "実行ファイル"

----
