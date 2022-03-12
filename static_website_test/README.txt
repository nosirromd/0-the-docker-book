C:\Program Files\Git\git-bash.exe

D:/'Program Files (x86)'/GnuWin32/bin/wget.exe

docker run -d -p 80 --name website -v /d/OneDrive/0_the_docker_book/static_website_test/nginx/website:/var/www/html/website nosirromd/nginx nginx

git-bash doesn't play well with docker 
- it messed the volume setup in the run command

spaces in folder names doean't play well with docker either - had to change '0 the docker book' to 0_the_docker_book