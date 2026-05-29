# X 黄推屏蔽器 - Grok 对话上下文

> **下次想继续这个项目时，直接把下面这段文字复制给 Grok 即可：**

```
我在做一个叫「X 黄推屏蔽器」的 Chrome 扩展，仓库地址是：
https://github.com/weixunkkkkk/x-huangtui-blocker

本地路径：/Users/mac/Developer/x-huangtui-blocker

请先阅读仓库根目录的 GROK_CONTEXT.md 文件，了解当前项目状态和上下文，然后再继续帮我。
```

---

**项目地址**: https://github.com/weixunkkkkk/x-huangtui-blocker  
**本地路径**: `/Users/mac/Developer/x-huangtui-blocker`  
**最后更新**: 2026-05-29

---

## 项目简介

这是一个基于 [X Focus Filter](https://github.com/vorojar/x-focus-filter) 二次开发的 Chrome 扩展，主要目标是**针对中文用户强力屏蔽 X（Twitter）上的黄推、福利推广、车牌、裸聊等内容**。

核心定位：**中文黄推杀手**，而非原版的“专注科技内容”。

---

## 当前状态（2026-05-29）

### 已完成
- Fork X Focus Filter 并创建独立仓库
- 大幅扩充中文黄推黑名单（`content.js` 中的 `BLACKLIST`）
- 更新 `manifest.json` 名称和描述为「X 黄推屏蔽器」
- 重写 `README.md`（中文为主）
- 生成并更新符合 Web Store 规范的图标（16/48/128）
- 准备 Chrome Web Store 上架材料：
  - 名称、简短描述、详细描述（中英文）
  - 隐私政策
  - Host 和 Storage 权限理由说明
- 生成多张模拟截图（已处理成 1280x800）
- 完成 GitHub 首次推送

### 重要文件位置
- `content.js`：核心过滤逻辑 + 强力黑名单
- `manifest.json`：扩展配置
- `icons/`：已符合规范的图标
- `GROK_CONTEXT.md`：本文件（重要上下文）

---

## 与 Grok 继续对话的推荐方式

下次想继续这个项目时，**最有效的方式**是：

### 最佳方式（强烈推荐）：
1. 打开这个 GitHub 仓库：https://github.com/weixunkkkkk/x-huangtui-blocker
2. 新建一个对话时，直接把下面这句话复制粘贴给 Grok：

```
我在做一个叫「X 黄推屏蔽器」的 Chrome 扩展，基于 X Focus Filter 二次开发，目标是强力屏蔽中文黄推。

项目仓库：https://github.com/weixunkkkkk/x-huangtui-blocker
本地路径：/Users/mac/Developer/x-huangtui-blocker

请先阅读仓库根目录的 GROK_CONTEXT.md 文件，了解当前状态和上下文，然后再继续帮我处理。
```

3. Grok 看到 `GROK_CONTEXT.md` 后，会快速理解项目背景。

---

## 下次可能需要做的事情（待办）

- [ ] 完善并上传真实的屏幕截图（目前主要用模拟图）
- [ ] 填写 Chrome Web Store 的权限理由（Host + Storage）
- [ ] 完成 Privacy practices 部分
- [ ] 验证并填写开发者联系邮箱
- [ ] 打包最终干净的 ZIP 并上传
- [ ] 考虑是否要改默认行为（目前为了测试关闭了正向过滤）
- [ ] 继续优化黑名单（根据实际使用反馈补充关键词）

---

## 重要决策记录

- 项目采用 **Fork + 重度定制** 路线，而不是从零写。
- 默认行为暂时偏向“激进屏蔽黄推”（关闭了原版的 Tech/AI 类别过滤）。
- 图标和截图都按照 Chrome Web Store 严格要求处理过。
- 所有上架相关文案都已准备好中英文版本。

---

## 联系方式 / 备注

- GitHub: weixunkkkkk
- 本地开发主要路径：`/Users/mac/Developer/x-huangtui-blocker`
- 打包时请使用干净 ZIP（排除 .git、.spec-workflow 等）

---

**提示**：以后每次重要修改后，建议更新本文件的时间和状态，方便下次快速接上。