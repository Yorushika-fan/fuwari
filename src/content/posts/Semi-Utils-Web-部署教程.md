---
title: Semi-Utils-Web 部署教程
published: 2025-12-22
description: '一个强大的在线图片处理工具，支持 RAW 格式、批量处理、水印添加等功能。详细介绍 Semi-Utils-Web 的部署流程和配置方法'
image: ''
tags: [Semi-Utils-Web, 部署, 教程, Docker, 图片处理]
category: '教程'
draft: false 
lang: 'zh_CN'
---

# Semi-Utils-Web 部署教程

> 一个强大的在线图片处理工具，支持 RAW 格式、批量处理、水印添加等功能。

## 🚀 使用 Docker Compose 部署

### 1. 创建 docker-compose.yml 文件

创建一个 `docker-compose.yml` 文件：

```yaml
services:
  backend:
    image: yorushikafan/semi-utils-web-backend:latest
    container_name: semi-utils-backend
    ports:
      - "8000:8000"
    volumes:
      - sessions_data:/app/sessions
    environment:
      - LOG_LEVEL=INFO
    restart: unless-stopped
    healthcheck:
      test: ["CMD", "curl", "-f", "http://localhost:8000/health"]
      interval: 30s
      timeout: 10s
      retries: 3

  frontend:
    image: yorushikafan/semi-utils-web-frontend:latest
    container_name: semi-utils-frontend
    ports:
      - "80:80"
    depends_on:
      - backend
    restart: unless-stopped

volumes:
  sessions_data:
```

### 2. 启动服务

```bash
docker compose up -d
```

### 3. 访问应用

打开浏览器访问 `http://localhost` 即可使用。

---

## 📸 部署截图


![Semi-Utils-Web](https://pic.250996007.xyz/api/images/f9459cee-a57f-4ebe-81a6-d66c91589952)

![效果图](https://pic.250996007.xyz/api/images/75967c73-6534-4009-a1db-a9a4fc68f3b5)
