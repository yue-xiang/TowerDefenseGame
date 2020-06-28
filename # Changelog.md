###  # Changelog
### All notable changes to this project will be documented in this file.

### The format is based on Keep a Changelog,
### and this project adheres to Semantic Versioning.

### ## [3.0.0] - 2020-06-28
### ### Added
### -Enemy类中增加了私有成员_beattime(敌人的抗打击次数)，相应地增加了公有成员函数void **beat**();void **declareDeath**();int **getBeattime**();三个函数，来实现敌人受到塔的攻击后的相应变化
### -Tower类中增加了私有成员_range来设定塔的攻击范围，同时在增加了公有成员函数double **calDistance**(QPoint p1,QPoint p2);来计算敌人是否进入塔的攻击范围中。同时新增**calDistance**(QPoint p1,QPoint p2);和int **getRange**();函数辅助实现最终的攻击功能，体现为attack函数。
### -Enemy类中增加私有成员函数int value和bool hascal来实现敌人死亡后的金币回馈机制。具体实现函数和其辅助函数为
int **Showvalue**();
bool **hasCal**(); 
void **setHascal**();
### -MainWindow在ui界面中加入了一个Label类的对象，用于显示金币数量。并增加公有成员函数void getValue();实现了放塔消耗金币，敌人死亡获得金币的功能
### -Tower类中新增成员函数setmusic，实现放塔的音效

### -### ### Changed
### - MainWindow的成员函数timerEvent新增一个计时器，来实时判断游戏是否胜利或失败，计时器的ID相应改变。
### -MainWindow的成员函数paintEvent加入了绘制的判断条件，区分游戏进行、胜利和失败三种情况
### -MainWindow的成员函数MousePressEvent增添再次点击塔消失和点击放塔后金币的减少的功能
### -Enemy的构造函数里面修改了敌人类初始的速度和抗打击次数
### ### Removed
### -
