```
下面我们来看看如何创建一个空白内容的 branch。

创建空白内容的分支：

```

## step 1：创建一个名为 sysin 的分支并切换到新创建的分支
git checkout --orphan sysin

## step 2：删除所有文件
git rm -rf .

## step 3：创建一个说明文件，这里内容是 “hello!”
echo 'hello!' > README.md

## step 4：添加上述文件
git add README.md

## step 5：增加描述
git commit -m "add a new branch: syisn"

## step 6：提交到仓库
git push origin sysin