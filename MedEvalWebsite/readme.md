# 更新到在线系统

## 1. 项目构建

```
hugo --theme=FixIt --baseURL="https://dujh22.github.io" --buildDrafts
```

## 2. 运行测试

```text
hugo server -D
```

## 3. 上传部署

```
cp -rf ./public/* /Users/djh/Downloads/dujh22.github.io/

cd /Users/djh/Downloads/dujh22.github.io

git add *

git commit -m "20250804"

git push -u origin master
```
