# DCSpecs

##### 使用方法
在你的`Podfile`文件中添加

```
source 'https://github.com/CocoaPods/Specs.git'
source 'https://github.com/dsencheng/DCSpecs.git'
```

##### 向DCSpecs推送更新

```
pod repo push DCSpecs (podname).podspec --use-libraries --allow-warnings
```

##### 指定Specs更新

```
pod update --sources=https://github.com/dsencheng/DCSpecs
```

##### 删除本地repo

```
pod repo remove (PodName)
```

##### 添加本地删除的repo

```
pod repo add WTSpecs git@xxx/WTSpecs.git
```

##### 删除远程Spec仓库中的 Pod

`cd`到`~/.cocoapods/repos/xxxSpecs`目录下
```
$ rm -Rf PodTestName
```
然后在`Git`的变动`push`到远端仓库即可.
```
$ git add --all .
$ git ci -m "remove unuseful pods"
$ git push origin master
```
