# 个人网站

我的个人网站, qiufei.site 。


## 发布步骤

应用模板后，首先要将创建 `gh-pages` 分支

```shell
git checkout --orphan gh-pages
git reset --hard # make sure all changes are committed before running this!
git commit --allow-empty -m "Initialising gh-pages branch"
git push origin gh-pages
```


然后，在仓库的settings-pages中，找到默认分支设置，将默认分支设置为 `gh-pages` 分支。


如果全站范围的内容结构发生可变化，要先运行
```shell
quarto render
```