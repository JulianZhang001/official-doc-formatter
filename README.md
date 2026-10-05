
<div align="center">

**把公文 Word 排版交给脚本，30 秒出规范件。**
依据 GB/T 9704-2012 自动调整版式、规范标点，输出规范 Word + 修改报告。

`本地运行 · 浏览器操作 · 不上传任何文档`

</div>

---

# 公文 Word 自动校排工具

本仓库整理的是一个本地可运行的 Word 公文自动校排程序。用户上传 Word 后，程序会依据国家标准自动调整公文版式、规范常见标点，并输出规范版 Word 与修改报告。

## 标准依据

- GB/T 9704-2012《党政机关公文格式》
- GB/T 15834-2011《标点符号用法》

## 项目内容

- `official_doc_formatter/`：可运行程序源码。
- `official_doc_formatter/README.md`：运行方式与功能说明。
- `official_doc_formatter/docs/standards/`：国家标准依据文件。
- `公文Word自动校排程序设计方案.md`：需求、架构、规则、模块和开发路线。

## 快速启动

```bash
cd official_doc_formatter
python3 -m pip install -r requirements.txt
python3 run_server.py
```

打开浏览器访问：

```text
http://127.0.0.1:8765
```

## 说明

仓库默认不提交用户上传的 Word 文档、申报材料、处理输出文件和本地缓存，避免把业务材料或个人文件误传到代码仓库。

---

## 许可

MIT © 山城_居老师

## 适用场景

- 机关、学校、国企公文起草后的格式规范化
- 批量文档格式检查，避免逐份手调行距字号
- 教学演示：现场展示公文国标是怎么落地的

## 反馈

问题和建议请提交 [issue](https://github.com/JulianZhang001/official-doc-formatter/issues)。
