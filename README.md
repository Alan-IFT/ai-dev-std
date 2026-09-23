# ai-dev-std

AI 辅助开发的项目管理标准与机械检查器。内容只有三个目录加一个插件清单目录，与维护仓 `main` 上同名目录逐字一致：

- `标准/` 四章正文、覆盖与采用检查、参考资料卡、示例项目
- `templates/` 载体实例模板
- `tools/std/` 检查器与契约（`python3 .std/tools/std/check_all.py .`）
- `.claude-plugin/` Claude Code 插件清单：把内嵌的 `.std/` 当插件加载，接法见 `tools/std/README.md`「Claude Code 拦截层」

本仓是发布产物，不在这里修改任何内容。`main` 永远指向最新发布；每个发布提交另打一个 tag，要钉某一版把下面命令里的 `main` 换成 tag 名。

**取用**（在采用项目根执行一次，原样复制）：

```
git subtree add --prefix=.std https://github.com/Alan-IFT/ai-dev-std.git main --squash
```

**升级**（原样复制）：

```
git subtree pull --prefix=.std https://github.com/Alan-IFT/ai-dev-std.git main --squash
```

拉到的是哪一版：`.std/标准/README.md` 第 3 行的修订号，写进项目的 `governance/STANDARD_VERSION`。升级前的越界检测与读差异步骤见 `tools/std/README.md` 「接入一个项目」。

**许可**：`标准/`、`templates/` 为 CC BY 4.0（`LICENSE-DOCS`），`tools/std/` 及代码为 MIT（`LICENSE`）。引用的第三方材料版权归原作者。

| tag | 来自 main |
|---|---|
| `2026-09-13` | `f355c1f`（首个公开发布） |
| `2026-09-13.1` | `330c8e6` |
| `2026-09-13.2` | `732bd73` |
| `2026-09-13.3` | `080c444` |
| `2026-09-21` | `d4f14f7` |
| `2026-09-22` | `411a2f5` |
| `2026-09-22.1` | `68d85c2` |
| `2026-09-22.2` | `74ee0d0` |
| `2026-09-22.3` | `15407ba` |
| `2026-09-22.4` | `1869148` |
| `2026-09-23` | `846d876` |
| `2026-09-23.1` | `777579c` |
| `2026-09-23.2` | `115eae9` |
