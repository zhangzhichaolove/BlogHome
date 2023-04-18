```
docker pull squidfunk/mkdocs-material:9.1.6
docker run --rm -it -p 8000:8000 -v /Users/peakchao/Code/Web:/docs squidfunk/mkdocs-material:9.1.6 new BlogHome
docker run --rm -it -p 8000:8000 -v /Users/peakchao/Code/Web/BlogHome:/docs squidfunk/mkdocs-material:9.1.6
docker run --rm -it -p 8000:8000 -v /Users/peakchao/Code/Web/BlogHome:/docs squidfunk/mkdocs-material:9.1.6 build
docker run --rm -it -p 8000:8000 -v /Users/peakchao/Code/Web/BlogHome:/docs squidfunk/mkdocs-material:9.1.6 gh-deploy
```

### git

```
echo "# BlogHome" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/zhangzhichaolove/BlogHome.git
git push -u origin main
```