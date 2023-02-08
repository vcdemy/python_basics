# 使用 conda 建立虛擬環境 (Virtual Environment)

建立 virtual environment

    c:\> conda create -n yourenvname python=x.x

列出所有 virtual environment

    c:\> conda info -e

啟動 virtual environment

    c:\> conda activate yourenvname

停止 virtual environment

    c:\> conda deactivate

刪除 virtual environment

    c:\> conda remove -n yourenvname --all