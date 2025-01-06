# 使用 Python 作為基礎映像
FROM python:3.10

# 設定工作目錄為 /app
WORKDIR /app

# 複製所有檔案到工作目錄
COPY . ./

# 開放 3015 埠號
EXPOSE 3015

# 設定容器啟動時執行的命令
CMD ["python3", "rng.py"]