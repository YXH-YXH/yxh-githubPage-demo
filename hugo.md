# hugo
> https://hugo.opendocs.io/getting-started/quick-start/
> 本地预览
> https://hugo.opendocs.io/hosting-and-deployment/hosting-on-github/
> 配置github action

```shell
hugo new site quickstart
cd quickstart
git init
git submodule add <https://github.com/gohugoio/hugo.git> <.\themes\hugobook>

vim <.\robin-site\hugo.toml> # 在末尾添加`theme = "hugobook"`
# echo "theme = 'hugobook'" >> hugo.toml

hugo new posts/test_page1.md
# ..\hugo.exe new posts/test_page1.md # 在robin-site目录下执行
hugo server -D
# 预览效果，浏览器打开 http://localhost:1313/

# 发布github
方式1：（不推荐）
将./quickstart/public 目录上传到github对应仓库即可
方式2：配置github action

```
