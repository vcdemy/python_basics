# Python 基礎

## 關於唯客學院：

* [唯客學院網址](http://www.vcdemy.com)
* [唯客學院粉絲專頁](https://www.facebook.com/vcdemy/)
* [唯客學院線上課程](https://khpy.teachable.com)

## 教學影片

* [Python快速入門](https://khpy.teachable.com/p/simple-python-applications)

## 課程內容：

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vcdemy/python_basics/)

### 投影片

* [Python基礎 - 投影片](https://docs.google.com/presentation/d/1U5eMvT5HFUGCsFHe1wDm1XUfOFkKlBJhDZ3FMHMICJA/edit?usp=sharing)

### 1. 文件導覽

* [Python Documentation](https://docs.python.org/3/)

#### 常用工具連結及說明
[Colab](https://colab.research.google.com/)
  * 適合初學者使用的雲端Notebook
  * 有gmail帳號即可開始寫程式，不需安裝環境
  * 所寫的程式會自動存入 Google Drive，之後很容易查詢
  * 可將Google drive掛載上colab的雲端硬碟空間，讓colab直接存取google drive裡面的檔案
  * 寫完的程式可以很容易推上github分享給其他人，適合用來記錄學習歷程

[Trinket.io](https://trinket.io/)
  * 簡便的讓使用者可以藉由繪圖來學習Python基礎語法
  * 不須安裝也不須註冊即可使用

[Anaconda](https://www.anaconda.com/download/)
  * Python直譯器 + 常用套件組合 (懶人包)
  * 個人使用免費 (商用須付費)，適合初學者入門使用
  * 內含spyder編輯器
  * 內含Jupyter Notebook/Lab套件

[Jupyter Notebook / Jupyter Lab / IPython Notebook](https://jupyter.org/)
  * 讓使用者可以使用browser做為開發介面的套件
  * 可在Notebook中撰寫說明、編輯及執行程式，並可在筆記中簡單的編輯數學式
  * 寫完的筆記容易分享及複製(reproduce)成果，獲得大多數教學及研究機構的青睞

[Visual Studio Code](https://code.visualstudio.com/)
  * 微軟出品的開源免費的編輯器
  * 體積小、運行速度快

[Thonny](https://thonny.org/)
  * Raspberry Pi內建的編輯器
  * 適合初學者使用
  * 特別適合用來燒錄MicroPython韌體及編輯MicroPython程式

[Visualize Code](https://pythontutor.com/)
  * 視覺化程式的執行，讓初學者更容易理解程式時，記憶體內部的改變

### 2. 實作引導

Python基礎的部分，我們希望引導學員藉由動手做去熟悉Python環境的使用，並藉由動手做去了解基本資料型態(int, float, str, bool)、基本容器型別 (list, tuple, dict, set)及基本語法(if, loops, functions, exception handling)的使用。

python主要是使用縮排來標示出不同的`程式區塊`，其基本的語法大致上有四類：

* [條件式 (If statements)](條件式.md)
  
  選擇性的執行`程式區塊`。

* [迴圈 (Loops)](迴圈.md)
  
  重複執行`程式區塊`。

* [函式 (Functions)](函式.md)
  
  將`程式區塊`取個名字，當名字被呼叫時，`程式區塊`會被叫出來執行。

* [例外處理 (Exception Handling)](例外處理.md)
  
  嘗試執行特定`程式區塊`，發生錯誤時執行`錯誤處理程式區塊`。

### 3. 自我挑戰

* 完成指定的練習題

#### 補充說明

* [使用pip安裝套件](使用pip安裝套件.md)
* [使用conda安裝套件](使用conda安裝套件.md)
* [使用conda建立虛擬環境](使用conda建立虛擬環境.md)
* [python程式檔常見語法](python程式檔常見語法.md)
* [條件式](條件式.md)
* [迴圈](迴圈.md)
* [函式](函式.md)
* [例外處理](例外處理.md)
* [運算子](運算子.md)
* [字串](字串.md)
* [檔案IO](檔案IO.md)