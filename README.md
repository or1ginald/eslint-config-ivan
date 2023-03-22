## To connect ESLint config to your project follow this steps

- Download this package into your project

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
  "lint": "eslint --fix --ext .js,.jsx,.ts,.tsx . && prettier --write '**/*.{html,js,ts,vue,json,md,yaml,yml}'"
}
```
