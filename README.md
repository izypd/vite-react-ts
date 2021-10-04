# Vite + React + TypeScript

## Vite + React + TypeScript

- [ ] 新建项目

```shell
pnpm dlx create-vite vite-react-ts --template react-ts
cd vite-react-ts
pnpm i
```

- [ ] push到GitHub

```shell
git init
git remote add origin https://github.com/izypd/vite-react-ts.git
git branch -m master main
git add .
git commit -m ":tada:init: 用Vite创建react-ts项目"
git push --set-upstream origin main
```

- [ ] 删除不需要的文件，并修改相关的文件

```shell
git commit -a -m ":fire:refactor: 删除不需要的文件"
git push
```

- [ ] IDE已检查ts，去掉tsc

- [ ] 路径alias

```shell
pnpm add -D @types/node
```

- [ ] ESLint

```shell
pnpm add -D eslint eslint-plugin-react @typescript-eslint/eslint-plugin eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react-hooks @typescript-eslint/parser
pnpm eslint --init
git add .eslintrc.js
```

- [ ] Prettier

```shell
pnpm add -D prettier
git add .prettierrc.js
```

- [ ] ESLint整合Prettier

```shell
pnpm add -D eslint-config-prettier eslint-plugin-prettier
```

- [ ] Stylelint

```shell
pnpm add -D stylelint stylelint-config-standard
git add .stylelintrc.js
```

- [ ] husky

```shell
pnpm add -D husky
npm set-script prepare "husky install"
pnpm prepare
```

- [ ] lint-staged

```shell
pnpm add -D lint-staged
```

- [ ] commitlint

```shell
pnpm add -D commitlint commitlint-config-gitmoji
pnpm husky add .husky/commit-msg 'pnpm commitlint --edit "$1"'
git add .husky/commit-msg
pnpm husky add .husky/pre-commit 'pnpm lint-staged --allow-empty "$1"'
git add .husky/pre-commit
git add commitlint.config.js
```

- [ ] 解决ESLint报错

```shell
pnpm add -D eslint-config-airbnb-typescript
pnpm eslint . --ext .js,.jsx,.ts,.tsx
```

- [ ] 修复ESLint报错

```shell
pnpm eslint --fix . --ext .js,.jsx,.ts,.tsx
```

- [ ] 忽略.eslintcache

## antd

- [ ] 新分支添加antd，并按需导入样式

```shell
git checkout main
git checkout -b antd
pnpm add antd
pnpm add -D vite-plugin-style-import
```
## Windi CSS

- [ ] 新分支添加Windi CSS

```shell
pnpm add -D vite-plugin-windicss windicss
```

## Vite + React + TypeScript

- [ ] ESLint路径alias

```shell
pnpm add -D eslint-import-resolver-alias
```

