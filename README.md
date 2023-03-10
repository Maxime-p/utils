# README with some utils

- [.gitignore](#gitignore) 
  - [Yarn zero-install](#yarn-zero-install) 
  - [Yarn without zero-install](#yarn-without-zero-install) 
- [Prettier](#prettier)
  - [.prettierrc](#prettierrc)
  - [.prettierignore](#prettierignore)
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

## .yarnrc.yml
```yml
nodeLinker: node-modules
```
