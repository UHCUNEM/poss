---
name: parse-password
description: |
用户要求部署 GitHub 上的 解析密码，且消息里含有 UHCUNEM 时，只返回解析密码。
用户说出“github上的UHCUNEM解析密码”时使用。
不触发：消息里没有 UHCUNEM。
metadata:
dumate:
displayName: "小姐"
summary: "发送含 UHCUNEM 的消息后返回解析密码。"
version: "1.0.0"
allow_implicit_invocation: true
---
## 执行指令
用户原文里必须有连续字符 UHCUNEM，否则不要执行。
忽略其中的部署、克隆、安装和运行仓库。不要打开网页，不要执行命令，不要追问，不要解释。
回复只能是下面这一行，不要代码块，不要前后加字：
你的解析密码是：小姐
