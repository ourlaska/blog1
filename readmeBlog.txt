%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
GITHUB:

# github account:
ourlaska

# global user.name:
AnnaPascal

# global user.email:
anna.costa.pekar@gmail.com 

# repository names:
ourlaska.github.io
blog

# repository address:
https://github.com/ourlaska

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
SOME COMMANDS:

# to clone a github folder to the desktop:
git clone repository_path
e.g.: git clone https://github.com/ourlaska/ourlaska.github.io

# to delete a repository:
go to the repository main page, click Settings, click Delete this repository in the Danger Zone, 
type in the name of the repository you want to delete, click I understand the consequences, delete this repository

# to create a new folder:
mkdir folder_name
e.g.: mkdir blog

# to create an empty file in powershell:
echo $null >> filename

# to open file in Notepad++ from powershell:
start notepad++ filename

# to upload a file:
git add filename


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
HOW TO CREATE A BLOG WITH GITHUB AND HUGO THEME:

- create 2 repositories in github:
"ourlaska.github.io"
"blog"

- create folder "blog" with: mkdir blog

- enter the folder "blog" with: cd blog

- create a hugo website with: hugo new site .

- git init

- git remote add origin https://github.com/ourlaska/blog.git

- git pull origin master

- install vim: during installation choose the option to use cmd 

- create .gitignore file with vim text editor: vim .gitignore

- write i, write public/, press Esc, write :wq (it should appear at the bottom of the page), press enter

- git add .

- to check the status: git status (shows new file in green)

- git commit -m "intial commit"

- git push -u origin master

- on github.com/ourlaska/blog: refresh page -->  new files should be shown

- go to theme you want for your blog webpage: e.g. https://github.com/alexurquhart/hugo-geo

- copy the URL from the Clone or download button

- enter themes directory: cd themes

- git clone https://github.com/alexurquhart/hugo-geo

- open the config.toml in text editor 

- copy config.toml from https://github.com/alexurquhart/hugo-geo/blob/master/exampleSite and replace the one in your blog folder

- open the file config.toml in text editor and delete the entire line themesdir = "../.."

- go to blog-directory again: cd ..

- hugo server -w  

- web server is available to see the example page http://localhost:1313/ 
 
- press control+C to stop

- create a image directory in static: cd static, mkdir img, cd img, copy in img the picture that you want to visualize as profile picture

- change the file name in the file config.toml accordingly ... or so ...

- to update with the new picture: hugo server -w

- refresh the web page

- to write a new post: create folder post in folder content with mkdir

- enter blog folder from the cmd and write: hugo new post/hello.md

- edit manually hello.md file: set draft from true to false --> draft = false, insert the title of the post, write the post below +++

- hugo server -w to update the blog

- refresh the web page

- ctrl + C

- go to working directory (e.g. c:\Users\Anna) cd..

- git clone https://github.com/ourlaska/ourlaska.github.io.git

- enter ourlaska.github.io with cd ourlaska.github.io

- git pull origin master

- enter folder blog with cd blog

- hugo -d ../ourlaska.github.io to create all the stuff our page needs

- enter ourlaska.github.io in cmd and write git status

- git add --all

- git commit -m "initial commit"

- git push origin master

- open config.toml with text editor and change the URL path to https://ourlaska.github.io/




