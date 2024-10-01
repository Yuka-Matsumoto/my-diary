# frontend/Dockerfile
FROM node:18-alpine

# 作業ディレクトリを設定
WORKDIR /app

# パッケージをインストール
COPY package*.json ./
RUN npm install

# ソースコードをコピー
COPY . .

# 開発用サーバーを起動
CMD ["npm", "run", "dev"]

# ホットリロードを有効化
EXPOSE 3000
