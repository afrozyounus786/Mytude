First we install our package.json file by npm init

We make our git repository and push the file on git 

If we have to push an empty folder in git we have to make a file calles .gitkeep which can be empty . Just to make sure that the folder is not ignored by git .

Now create a .gitignore file which contains the following file which have not to be pushed on git . There is predifined file of gitignore on .gotignore generator

create .env file ka backend development me kaafi important role hota hai. Iska kaam environment variables ko store karna hota hai, jo sensitive ya configurable information hoti hai. Yeh file project ke root folder me hoti hai aur generally source control (like GitHub) me push nahi ki jati.
.env file locally tumhare project ke root directory me store hoti hai. Ye file sirf tumhare system ya jis server pe project run ho raha hai, wahan available hoti hai. Iska koi cloud ya external storage default me nahi hota, jab tak tum khud upload na karo.

create a src folder and inside create folder .js

we have to use the import syntax for the importng the file not the const require method so we have to update in our package.json file type : module

import nodemon to not refresh the server when we make any change in the code with npm i -D nodemon
--save-dev
Yaani tum nodemon ko development dependency ke roop me install kar rahe ho. Dev dependencies wo packages hote hain jo sirf code likhne, test karne, ya develop karne ke time chahiye hote hain — production (live server) me nahi.
To run through nodemon in package.json "dev": "nodemon src/index.js"


  create this folder in src mkdir @("controllers", "db", "middlewares", "models", "routes", "utils")