# Golang
Go言語　環境構築Tips


※構築環境はUbuntu14.04/2018年6月/
　ベース環境やアップデートにより版数やコマンドが変わる可能性あります

$ sudo apt-get update
https://golang.org/dl/（Linuxの最新版をダウンロード）

$ wget https://dl.google.com/go/go1.10.3.linux-amd64.tar.gz

$ sudo tar -C /usr/local -xzf go1.10.3.linux-amd64.tar.gz

$ echo '# golang'                            >> ~/.bashrc

$ echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc

$ source ~/.bashrc

$ go version

⇒go version go1.10.3 linux/amd64

https://gobot.io/documentation/platforms/tello/

$ cd 

$ go get -d -u gobot.io/x/gobot/...

https://gobot.io/documentation/platforms/joystick/

$ wget https://www.libsdl.org/release/SDL2-2.0.8.tar.gz

$ tar -zxvf SDL2-2.0.8.tar.gz

$ cd SDL2-2.0.8/

$ ./configure && make && sudo make install

⇒MplayerはUbuntuソフトウェアセンターからインストールして下さい

$ sudo apt-get install ubuntu-restricted-extras

⇒選択があるので、"はい"で問題ないです

ファイル配置してgoフォルダへ上書き展開
$ cd

$ tar tvfz tello_project.tar.gz

$ tar xvfz tello_project.tar.gz

$ go build "ファイル名.go"


■参考
・tello_project.tar.gzを固めるとき
$ tar cvfz tello_project.tar.gz go/src/*.go go/src/gobot.io/x/gobot/platforms/joystick/joystick_dualshock3.go 
