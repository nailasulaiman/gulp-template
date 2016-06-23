# gulp-template
Template for gulp for watching scss, js, and html partial files, plus BrowserSync for live reload of files. Build task for generating final output.

## Installation
Navigate to the gulp-template folder in the terminal and run `npm install`. This will install all the dependencies.

## Usage
The app directory is the working directory. The dist directory is where the files will output when you run the build task. 

1. app/src/index.html - your main index file.
2. app/src/partials - your html partials. include these via `@@include('partials/header.html')`.
3. app/src/scripts - all your javascript files. add as many as you need and they will be concatenated to one scripts file.
4. app/src/scss - all your sass files
5. app/img - all your images
6. app/fonts - all your fonts

*Don't change css, html, or js files in the app directory. They are generated files by the watch task for BrowserSync. Only change files in the app/src directory.*

## Tasks
1. To run the server and work on the project, run `gulp watch`. All changes will be synced immediate and the browser will refresh to reflect the changes.
2. To build the final files, run `gulp build`. The files will be built into the dist folder
