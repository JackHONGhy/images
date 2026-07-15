# images

GitHub 图床仓库，配合 [jsDelivr](https://www.jsdelivr.com/) CDN 使用。

## 上传图片

1. 打开仓库：https://github.com/JackHONGhy/images
2. 进入 `img/` 文件夹（或直接在根目录）
3. 点击 **Add file** → **Upload files**
4. 拖入图片，填写 commit 信息后点击 **Commit changes**

## jsDelivr 链接格式

```
https://cdn.jsdelivr.net/gh/JackHONGhy/images@main/图片路径
```

### 示例

| 文件位置 | jsDelivr 链接 |
|----------|---------------|
| `img/logo.png` | `https://cdn.jsdelivr.net/gh/JackHONGhy/images@main/img/logo.png` |
| `banner.jpg` | `https://cdn.jsdelivr.net/gh/JackHONGhy/images@main/banner.jpg` |

### 在网页中使用

```html
<img src="https://cdn.jsdelivr.net/gh/JackHONGhy/images@main/img/logo.png" alt="logo">
```

```markdown
![logo](https://cdn.jsdelivr.net/gh/JackHONGhy/images@main/img/logo.png)
```

## 固定版本（推荐生产环境）

用 Git tag 固定版本，避免更新后链接变化或缓存问题：

```
https://cdn.jsdelivr.net/gh/JackHONGhy/images@v1.0.0/img/logo.png
```

在 GitHub 仓库 **Releases** 或 **Tags** 中创建 tag 即可。

## 注意事项

- 仓库必须为 **公开**，jsDelivr 才能访问
- 新上传的图片可能需要几分钟才能在全球 CDN 生效
- 建议图片放在 `img/` 目录，便于管理
- 单文件建议不超过 20MB