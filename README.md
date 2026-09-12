# ai-dev-std

AI 辅助开发的项目管理标准与机械检查器。内容只有三个目录，与维护仓 `main` 上同名目录逐字一致：

- `标准/` 四章正文、覆盖与采用检查、参考资料卡、示例项目
- `templates/` 载体实例模板
- `tools/std/` 检查器与契约（`python .std/tools/std/check_all.py .`）

本仓是发布产物，不在这里修改任何内容。每个发布提交打一个 tag，tag 名就是采用项目写进 `governance/STANDARD_VERSION` 的值（日期，同日再发加 `.1`、`.2`）。

**取用**（在采用项目根执行一次）：

```
git subtree add --prefix=.std https://github.com/Alan-IFT/ai-dev-std.git <tag> --squash
```

**升级**：同一条命令把 `add` 换成 `pull`，其余参数不变；`.std/` 不存在用 add，存在用 pull。可选一行本机 git alias 让 `git std <tag>` 兼做两者，见 `tools/std/README.md` 「接入一个项目」，那里也有升级前的越界检测与读差异步骤。

**许可**：`标准/`、`templates/` 为 CC BY 4.0（`LICENSE-DOCS`），`tools/std/` 及代码为 MIT（`LICENSE`）。引用的第三方材料版权归原作者。

| tag | 来自 main |
|---|---|
| `2026-09-13` | `f355c1f`（首个公开发布） |
| `2026-09-13.1` | `330c8e6` |
