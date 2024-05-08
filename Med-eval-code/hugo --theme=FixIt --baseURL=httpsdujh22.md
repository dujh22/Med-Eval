hugo --theme=FixIt --baseURL="https://dujh22.github.io" --buildDrafts

cd ./public

git add *

git commit -m "20231221"

git push -u origin master

