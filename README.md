# Dockerを用いたpythonの環境構築

VSCodeとDockerを使用してPythonの開発環境をセットアップする方法を示します。  
この環境は以下の要件を満たしています：

1. **VSCodeのUIでコンテナをビルド・起動する**
2. **VSCodeのUIでコンテナ内のソースコード編集やスクリプトの実行を行う**
3. **devcontainer と Docker を使用する**

## ディレクトリ構造

```plaintext
project-root/
├── .devcontainer/
│   ├── Dockerfile
│   └── devcontainer.json
├── src/
│   └── main.py
└── requirements.txt






