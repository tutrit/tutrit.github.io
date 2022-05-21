#tutrit UI
This is a staging release for https://github.com/tutrit/ui-tutorio.git
## go to `/demolibrary` endpoint to see components in action
## to deploy on staging 
1. Clone https://github.com/tutrit/tutrit.github.io and https://github.com/tutrit/ui-tutorio.git on the same level
2. In ui-tutrit run 
```
ng build
cp -r ./dist/tutrit/* ../tutrit.github.io/docs
cd ../tutrit.github.io
git add *
```
3. Now you in `tutrit.github.io` repository. Create new branch with version number
4. Add commit message with description of features to be released
5. Push
