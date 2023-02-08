FROM node:16.0.0
WORKDIR /app/react

# # package.jsonとyarn.lockを/usr/src/appにコピー
COPY ["frontend/package.json", "frontend/yarn.lock", "app/react/"]
# パッケージをインストール
RUN yarn install
# ファイルを全部作業用ディレクトリにコピー
COPY frontend/ app/react/
# コンテナを起動する際に実行されるコマンド
ENTRYPOINT [ "yarn", "start" ]