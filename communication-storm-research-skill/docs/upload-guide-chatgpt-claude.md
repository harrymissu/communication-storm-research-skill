# 上载到 ChatGPT 和 Claude 的最简单路径

## 1. ChatGPT Project 路径

适合个人或课程组重复使用。

1. 打开 ChatGPT。
2. 新建 Project。
3. 将 `prompts/chatgpt-project-instructions.md` 粘贴到 Project instructions。
4. 上传以下文件：
   - `SKILL.md`
   - `README.md`
   - `templates/*.md`
   - `examples/*.md`
   - `docs/references.md`
5. 在项目中输入：

```text
请用传播学 STORM 方法分析我的论文题目：【题目】
```

## 2. Custom GPT 路径

适合想做成一个可分享工具的老师或课程团队。

1. 进入 GPTs → Create。
2. 在 Configure / Instructions 中粘贴 `prompts/chatgpt-project-instructions.md`。
3. 在 Knowledge 中上传本文件夹内的 Markdown 文件。
4. 开启 Web Search。
5. 如需处理问卷数据，开启 Code Interpreter & Data Analysis。
6. 在 Preview 中测试后保存。

注意：OpenAI 官方建议把行为规则写在 Instructions 中，把文件作为 Knowledge 参考资料。

## 3. Claude Code 路径

适合愿意在本地/代码环境中使用 Skill 的用户。

macOS / Linux：

```bash
mkdir -p ~/.claude/skills
cp -R communication-storm-research-skill ~/.claude/skills/communication-storm-research
```

然后重启 Claude Code，输入：

```text
当前可用 Skills 有哪些？
```

确认已识别后，即可使用：

```text
请用 communication-storm-research skill 分析这个传播学论文题目：……
```

## 4. Claude.ai / Claude Project 替代路径

如果账号没有 Skills 安装入口：

1. 新建 Claude Project。
2. 上传 `SKILL.md`、`README.md`、`prompts`、`templates`、`examples`。
3. 将 `prompts/master-prompt.md` 作为项目默认指令。
4. 每次在项目中输入论文题目即可。

## 5. 使用边界

- 不上传学生隐私信息。
- 不上传未脱敏访谈原文。
- 不上传未公开数据。
- 不要求 AI 代写最终论文。
- 所有文献引用必须由学生自行核实。
