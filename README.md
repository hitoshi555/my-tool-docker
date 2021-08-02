# my-tool-docker

## 作った理由

Zoom などでミーティングしている時に図で説明したいがマウス操作で図を書くのに慣れなかったため手元にある ipad と apple pencil を利用したかったから。

## 使用言語・技術

docker  
react  
nest.js  
typescript  
socket.io  
material-ui  
ngrok

## my-tool-react と my-tool-nest の配置

それぞれのボリュームがファイル直下に繋がっているため my-tool-react と my-tool-nest をファイル直下に配置する。  
ファイルは以下の形になる。

```
.
├── .gitignore
├── Dockerfile.backend
├── Dockerfile.frontend
├── README.md
├── my-tool-react
└── my-tool-backend
```

## 使い方

以下のコマンドで Docker を立ち上げる。

```
$ docker-compose build
$ docker-compose up
```

ngrok で外部に公開する。  
設定は以下 url 参照。  
[qiita](https://qiita.com/reona396/items/d7a7958b68d738f7c56e)

```
$ ./ngrok start http wss
```

Ngrok で立ち上がった nest.js 用ポートを react の socket.io に繋げる。

iPad に url を共有して使用する。
