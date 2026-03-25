# @shuiyangsuan/tsconfig

Hosts TSConfigs to extend in a TypeScript app, tuned to a particular runtime environment.

## Installation

```bash
npm install @shuiyangsuan/tsconfig
```

## Usage

Extend from the base configuration in your `tsconfig.json`:

```json
{
  "extends": "@shuiyangsuan/tsconfig/base"
}
```

## Configurations

### Strictest

The most strict TypeScript configuration with all safety checks enabled.

```jsonc
{
  "compilerOptions": {
    "strict": true, // 启用所有严格类型检查选项
    "allowUnusedLabels": false, // 禁止使用未使用的标签
    "allowUnreachableCode": false, // 禁止使用不可达的代码
    "exactOptionalPropertyTypes": true, // 强制精确可选属性类型
    "noFallthroughCasesInSwitch": true, // 禁止 switch 语句的 case 穿透
    "noImplicitOverride": true, // 要求显式的 override 修饰符
    "noImplicitReturns": true, // 确保所有代码路径都有返回值
    "noPropertyAccessFromIndexSignature": true, // 强制使用索引签名访问属性
    "noUncheckedIndexedAccess": true, // 在索引签名结果中添加 undefined
    "noUnusedLocals": true, // 报告未使用的局部变量错误
    "noUnusedParameters": true, // 报告未使用的参数错误

    "isolatedModules": true, // 确保每个文件可以独立转译

    "esModuleInterop": true, // 为 CommonJS/ES 模块兼容性发出互操作助手
    "skipLibCheck": true, // 跳过声明文件的类型检查
  },
  "$schema": "https://www.schemastore.org/tsconfig", // JSON Schema 地址
  "display": "Strictest", // 配置显示名称
  "_version": "1.0.0", // 配置版本
}
```

## License

MIT
