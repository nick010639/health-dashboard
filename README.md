# 健康仪表板

显示 health agent 的健康跟踪数据。

## 访问地址

- 线上：https://health.aiwinner.top
- GitHub：https://github.com/nick010639/health-dashboard

## 技术栈

- 前端：原生 HTML/CSS/JS，单文件
- 数据存储：Supabase Database
- 部署：Vercel + Cloudflare 代理

## 功能

- 当前体重 vs 目标体重对比
- 今日饮食记录
- 本周运动统计
- 体重趋势折线图（最近14天）
- 自动从 Supabase 读取最新数据

## 开发

```bash
# 本地预览
cd dashboard
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080
```

## 部署

代码推送到 GitHub `nick010639/health-dashboard` 仓库后，Vercel 自动部署。

## 数据同步

- 每日早上 9 点自动同步（cron job）
- 也可手动点击"今日日期"按钮刷新
