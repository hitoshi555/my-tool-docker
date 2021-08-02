# my-tool-docker

## 作った理由

Zoom などでミーティングしている時に図で説明したいがマウス操作で図を書くのになれず手元にある ipad と apple pencil を使いたかったから。

## my-tool-react と my-tool-nest の配置

ボリュームがファイル直下に繋がっているため my-tool-react と my-tool-nest をファイル直下に配置する。  
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
