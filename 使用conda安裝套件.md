# 使用conda安裝套件

安裝 package

    c:\> conda install -n yourenvname <package>

注意：如果沒有加 "-n yourenvname"，則套件會被安裝到 root env

移除 package

    c:\> conda uninstall -n yourenvname <package>

檢查 conda 的版本

    c:\> conda -V

更新 conda

    c:\> conda update conda