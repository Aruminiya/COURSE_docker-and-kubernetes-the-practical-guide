# 使用 Node.js 14 作為基礎映像
FROM node:14

# 設定工作目錄為 /app
WORKDIR /app

# 複製 package.json 到工作目錄
COPY package.json .

# 執行 npm install 安裝相依套件
RUN npm install

# 複製所有檔案到工作目錄
COPY . .

# 開放 3000 埠號
# 這行是告訴 Docker 容器，我們希望能夠從外部連接到這個應用程式 而不僅僅是在容器內部，需要使用 3000 埠號
EXPOSE 3000

# 設定容器啟動時執行的命令
CMD ["node", "app.mjs"]