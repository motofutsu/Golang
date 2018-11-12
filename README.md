# Golang
Go言語　環境構築Tips


※構築環境はUbuntu14.04/2018年6月/
　ベース環境やアップデートにより版数やコマンドが変わる可能性あります

----
■golangインストール

$ sudo apt-get update

https://golang.org/dl/（Linuxの最新版をダウンロード）

$ wget https://dl.google.com/go/go1.10.3.linux-amd64.tar.gz

$ sudo tar -C /usr/local -xzf go1.10.3.linux-amd64.tar.gz

$ echo '# golang'                            >> ~/.bashrc

$ echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc

$ source ~/.bashrc

$ go version

⇒go version go1.10.3 linux/amd64

----
■gobotインストール

https://gobot.io/documentation/platforms/tello/

$ sudo apt-get install git

$ cd 

$ go get -d -u gobot.io/x/gobot/...

$ ソースファイル作成

$ go build "ファイル名.go"

$ ./"実行ファイル"

または

$ go run   "実行ファイル"

----
