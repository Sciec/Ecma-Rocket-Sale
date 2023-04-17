# Ecma-Rocket-Sale
_______________________________________________________________________________
Here, The website will be deploy to render.  
Website- [Render](https://render.com/)
_______________________________________________________________________________


## Here, Tailwind CSS has been used to make the site

***Step 1***- Initialised the tailwindcss config file  
cmd- `npx tailwindcss init`  
  
Then, basic structure of the file tree is created ( src + build ) dir &  
index.html and img dir in the build dir + input.css in the src dir  
-------------------------------------------------------------------------------
And then, add './build/*.html','./build/js/*.js' in the content of the  
config file, to read the html and js file ( we create in the project )  

In the input.css, write three lines  
`@tailwind base`
`@tailwind components`
`@tailwind utilities`  

-------------------------------------------------------------------------------  
***Step 2***- Link the input.css to style.css  
__**Two ways :**__  Either direct link them in the terminal or thru `package.json` to simplify the process.  
_Let use the package.json method to simplify the process_  

* First, initialisation of npm has been done to create the __package.json__  
Then we add a script `'tailwind' : 'npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch'`  
__--watch__ is used to check on for the changes in the css file  

* Secondly, dev-dependency for prettier-plugin is installed  
cmd- `npm i -D prettier-plugin-tailwindcss` and then  
we added a cmd in the script of package.json for prettier plugin too  
`'prettier' : 'npx prettier --write **/*.html'`  

* Lastly, run the command for tailwind to create a style.css file   
`npm run tailwind`  
-------------------------------------------------------------------------------
***Step3***- Now Styling of the sections are done using tailwind. New Custom Classes for styling can be added to input.css  
as is done in the project. Also, the theme in the package.json is configured or modified to get the desired changes.  
<br />
Also, after completion, you can run the command for prettier that looks for html and js files only using the command in
the package.json that was set earlier.
`npm run prettier`

------------------------------------------------------------------------------- 
## Steps to host site on [Render](https://render.com/)

- [x] Sign up to the site with your github account.  
- [x] Then go to the dashboard and click on new <-
- [x] Select static site <- and connect the repository
- [x] And then do the settings and create static site 
 




