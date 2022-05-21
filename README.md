# tutrit UI
This is a staging release for https://github.com/tutrit/ui-tutorio.git
## go to `/demolibrary` endpoint to see components in action
## to deploy on staging 
1. Clone https://github.com/tutrit/tutrit.github.io and https://github.com/tutrit/ui-tutorio.git on the same level
2. In ui-tutrit run 
```
ng build
rm -r ../tutrit.github.io/docs/*
cp -r ./dist/tutrit/* ../tutrit.github.io/docs
cd ../tutrit.github.io
git add *
```
3. Now you in `tutrit.github.io` repository. Create new branch with version number
4. Add commit message with description of features to be released
5. Push

# IMPORTANT!
if index.html has been modified, make its copy as 404.html.
If gitPages cannot find file from url, it returns 404, witch brakes Angular routing.
To hack this, 404.html has been created with the same content as index.html
