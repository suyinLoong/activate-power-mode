# activate-power-mode

- [power mode](https://github.com/codeinthedark/editor/pull/1) script for any website
- used [textarea-caret-position library](https://github.com/component/textarea-caret-position).
- [demo](https://cloud.githubusercontent.com/assets/688415/11440971/aadfae8e-9507-11e5-8aa0-0ecc87ca84b6.gif)


## 如何使用

```html
<script src="https://cdn.jsdelivr.net/gh/suyinLoong/activate-power-mode@1.2/dist/activate-power-mode.js"></script>
<script>
    POWERMODE.colorful = true; // 让特效呈现彩色
    POWERMODE.shake = false;   // 关闭屏幕抖动
    document.body.addEventListener('input', POWERMODE);
</script>
```

## 在Hexo Next主题上使用

1.[Hexo](https://hexo.io/) 配置

- 在 `/Hexo/source/` 目录下新建 `_data` 目录
- 在 `_data` 目录下新建 `bodyEnd.njk` 文件夹
- 在文件夹中写入以下代码：
  ```njk
  <script src="https://cdn.jsdelivr.net/gh/suyinLoong/activate-power-mode@1.2/dist/activate-power-mode.js"></script>
  <script>
      POWERMODE.colorful = true; // 让特效呈现彩色
      POWERMODE.shake = false;   // 关闭屏幕抖动
      document.body.addEventListener('input', POWERMODE);
  </script>
  ```

2.[Next](https://github.com/next-theme/hexo-theme-next) 配置

- 在 Next 配置文件中找到 `custom_file_path:`
- 取消 `bodyEnd: source/_data/body-end.njk` 的注释

