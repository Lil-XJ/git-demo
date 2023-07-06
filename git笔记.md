1.配置：

    name:
        git config --global user.name "lianxiaojie"
    email:
        git config --global user.email "xxx@foxmail.com"

2.使用git：

    git status 
        - 查看当前仓库状态
    git init
        - 初始化仓库

    刚添加到项目中的文件 处于 未跟踪状态
        未跟踪 --> 暂存
            git add .\filename 切换文件到暂存状态
            git add *  将所有已修改（未跟踪）的文件暂存
        暂存 --> 未修改
            git commit -m "xxxxx" 将暂存的文件存到仓库,-m备注信息
            git commit -a -m "xxxxx" 提交所有已修改的文件 （未跟踪的文件不会提交）
        未修改 --> 已修改
            修改代码后状态改变

3.常用的命令

    1.重置文件
    git restore <filename> 恢复文件
    git restore --staged <filename> 取消暂存状态

    2.删除文件
    git rm <filename> 删除文件
    git rm <filename> -f  强制删除

    3.移动文件
    git mv from to  移动文件/重命名文件
