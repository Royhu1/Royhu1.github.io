# 个人网站 - Royhu1.github.io

[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue)](https://royhu1.github.io)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 项目简介

这是一个基于 GitHub Pages 托管的个人网站项目，展示个人简历、项目作品和技术博客。

**网站地址**: https://royhu1.github.io

## 项目结构

```
Royhu1.github.io/
├── index.html          # 网站主页
├── css/                # 样式文件目录
├── js/                 # JavaScript 文件目录
├── images/             # 图片资源目录
├── resume/             # 简历目录
│   └── resume.md       # Markdown 格式简历
├── projects/           # 项目展示页面
├── blog/               # 博客文章目录
├── CLAUDE.md           # Claude Code 开发指引
└── README.md           # 项目说明文档
```

## 功能规划

### 已完成
- [x] 初始化 GitHub Pages 仓库
- [x] 创建基础 index.html
- [x] 创建项目文件夹结构
- [x] 添加 Markdown 格式简历

### 待开发
- [ ] 设计响应式布局
- [ ] 创建个人简介页面
- [ ] 添加项目展示模块
- [ ] 集成博客系统
- [ ] 添加联系方式表单
- [ ] 优化 SEO
- [ ] 添加深色模式支持
- [ ] 多语言支持（中/英）

## 技术栈

- **前端框架**: 纯 HTML/CSS/JavaScript（或根据需求选择框架）
- **托管平台**: GitHub Pages
- **版本控制**: Git
- **开发工具**: VS Code + Claude Code

## 本地开发

### 环境要求

- Git
- 本地 Web 服务器（推荐使用以下任一方式）

### 启动本地服务器

**方式一：使用 Python**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**方式二：使用 Node.js**
```bash
# 安装 http-server（仅需一次）
npm install -g http-server

# 启动服务器
http-server . -p 8000
```

**方式三：使用 VS Code 插件**
- 安装 "Live Server" 插件
- 右键 index.html，选择 "Open with Live Server"

访问 http://localhost:8000 查看网站效果。

## 部署流程

1. **提交代码到 GitHub**
   ```bash
   git add .
   git commit -m "描述你的修改内容"
   git push origin main
   ```

2. **自动部署**
   - GitHub Pages 会自动构建并部署
   - 通常在 1-2 分钟内生效
   - 访问 https://royhu1.github.io 查看更新

3. **检查部署状态**
   - 进入仓库设置 → Pages
   - 查看 "Your site is live at..." 状态

## 开发规范

### 代码风格
- HTML: 使用语义化标签，保持结构清晰
- CSS: 采用 BEM 命名规范
- JavaScript: 使用 ES6+ 语法，添加必要注释

### 文件编码
- 统一使用 **UTF-8** 编码
- 确保跨平台兼容性

### Git 提交规范
```
feat: 新功能
fix: 修复问题
docs: 文档更新
style: 样式调整
refactor: 代码重构
perf: 性能优化
test: 测试相关
chore: 构建/工具配置
```

## 内容规划

### 主页 (index.html)
- Hero 区域：个人介绍 + 头像
- 技能展示
- 项目精选
- 联系方式

### 项目页面
- 项目列表
- 详细介绍
- 技术栈说明
- 在线演示链接

### 博客模块
- 技术文章
- 学习笔记
- 经验分享

## 待办事项

### 近期任务
1. 修复 index.html 文件编码问题（UTF-16 → UTF-8）
2. 设计网站整体布局和配色方案
3. 创建响应式导航栏
4. 添加个人简介内容

### 中期任务
1. 开发项目展示页面
2. 集成第三方服务（如 Google Analytics）
3. 添加社交媒体链接
4. 优化移动端体验

### 长期任务
1. 实现博客系统（可考虑集成 Jekyll）
2. 添加评论功能
3. 国际化支持
4. 性能优化和 SEO

## 资源链接

- [GitHub Pages 官方文档](https://docs.github.com/en/pages)
- [HTML/CSS 最佳实践](https://www.w3schools.com/)
- [响应式设计指南](https://developer.mozilla.org/zh-CN/docs/Learn/CSS/CSS_layout/Responsive_Design)
- [SEO 优化指南](https://developers.google.com/search/docs)

## 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 联系方式

- GitHub: [@Royhu1](https://github.com/Royhu1)
- Email: [你的邮箱]

---

**最后更新**: 2025-10-08

**开发状态**: 🚧 建设中
