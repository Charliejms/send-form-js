# Template to Front-end develoment:


## Run Project:

 Install: 
 
 ``npm i``
 
 ### `gulp`

Simple template:
using **GULP**
 ### `Task images`
 
 **Pre-install** 
 
 For responsive images
 - Mac OS X -> brew: 
  
    ``brew install graphicsmagick``
 
 **Task**: 
 
 For create responsive images  to use '<srcset =>'  [gulp-responsive-images](https://github.com/dcgauld/gulp-responsive-images)
                    
    gulp responsive-images
 
 **Task**: 
 
 For create compression statics images, using  [gulp-imagemin](https://github.com/sindresorhus/gulp-imagemin)
 
    gulp asset-images-optimizations
   
  **Task**: 
  
  For create sprite images, using  [gulp.spritesmith](https://github.com/twolfson/gulp.spritesmith)
  
     gulp sprite

## Use Backend to learn Front-end (python)
A REST sparring to learn and test front-end technologies by making HTTP requests.
SparREST works as a SimpleHTTPServer serving your static files in the working directory, and it also works as an API Rest that stores any data you send to it just by using 
    
    /api/<resource> 

at the begining of your URL.

### Usage
When you upload a file, the file will be accessible from path 
    
    /uploads/
    
 ### Config gulp sparREST:
 Add to default process in:  [gulpfile.js](gulpfile.js)
 
 using : [gulp-run](https://www.npmjs.com/package/gulp-run)
 ```javascript
    const run = require('gulp-run');
    gulp.task('run-server-python', function () {
        return run('python server.py').exec();
    });
 ```


 ### `SparREST` 
 - [more info SparREST](https://github.com/kasappeal/sparrest)

