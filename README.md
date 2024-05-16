
# Dockerを用いたPythonの環境構築

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
```

## 環境の使い方

### 1. リポジトリのクローン

最初に、GitHubリポジトリをローカルにクローンします。

1. **VSCodeを開く**。
2. **コマンドパレットを開く** (`Ctrl+Shift+P`)。
3. **「Git: Clone」を選択**。
4. **リポジトリURLを入力**してクローン。
5. **クローンしたフォルダーを開く**。

### 2. 「Reopen in Container」でコンテナをビルド・起動

1. **VSCodeでクローンしたプロジェクトを開く**。
2. **コマンドパレットを開く** (`Ctrl+Shift+P`)。
3. **「Remote-Containers: Reopen in Container」を選択**。
4. 自動的に `.devcontainer` ディレクトリ内の `devcontainer.json` ファイルを使用してコンテナをビルドし、起動します。

### 3. 環境の確認と開発の開始

VSCodeでコンテナに接続後、以下の操作を行います。

1. **ターミナルを開く** 
2. ターミナルで次のコマンドを実行して、Pythonが正しくインストールされていることを確認します。

    ```bash
    python --version
    ```

3. 必要なPythonパッケージがインストールされていることを確認します。

    ```bash
    pip list
    ```

4. **`src/main.py`** を開いて、次のコマンドでスクリプトを実行します。

    ```bash
    python src/main.py
    ```

---






