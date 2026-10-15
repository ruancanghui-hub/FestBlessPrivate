# FestBlessPrivate

「节日祝福」App Store Connect 用法律与支持页，通过 GitHub Pages 发布。

## 启用后 URL

| 用途 | URL |
|------|-----|
| 隐私政策 | https://ruancanghui-hub.github.io/FestBlessPrivate/privacy/ |
| 用户协议 / EULA | https://ruancanghui-hub.github.io/FestBlessPrivate/terms/ |
| 支持 | https://ruancanghui-hub.github.io/FestBlessPrivate/support/ |
| 首页 | https://ruancanghui-hub.github.io/FestBlessPrivate/ |

## 启用 GitHub Pages

1. 仓库 **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: `main`，文件夹：`/ (root)`
4. 保存，等待 1–2 分钟后打开上方隐私政策 URL

或 CLI：

```bash
gh api repos/ruancanghui-hub/FestBlessPrivate/pages \
  -X POST \
  -f "build_type=legacy" \
  -f "source[branch]=main" \
  -f "source[path]=/"
```

## App Store Connect 填写

- **Privacy Policy URL** → `/privacy/`
- **Terms of Use / EULA（自定义）** → `/terms/`
- **Support URL** → `/support/`

App 内「隐私政策」「用户协议」链接已指向上述 Pages 地址。
