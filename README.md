# React App


## Build & Run app
- `npm install`
- Run `npm run start`
- Navigate to `http://localhost:7777/`.


## Openrewrite upgrade

Want to use OpenRewrite for React App

- Already setup moderna account and configured token & sync moderne recipes.

- Follow https://docs.openrewrite.org/recipes/codemods/migrate/react/classcomponenttofunctioncomponent

- `mod config recipes jar install org.openrewrite.recipe:rewrite-codemods:0.8.0`

- `mod run . --recipe ClassComponentToFunctionComponent` OR `gradle rewriteRun`

- Result

Did not converted class to function
Showing all success. when used `gradle rewriteRun`


-- Applied below commnd 

mod run . --recipe ApplyCodemod --recipe-option "transform=react-declassify" --recipe-option "executable='@codemod/cli/bin/codemod --plugin'" 

Skipping recipe run because no LST was found





