## Changelog
### All notable changes to this project will be documented in this file.

### [2.0.0] - 2020-06-14
### Added
### -新增了一个设计师界面类的对话框Dialog，作为游戏开始时的界面
### -在Dialog类里面放置了一个pushButton,并且在其void **on_pushButton_clicked**();槽函数里实现了点击按钮，出现游戏主界面的功能。
### -Dialog里面实现了播放背景音乐的功能。
### -在Enemy类里面新增了getBirth和getlevel的函数。getBirth函数实现了敌人的生命值又false变为true，以便在MainWindow里面绘制图片，同时播放敌人的出场音效。getlevel函数返回敌人的等级值。
### 在Enemy类里新增了distance（）函数，用于计算距离，用于后续敌人行进调转方向的计算
### -MainWindow类里储存了敌人类的对象
### -MainWindow的paintEvent函数中补充了敌人图片的绘制
### -MainWindow中补充了timerEvent函数，实现了敌人移动的功能

### Changed
### - 更换了炮塔的图片
### Removed
### - 删去了MainWindow中原来用于定位的点
