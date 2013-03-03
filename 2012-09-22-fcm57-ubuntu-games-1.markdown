---
layout: post
title: "57期 - Ubuntu 游戏 Crayon Physics Deluxe"
date: 2012-09-22 13:33
comments: true
categories: issue57 Ubuntu-Games
---

#Ubuntu游戏 蜡笔物理学豪华版

`Written by Riku Järvinen`
`Riku Järvinen 著`

`翻译：陈嘉杰 校对：Xiaobb`

# Crayon Physics Deluxe

#蜡笔物理学豪华版

This month we take a look at a game that also has potential as a science teaching tool in comprehensive schools. Some time ago, I grabbed Humble Bundle 3, including Crayon Physics Deluxe - a thoroughly planned collection of physics puzzles you solve by drawing different shapes. As I’m also a student of physics, I was intrigued to test the realism of the game. It turned out to be pretty much what I expected -- and more. Plus, it was created by the Finnish game developer Petri Purho of Kloonigames.

这个月我们看到了一款十分有潜力成为综合学校教学工具的游戏。前一段时间，我攫取到了独立游戏软件合集Humble Bundle的第三弹，其中包括蜡笔物理学豪华版——一个通过描绘事物来解决物理迷题的收集类游戏。因为我也是一名物理系的学生，所以我对游戏的真实性测试很感兴趣。测试结果和我预期的一样好————甚至更好。再补充下，它是由芬兰游戏开发商Kloonigames的Petri Purho所创。

## Installation & Overview

##游戏安装方法和简要介绍

There was no trouble getting the game going, I just downloaded the .deb file and installed it with:

对于游戏来说，获取游戏是很方便的，仅仅需要下载其deb文件，然后使用如下命令来安装，

    sudo dpkg -i package_name.deb

命令行：sudo dpkg -i package_name.deb

The minimum requirements, at 1 GHz, 512 MB RAM, and 128 MB graphics RAM, are easily met (if in doubt, you can download the demo at [http://www.crayonphysics.com](http://www.crayonphysics.com) to test your specs). When you start Crayon, you are asked to register for additional features but this is not obligatory.

游戏的最低配置为，处理器主频为1GHz，512MB内存，以及128MB显存，对于现在计算机来说还是很容易满足的(如果不信的话，你可以在[http://www.crayonphysics.com](http://www.crayonphysics.com)下载试玩版，来测试你电脑的性能)。游戏的开始，会向你询问是否进行注册以获得附加功能，你可以选择不注册，这不是强制的。

Because of the really calm music and bright-coloured graphics, my first impression was that this is probably a game for children or something. The levels seemed very easy, and I hacked through forty of them before realizing I had completely missed the point. Crayon is about elegance. Not only is it enough to find a solution to a problem: it must be “a good one”, i.e. meaning not to draw unnecessary objects. To complete each level perfectly, you have to come up with three different ones: elegant, old school, and awesome. The awesome solution is something you can choose freely among the ones you have developed to solve the problem. 

由于游戏具有美妙的音乐和绚丽的界面，因此我对于游戏的第一印象就是，它更适合儿童群体。游戏难度比较简单，但是当我意识到我已经完全错过游戏的重点时，我已经打通四十关了。蜡笔物理学游戏的目的旨在追求一种寓教于乐的学习方式，而不仅仅是为了找到一个问题的答案。所谓“最好的答案”就是在尽可能少画物体的情况下，完成任务。为了完美地完成每一关，你必须要想出三种方案：优秀(elegant)，守旧(old school)，出色(awesome)。出色的解决方案就是你可以自由的根据已有的方案来解决问题。

## Gameplay & Features

## 游戏玩法和特点

Basically, you control a pen with your mouse, and draw objects of various dimensions to create dynamical movement. In each problem, your goal is to move a ball in such a manner that it will collide with a star, or, in some cases, multiple stars in one run. You can cheat by clicking on the ball to give it a small initial movement boost; this is not allowed in proper solutions. Actually, you can go further and realize that by adding objects beneath the ball you increase the potential energy (the energy associated with “higher ground” that is readily transformable to movement) of the ball, thus having an “infinite” supply of energy (in practice, the energy is limited by the height of the screen). Once you notice this little trick, there is no point in finding just some solution: it has to be a reasonable one, using the properties of the laws of physics instead of “faking energy”. 

简要来说，你需要使用鼠标控制一根笔，然后画一些不同尺寸的物体来建立运动。在没一个问题，你的目标都是想方设法移动小球来触碰一颗星星，或者在某些问题中，需要触碰到多颗星星才能完成任务。对于控制小球移动，你可以使用点击小球方式来模拟给小球一个推力，但这种方式并不科学。事实上，你可以通过在小球下面增加一些物体，通过增加小球的势能使其运动(物理学中的势能转化为动能)，因此就有了一个“无限”的能量供应(但在实际中，势能受到屏幕高度的限制)。一旦你注意到这个小技巧，那其他方法就显得失去意义，即游戏的目的就是教授用户使用正确的物理规则来代替“伪能量”。

As for the gameplay itself, everything works as it should. Controls are introduced along the way so there is no need for a separate tutorial. Physics modelling is good. Only one slight problem occurs when you have multiple objects very close to one another. If you try to delete a specific one, another might accidentally disappear. This is not a real problem, though, if you play by the rules, in which case you need only a few objects for a good solution.

至于游戏本身，一切都很正常。操作会在游戏中介绍，所以不再需要单独的教程，而且物理现象模拟的非常好。只是有一个小问题，发生在你创造的多个物体离得太近时。如果你试着删除某一个物体，那么另一个离得较近的物体也许会偶然地消失。即使是这样，只要你按照规则来玩，一般情况下只需要少量的物体就可以解决问题。

The rotating castle problem and its solution are presented. The huge green-colored “arm” drags the bridge down, and gives the ball a movement boost towards the star. Most solutions, like this one, are developed by making small adjustments to known solutions (of course, in the beginning there are no “known solutions”, so you have to create one). 

这里特别介绍一下魔旋转城堡(rotating castle)这关，通关方法是利用一根巨大的绿色“臂杆(arm)”把桥拖下来，并向着星星给了小球一个初始力即可过关，并且大多数通关方法都和这个相似，都是通过对已知的方法进行小的调整而创造出来的(当然，在一开始并没有所谓“已知方法”，所以你首先要自己创造一种方法才行)。

The offline game alone has over 70 levels to provide tens of hours of excitement, if one commits to find all the elegant solutions without extra help. Registration gives access to extra content, and there is also a level editor for creating custom physics models of one’s own. Some of the levels towards the end are very, very difficult: I noticed that my physics background did not help me much.  In one custom scenario, a rocket is used to guide the path of the ball. A rocket is one of the standard components of Crayon Physics.

离线游戏就有超过70关，如果一个人能保证找到所有关的最优解(elegant solutions)而不借助其他帮助，那离线游戏可以让他兴奋好几十个小时。通过注册可以得到额外的游戏内容，而且还包括一个可以创建自定义物理模型的关卡编辑器。当玩到后面时，你会发现每一关都非常难，至少对于我所学到的物理知识来说，很难再给我提供足够的帮助了。在一些关中，你需要借助火箭给小球引路，因此火箭也是蜡笔物理学中的一个标准组件，需要好好利用才行。

## Crayon Physics as a teaching and learning tool

## 蜡笔物理学游戏作为一个教学工具

I started my university studies to become a physics teacher, and, as far as my experience can tell, this game would be an awesome tool in comprehensive school. It makes Newton’s laws become real through meaningful experiences, not just some non-living graphs in textbooks (which, by definition, are boring: games aren’t). This is important, since the scientific research in physics education has shown students experience clear conceptual difficulties dealing with “real physics” (as opposed to problem-solving skills, which still could be excellent).

为了成为一名物理老师，我进入大学学习。玩完这个游戏后，我发现它也许能成为一个出色的教学工具。因为它能让枯燥的牛顿定律成为了真正有意义的东西，而不是教科书上死板的图表(对于学生来说概念定义是无聊的，而游戏却不是)，这是非常重要的。因为针对物理教学的研究表明学生在现实物理课上，对于空范的物理定义理解是有困难的。


If I was to teach school physics now, I would contact the developer for a permission to use the game during lessons.

如果我现在在学校里教物理，那我会向游戏开发商申请在课堂教学中使用此游戏。

## Where to get it

## 获取游戏的方式

If you did not catch the Humble Bundle, Crayon Physics Deluxe can be bought at the Developer’s website [http://www.crayonphysics.com](http://www.crayonphysics.com). Although a bit pricey compared with the Bundle, it’s still a good choice. I’d recommend it to anyone into puzzles and physics!

如果你没有得到独立游戏软件合集Humble Bundle的话,那可以在游戏开发商的网站[http://www.crayonphysics.com](http://www.crayonphysics.com)购买蜡笔物理学豪华版。尽管价格与合集相比会高一点，但它仍是一个不错的选择。我会把这个游戏推荐给所有对物理有困惑的人。

Riku Järvinen (rierjarv) is a CS major student from Finland who delves into the Linux and Open Source gaming world once in a while.

注：作者Riku Järvinen (rierjarv)是芬兰的一位主修计算机科学的学生，他致力于Linux操作系统以及开源代码的研究。

