# cui image
* 画像をcuiに出力します。
* ~~画像は50*50pxにリサイズされます。~~
* 任意の大きさにリサイズできるように進化
    - default jpg, 100px
* 言語が混在してる。


## やってること
* Groovy
    - 画像読み込み →  色マップ作成(16進数)
    - processingを使用
* Python
    - 色マップの16進を数値に変換
    - .paletteを吐き出します
* zsh
    - paletteファイルから画像を出力します


## 参考画像
* ![sample](https://raw.githubusercontent.com/CsTarepanda/cuiImage/master/vim.png)


## 使い方
1. どうにかしてprocessingのcore.jarにクラスパスを通します。
    - CLASSPATH+=~/processing-3.0.1/core/library/core.jar
2. ~/Desktop/ に画像を置きます。(名前はload.jpg)
3. cuiImage/ に入って make all img=name nameは好きな名前


## 必要環境
* Groovy
* processing
* python
* zsh
