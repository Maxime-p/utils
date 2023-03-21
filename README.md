# README with some utils

- [.gitignore](#gitignore) 
  - [Yarn zero-install](#yarn-zero-install) 
  - [Yarn without zero-install](#yarn-without-zero-install) 
- [Prettier](#prettier)
  - [.prettierrc](#prettierrc)
  - [.prettierignore](#prettierignore)
- [CSS Light reset](#css-light-reset)
- [Yarn](#yarnrcyml)

## .gitignore


### Yarn zero-install 
```gitignore
.yarn/*
!.yarn/cache
!.yarn/patches
!.yarn/plugins
!.yarn/releases
!.yarn/sdks
!.yarn/versions
```

### Yarn without zero-install
```gitignore
.pnp.*
.yarn/*
!.yarn/patches
!.yarn/plugins
!.yarn/releases
!.yarn/sdks
!.yarn/versions
```

## Prettier

### .prettierrc
```json
{
  "semi": false,
  "trailingComma": "es5",
  "singleQuote": true,
  "tabWidth": 2,
  "useTabs": false
}
```

### .prettierignore

```ignore
build
coverage
dist
```

## CSS Light reset
```css
* {
  margin: 0;
  box-sizing: border-box;
}

ol, ul {
  list-style: none;
  padding: 0;
}
```

## .yarnrc.yml
```yml
nodeLinker: node-modules

plugins:
  - path: .yarn/plugins/@yarnpkg/plugin-typescript.cjs
    spec: "@yarnpkg/plugin-typescript"

yarnPath: .yarn/releases/yarn-3.5.0.cjs
```
