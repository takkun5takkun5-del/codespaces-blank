# デスクトップ環境付きのベースイメージを使う
FROM mcr.microsoft.com/devcontainers/universal:2

# ルート権限でChromiumとNetsurfを自動インストールする設定
USER root
RUN apt-get update && apt-get install -y \
    chromium \
    netsurf-gtk \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# ユーザーを元に戻す
USER codespace