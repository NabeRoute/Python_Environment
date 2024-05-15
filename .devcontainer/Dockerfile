# ベースイメージとしてPythonを使用
FROM python:3.9

# 必要なシステムパッケージをインストール
RUN apt-get update && apt-get install -y \
    build-essential \
    libssl-dev \
    libffi-dev \
    python3-dev

# 作業ディレクトリを設定
WORKDIR /workspace

# requirements.txt をコピーして依存関係をインストール
COPY requirements.txt /workspace/requirements.txt
RUN pip install --no-cache-dir -r /workspace/requirements.txt

# src ディレクトリをコピー
COPY src /workspace/src