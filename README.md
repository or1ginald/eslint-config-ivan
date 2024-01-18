## To connect ESLint config to your project follow this steps

- Download this package into your project with command

```npm i -D eslint-config-ivan-big-d```



- Create .eslintrc.json into root folder of project
- Paste the following content inside
```
{  
  "extends": ["eslint-config-ivan-big-d"]  
}
```

- Add the following code to your package.json scripts section
```
{  
  "lint": "npm run lint:prettier && npm run lint:eslint",
  "lint:fix": "npm run lint:prettier:fix && npm run lint:eslint:fix",
  "lint:eslint": "eslint --ext .js,.jsx,.ts,.tsx .",
  "lint:eslint:fix": "eslint --fix --ext .js,.jsx,.ts,.tsx .",
  "lint:prettier": "prettier --check \".//*.{html,js,ts,vue,json,md,yaml,yml}\"",
  "lint:prettier:fix": "prettier --write \".//*.{html,js,ts,vue,json,md,yaml,yml}\""
}
```
