# 天青之韵 · 汝瓷官网

汝窑主题的纯静态展示站，React 19 + Vite 7 + Tailwind v4。和 [`ru-porcelain-web`](https://github.com/songdaochuanshu/ru-porcelain-web) 同源，这一份是最初的官网版本。

## 技术栈

React 19 + TypeScript · Vite 7 · Tailwind CSS v4 · wouter · lucide-react

## 本地开发

```bash
pnpm install
pnpm dev        # http://localhost:3000
pnpm build      # 产物在 dist/public
pnpm preview
pnpm check      # tsc --noEmit
```

## 部署

```bash
pnpm build
npx wrangler pages deploy dist/public --project-name ru-porcelain-showcase
```

## 状态

这个仓库没有配置 `wrangler.toml`，也没有接 Pages 项目，README 早期的演示地址已经失效——**当前没有线上部署**。如果想恢复，按上面的命令建一个 Pages 项目即可（构建命令 `pnpm build`，输出目录 `dist/public`）。

## 变更记录

- 2026-10-25：移除 Manus WebDev 模板残留（内联 React 运行时插件、调试日志收集器、`/manus-storage` 代理、express 服务端、`__manus__` 收集脚本），构建脚本改为纯 `vite build`；补 README 与 MIT LICENSE。

## License

[MIT](./LICENSE)
