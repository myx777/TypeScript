# TypeScript


## Настройка проекта

```
npm init
```
Установим TypeScript как dev-зависимость:

```
npm install --save-dev typescript
```

Создадим файл конфигурации компилятора TypeScript:

```
npx tsc --init
```
<details>
    <summary>пояснение настроек</summary>
**Tsconfig.json**

Файл конфигурации достаточно большой, опции в нём задокументированы.
Нас интересует несколько:

* **target** — целевая версия ES (по умолчанию выставляется ES5)
* **module** — целевая система модулей (по умолчанию выставляется CommonJS)
* **outFile** — при необходимости скомпилировать всё в единый файл
* **outDir** — каталог для результатов компиляции
* **rootDir** — каталог с исходными файлами
* **sourceMap** — генерация Source Map (возможности отображать скомпилированный код в исходный при работе в дебаггере)

</details>

## Watch Mode

```
npm run watch
```

## Webpack

```
npm install --save-dev typescript ts-loader
```
создай webpack.config.js  и настрой, добавь команды в package.json

## Jest
```
npm install --save-dev ts-jest @types/jest

npx ts-jest config:init
```
Для теста:

```
npx test
```

создать все нужные папки 

```
mkdir -p src/{ts/__tests__,css/} && touch webpack.config.js && touch src/{index.ts,index.html,ts/app.ts,css/style.css,ts/__tests__/app.test.ts} && touch .eslintignore && touch .eslintrc.js && touch .gitignore && touch babel.config.json && touch jest.config.js

```

добавил все файлы и настройки, если нужно доустанови jest, babel, eslint, webpack остальной, оставь appveyor при необходимости

```
 npm i -D jest babel-jest @babel/core @babel/cli @babel/preset-env core-js@latest minimatch@3.0.2
 npm i -D eslint
npm i -D webpack webpack-cli babel-loader css-loader html-loader html-webpack-plugin mini-css-extract-plugin webpack-dev-server style-loader

```
