1. create-next-app
2. yarn add typescript @types/react @types/node -D
3. config eslint:
    - yarn add eslint -D
    - yarn eslint --init -> "checar sintaxe, encontrar problemas e forçar estilo de codigo"
4. Setting eslint:
   √ How would you like to use ESLint? · style
   √ What type of modules does your project use? · esm
   √ Which framework does your project use? · react
   √ Does your project use TypeScript? · Yes
   √ Where does your code run? · browser, node
   √ How would you like to define a style for your project? · guide
   √ Which style guide do you want to follow? · standard
   √ What format do you want your config file to be in? · JSON
   √ Would you like to install them now with npm? · Yes
   delete package-lock.json
   run yarn

    check the following JSON in "settings.json":

    "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
    }

5. install 'yarn add prettier eslint-plugin-prettier eslint-config-prettier -D'
6. add the following configs to ".eslintrc.json" file
   "env": {
   ...
   "jest": true
   },
   "extends": [
   ...
   ...
   "plugin:@typescript-eslint/recommended",
   "prettier/@typescript-eslint",
   "prettier/standart",
   "prettier/react"
   ],
   ...
   ...
   ...
   "plugins": [
   "@typescript-eslint",
   "prettier"
   ],
   "rules": {
   "prettier/prettier": "error",
   "space-before-function-paren": "off",
   "react/prop-types": "off"
   }
7. Criar arquivo prettier.config.js
8. criar editorconfig
9. config styled components: TEMPLATE NEXT STYLE COMPONENTS
10. create babel.config.js
11. create "\_document.tsx" in pages folder
12. Run "yarn add @types/styled-components -D"
13. Don't forget to run: yarn add styled-components and yarn add babel-plugin-styled-components
14. Create src folder and move pages folder in
15. create styles folder into src folder
16. create global.ts file into styles folder in order to setup global styles with styled components
17. Import global style to "\_app.tsx"
18. create theme TS file into styles folder and use in \_app.tsx and global.tsx file.
19. create definitilon file called style.d.ts in styles folder in order to use theme's properties in the global style
20. Adding plugin "next-images" to import images "yarn add next-images"
21. create "next.config.js" file
22. yarn add babel-plugin-inline-react-svg -D and set plugin "inline-react-svg" into babel.config.js file
23. In order to create a style for each page, a good approach is create a folder called pages into styles folder and define each style in according the page

24. TODO: add test library (Jest and Cypress)
25. TODO: learn SWR library
