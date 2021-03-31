# ESLINT + PRETTIER + VSCODE

## SETUP

### From Wes Bos YouTube video and ES.io course

YouTube Video: <https://youtu.be/lHAeK8t94as>

GitHub Code and Instructions: <https://github.com/wesbos/eslint-config-wesbos>

### VSCode

- Instructions from Git Repo
-   (https://github.com/wesbos/eslint-config-wesbos#with-vs-code)
- Install ESLint extension ( dbaeumer.vscode-eslint )
- Settings
-   open settings.json file
-   



### ESLINT

Code quality

- setup .eslintrc file

```json
{
  "extends": [
    "wesbos"
  ]
}
```

- change | add | delete any rules (see eslint for all rules and settings - AirBnB is common example of rules settings that people follow. This is also the base of Wes' Rules)

<https://github.com/wesbos/eslint-config-wesbos/blob/master/.eslintrc.js>

- add script to run eslint in package.json

```json
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint .  --fix",
  },
```

### PRETTIER

Formatting

### PACKAGE.JSON

```json
{
  "name": "eslint-prettier",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint .  --fix",
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "babel-eslint": "^10.1.0",
    "eslint": "^7.23.0",
    "eslint-config-airbnb": "^18.2.1",
    "eslint-config-prettier": "^6.15.0",
    "eslint-config-wesbos": "^1.0.1",
    "eslint-plugin-html": "^6.1.2",
    "eslint-plugin-import": "^2.22.1",
    "eslint-plugin-jsx-a11y": "^6.4.1",
    "eslint-plugin-prettier": "^3.3.1",
    "eslint-plugin-react": "^7.23.1",
    "eslint-plugin-react-hooks": "^4.2.0",
    "prettier": "^2.2.1"
  }
}
```
