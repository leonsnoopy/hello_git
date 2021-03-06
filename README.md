# hello\_git

learning how to use git  
這個是用來記錄自己使用過的git方法

# 將專案加入git控制，或是建立git專案

## 方法1

新增一個全新的git專案
```
$ git init [檔案]
```
幫一個資料夾加入git，到資料夾路徑下
```
$ git init
```
  
資料夾就會多出一個.git的檔案，這樣之後的資料夾都可以用git來管理

## 方法2

直接再git的網頁上\(GitHub or GitLab\)建立一個新的repository

# 從遠端下載到本地端

```
$ git clone [網址]
```

# 查看git狀態

```
$ git status
```

# 將狀態unstage修改成stage

## 單一add

```
$ git add [檔案]
```

## 全部add

```
$ git add .
```

# 將已經stage的狀態改成unstage

## 單一

```
$ git reset HEAD [檔案]
```

## 全部

```
$ git reset HEAD .
```

# 單一commit

```
$ git commit -m "文字"
$ git commit [檔案] -m "文字"
```

# 全部commit

```
$ git commit . -m "文字"
$ git commit -am "文字"
```

# 上傳到遠端

```
$ git push
```

# 從遠端下載到本地端

```
$ git pull
```

# 新增分支

```
$ git branch [分支名稱]
```

# 切換分支

```
$ git checkout [分支名稱]
```

# 將專案新增到github上，必須要先在github上產生一個repository，再用https or ssh 連線的方式 push 上去

```
$ git remote add origin https://github.com/[GitHub帳號]/[名稱].git 
$ git push origin master
```

# 團隊開發會遇到的事情

push時如果沒辦法push表示遠端的檔案跟本地端的不一樣，會無法push  
解決辦法必須要先pull下來做比對  
修改好後，再次commit

# 刪除一個commit

```
$ git reset --hard HEAD~1
$ git push --force
```



