# @shuiyangsuan/tsconfig

为 TypeScript 应用提供可复用的 TSConfig 配置，针对不同运行时环境优化。

## 设计原则
- 使用最新的语言标准和特性
- 与最新 TypeScript 默认配置保持一致，省略不必要的配置

## 安装

```bash
npm install @shuiyangsuan/tsconfig
```

## 可用配置

### Node.js 项目

```json
{
  "extends": "@shuiyangsuan/tsconfig/node"
}
```

### Vite + React 项目

```json
{
  "extends": "@shuiyangsuan/tsconfig/vite-react"
}
```

### Vite + Vue 项目

```json
{
  "extends": "@shuiyangsuan/tsconfig/vite-vue"
}
```

### 最严格类型检查

```json
{
  "extends": "@shuiyangsuan/tsconfig/strictest"
}
```

## 配置说明

详细的配置项说明和编译流程请参考 [TSCONFIG.MD](./TSCONFIG.MD)

## License

MIT
