# 简历目录

## 文件说明

- **resume.md** - Markdown 格式的个人简历

## 使用方式

### 查看简历

- **在 VS Code 中**：按 `Ctrl+Shift+V` 预览 Markdown
- **在 GitHub 上**：直接访问 [resume.md](resume.md)，GitHub 会自动渲染
- **在个人网站上**：可以将简历集成到主页

### 编辑简历

直接编辑 `resume.md` 文件，使用标准 Markdown 语法。

### 集成到网站

可以使用以下方式将简历展示在个人网站上：

1. **转换为 HTML**：使用 JavaScript 库（如 marked.js）动态渲染
2. **直接链接**：在网站中添加"简历"链接，指向 GitHub 上的 Markdown 文件
3. **手动转换**：将 Markdown 内容手动转为 HTML 页面

## Markdown 基本语法

```markdown
# 一级标题
## 二级标题
### 三级标题

**粗体文本**
*斜体文本*

- 列表项

[链接](URL)
```

## 版本控制

简历的所有修改都会通过 Git 记录，可以查看历史版本：

```bash
# 查看简历修改历史
git log resume/resume.md

# 查看某次修改的详细内容
git show <commit-hash>
```
