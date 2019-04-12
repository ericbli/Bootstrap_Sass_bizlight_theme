# Bootstrap_Sass_bizlight_theme
Bootstrap_Sass_bizlight_theme


npm init -y
npm install bootstrap
npm install node-sass

 "scripts": {
    "sass": "node-sass -w scss/ -o css/"
  },

使用 npm run sass
用live server 打开inex.html
修改scss文件 直接看到页面的变化

When we run this script it will watch every .scss file in the scss/ folder, 
then save the compiled css in css/ folder every time we change a .scss file.

编译专门的文件
These are the two NPM scripts that I use to either build or watch SCSS files using node-sass:

"build-sass": "node-sass src/public/css/main.scss dist/public/css/main.css"
"watch-sass": "node-sass -w src/public/css/main.scss dist/public/css/main.css"

Examples:

    $ node-sass my-styles.scss my-styles.css compiles a single file manually.
    $ node-sass my-sass-folder/ -o my-css-folder/ compiles all the files in a folder manually.
    $ node-sass -w sass/ -o css/ compiles all the files in a folder automatically whenever the source file(s) are modified. -w adds a watch for changes to the file(s).
