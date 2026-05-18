# my-blog
Personal technology blog built with Hexo and Stellar.
# JingweiYan's Blog

基于 Hexo + Stellar 的个人博客项目。

## 技术栈

- Hexo 8
- hexo-theme-stellar
- GitHub Pages

## 本地开发

安装依赖：

```bash
npm install
```

启动本地服务：

```bash
npm run server
```

访问：

```text
http://localhost:4000/my-blog/
```

## 构建

```bash
npm run build
```

等价于：

```bash
hexo generate
```

## 部署

当前站点配置：

```yaml
url: https://jingweiyan813-gif.github.io/my-blog
root: /my-blog/
theme: stellar
```

推送到 `main` 分支后，GitHub Actions 会自动构建并部署 `public/` 到 GitHub Pages。

## 目录说明

- `_config.yml`：Hexo 主配置
- `_config.stellar.yml`：Stellar 主题配置
- `source/_posts/`：博客文章
- `source/img/avatar.png`：站点头像
- `source/css/stellar-custom.css`：少量自定义样式
- `.github/workflows/pages.yml`：GitHub Pages 自动部署流程

## 注意

- 不提交 `node_modules/`
- 不提交 `public/`
- 不提交 `db.json`
- 当前项目只保留 Stellar 主题版本
