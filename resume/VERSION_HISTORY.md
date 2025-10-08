# Resume Version History

## 版本命名规则

格式：`resume_v{major}.{minor}_{YYYY-MM-DD}.md`

- **Major version (主版本)**: 重大内容变更（如新增学位、重要职位变更）
- **Minor version (次版本)**: 小幅更新（如新增项目、技能更新）
- **Date (日期)**: 更新日期 YYYY-MM-DD

## 版本列表

### v1.1 - 2025-10-08
**变更内容**：
- ✅ 新增 Teaching Experience 部分
- ✅ 添加 Lab Demonstrator (3C8) 职位
  - Department of Engineering, University of Cambridge
  - Oct 2024 - Present
  - 实验室指导、学生支持、实践教学

**文件**：`versions/resume_v1.1_2025-10-08.md`

---

### v1.0 - 2024-10-08
**初始版本**

**包含内容**：
- Education Background (PhD, Master's, Bachelor's)
- Research Experience (3 项主要研究)
- Industrial Project Experience (2 个项目)
- Work Experience (Software Engineer Intern)
- Skills (Programming, Deep Learning, Communication)
- Publications (4 篇)
- Patents (2 项)
- Prizes and Awards (4 项)
- Activities (会议、篮球协会、志愿者)

**文件**：`versions/resume_v1.0_2024-10-08.md`

---

## 更新建议

### 何时更新主版本 (Major Version)
- 获得新学位
- 开始新的正式职位
- 重大职业转变
- 完成重要里程碑

### 何时更新次版本 (Minor Version)
- 新增研究项目
- 发表新论文
- 获得新奖项
- 新增技能或证书
- 更新项目描述

### 最佳实践

1. **定期备份**
   - 每次重大更新前先备份当前版本
   - 使用明确的版本号和日期

2. **保持主文件最新**
   - `resume.md` 始终是最新版本
   - 历史版本保存在 `versions/` 文件夹

3. **记录变更**
   - 在此文件中记录每次更新的内容
   - 便于追溯和对比

4. **Git 版本控制**
   - 配合 Git commit 使用
   - 提供双重版本保障

## 快速更新流程

```bash
# 1. 备份当前版本
cp resume.md versions/resume_v{X}.{Y}_{DATE}.md

# 2. 编辑 resume.md

# 3. 更新本文件 (VERSION_HISTORY.md)

# 4. Git 提交
git add resume/
git commit -m "docs: Update resume to v{X}.{Y}"
git push
```

## 文件结构

```
resume/
├── resume.md                          # 当前最新版本
├── README.md                          # 使用说明
├── VERSION_HISTORY.md                 # 本文件 - 版本历史
└── versions/                          # 历史版本存档
    ├── resume_v1.0_2024-10-08.md     # 初始版本
    ├── resume_v1.1_2025-10-08.md     # 添加教学经历
    └── ...                            # 未来版本
```

---

**最后更新**: 2025-10-08
**当前版本**: v1.1
