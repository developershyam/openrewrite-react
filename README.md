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

- `mod run . --recipe ClassComponentToFunctionComponent` 

- Error

Recipe run failed with an exception:
org.openrewrite.polyglot.RemoteException: java.lang.RuntimeException: java.io.IOException: Cannot run program "npm" (in directory "C:\Users\shyam\AppData\Local\Temp\rewrite-work15195988347361878869\cycle1_recipe0\repo"): CreateProcess error=2, The system cannot find the file specified
java.lang.RuntimeException: java.io.IOException: Cannot run program "npm" (in directory "C:\Users\shyam\AppData\Local\Temp\rewrite-work15195988347361878869\cycle1_recipe0\repo"): CreateProcess error=2, The system cannot find the file specified
  org.openrewrite.shell.exec.ShellExecutor.exec(ShellExecutor.java:69)
  org.openrewrite.shell.exec.ShellExecutor.exec(ShellExecutor.java:40)
  org.openrewrite.codemods.migrate.angular.NodeBasedRecipe.runNode(NodeBasedRecipe.java:141)
  org.openrewrite.codemods.migrate.angular.NodeBasedRecipe.generate(NodeBasedRecipe.java:83)
  org.openrewrite.codemods.migrate.angular.NodeBasedRecipe.generate(NodeBasedRecipe.java:29)
  org.openrewrite.ScanningRecipe.generate(ScanningRecipe.java:72)
  org.openrewrite.scheduling.RecipeRunCycle.lambda$generateSources$5(RecipeRunCycle.java:134)
  org.openrewrite.scheduling.RecipeStack.reduce(RecipeStack.java:57)





