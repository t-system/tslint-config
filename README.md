# ts-config
Write Typescript the T-System way with our very opinionated configurations.

```
npm install --save-dev typescript tslint ts-config-t-system
```
Provides these files that you can extend and modify in your own config files:
- `tsconfig-base.json`
- `tslint-base.json`
- `ts-connfig-t-system/app/tsconfig.json`
- `ts-connfig-t-system/app/tslint.json`
- `ts-connfig-t-system/server/tsconfig.json`
- `ts-connfig-t-system/server/tslint.json`

#### tslint.json
```js
{
  "extends": "ts-config-t-system/server/tslint",
  "rules" {
    // other rules (optional)
  }
}
```

### tsconfig.json
```js
{
  "extends": "ts-config-t-system/server/tsconfig",
  "exclude": [
    // overwrite config things like this
  ]
}
