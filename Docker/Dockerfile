# 使用 scratch 或 alpine 作为基础镜像
FROM alpine

# 设置工作目录
WORKDIR /app

# 复制构建好的二进制文件（来自 GitHub Actions 构建步骤）
COPY jsrpc /app/jsrpc

# 设置可执行权限
RUN chmod +x /app/jsrpc

# 暴露端口（如果应用监听端口）
EXPOSE 12080

# 启动命令
ENTRYPOINT ["./jsrpc"]