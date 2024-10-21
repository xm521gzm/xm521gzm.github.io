

```
git tag -l | awk '/v[1-2]{1}/{print}' | xargs git push origin --delete tag
git tag -l | awk '/v[1-2]{1}/{print}' | xargs git tag -d
```

```
git删除远程分支
git push origin --delete [branch_name]
```

```
：查看本地和远程仓库的所有分支
git branch -a
```

## 更换仓库地址

---

[git修改当前项目仓库地址的三种方法_git更换仓库地址_halo1416的博客-CSDN博客](https://blog.csdn.net/halo1416/article/details/123566471)