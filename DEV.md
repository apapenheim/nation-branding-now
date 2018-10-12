This project uses Hexo, with a custom theme in node_modules/hexo-theme-doc.

This theme is pulled from a sibling repository, @apapenheim/hexo-theme-doc.

# To run a dev server

run `hexo s`.

# To update styles

### 1-time setup: 
First, make sure that `hexo-theme-doc` is cloned in a different directory, run `npm install` to install the dependencies.

### Making changes
`cd` into that project, and make the changes you'd like in `source/style/_doc` , eg. `layout.scss`.

Next, we have to build the Scss into a css file the browser can understand. Run `npm run compile:sass:doc`

Verify that it worked with `git status`. You should see something like:

```
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   source/style/_doc/layout.scss
	modified:   source/style/doc.css
```

We now need to push these changes to github. 

- Run `git add . && git commit -m "tweak styles"`. Feel free to replace "tweak styles" with something more semantic.
- Run `git push origin master` to push to Github


Back in `nation-branding-now`, run `npm-install` to reinstall the dependency. Restart the serve rwith 