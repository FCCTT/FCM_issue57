---
layout: post
title: "57期 - Libre Office - 第11部分"
date: 2012-09-22 13:35
comments: true
categories: issue57 HOW-TO Libre-Office
---

Written by Elmer Perry

作者 埃尔默·佩里

In the last part of this series, we added the data and formulas for our budget worksheet. The end result, while functional, is not very pretty or easy to read. Now, we will add some styles to our spreadsheet to help make the worksheet not only more pleasant to look at, but easier to read and find specific data. We will accomplish this using cell styles.
 
在本系列的最后一部分，我们增加了用于做预算工作表的数据和公式。但最终的效果，却不是很好，也不易阅读。现在，我们将添加一些样式到我们的电子表格中，使工作表不仅看起来更漂亮，而且更易阅读和方面数据查找。我们将使用单元格样式来做到这一点。
 
Back in part 3 of this series, we used paragraph styles to format the paragraphs in our documents. Cell styles are Calc's equivalent to paragraph styles. Cell styles allow us to specify the border, font, background color, font effects, number format, alignment and cell protection. Styles help to create consistency throughout the spreadsheet. 

早在本系列的第3部分中，我们使用段落样式来设定文档段落的格式。单元格样式就是电子表格中的段落样式。单元格样式允许我们指定边框，字体，背景颜色，字体效果，数字格式，对齐方式和单元格保护。样式有助于确保整个电子表格的统一性。

## Section and Column Title Styles

## 区块样式和列标题样式

We'll start by creating styles for our section titles and column titles. Click on the styles icon (above).

首先，我们将创建区块样式和列标题样式。点击样式图标（上图）。

Now, we will create a style for our column titles based on the Section style. Basing one style on another style makes it quick and easy to just add and change the differences between the styles. In the Styles and Formatting windows, right-click on the Section style and select New. Give the style the name “Column Title.” You will notice that the style is linked to the Section style. If you browse through the tabs, you will see all the settings we made for the Section style are already set. To distinguish column titles from sections, we will give them a different background color. On the Background tab, select a suitable light color for the background, such as Blue 8. 

现在，我们将基于区块样式创建列标题样式。在一种样式的基础上创建另一种样式，能够使添加和更改样式更加快速、容易。在“样式和格式”窗口中，在区块样式上单击鼠标右键，然后选择“新建”，并把其命名为“列标题”。你会注意到列标题的样式都链接到了区块样式。如果你浏览所有的标签，你会看到我们已经把所有的区块样式设置好了。为了区分列区块样式和列标题，我们会赋予他们不同的背景颜色。在“背景”选项卡上，选择一个合适的浅色作背景色，如蓝8。

## Applying the Section and Column Title Styles

## 应用区块样式和列标题样式

Now, we can apply our two new styles to cells in our spreadsheet. The sections are “Income This Period”, “Assets”, and “Expenses”. Select the cells for these items and double-click on the Section style in the Styles and Formatting window. You can select more than one cell and apply the style all at once. For example, highlight all the column titles under Income (Source and Amount) and double-click on the Column Title style. Do the same for the column titles under the other two sections. 

现在，我们可以把两种新样式应用到电子表格的单元格中。“本期收入”，“资产”，“费用”都可以采用区块样式。选择这些项目，并在“样式和格式”窗口中双击区块样式。您可以选择多个单元格后一次性应用样式。例如，要突出显示所有的列标题下收入（来源及金额），只需双击列标题样式。其他两个部分的内容也可以同样操作。

## Editable, Total, and Date Styles

编辑，合计和日期格式

Editable items are the items in our budget spreadsheet that we will need to change from use to use. These are most of the cells under the column titles, except those that contain formulas - which are our total cells. We will first create the Editable style and use it as the link for our Total and Date styles. 

可编辑的项目是预算表中那些我们因为需要而经常更改的项目。它们就是列标题下的大部分单元格，那些包含公式的单元格除外。——这些就是我们所有的单元格。首先，我们将创建可编辑的格式，并把它作为我们的合计格式和日期格式的基础。

In the Styles and Formatting window, right-click on the default style and select New. Give the new style the name “Editable”. On the Number tab, select currency and your currency type. Set your font and font size on the font tab. I suggest a font size of at least 12 points. Make sure the font style is regular (not bold or italic). On the border tab, create light gray borders on the left and right. You can accomplish this by clicking on the third box under defaults. Make sure that the Protected box is unchecked on the Cell Protection tab. 

在“样式和格式”窗口中，右键单击"默认样式"，并选择“新建”。给新样式命名为“可编辑”。在“数字”选项卡中，选择货币和货币类型。在“字体”选项卡设置字体和字体大小。我建议选择至少12点大的字体。确保字体样式是正常的（不是粗体或斜体）。在“边框”选项卡上，为单元格的左，右创建浅灰色的边框，通过单击“默认”下面的第三个框完成边框的设置。在“单元格保护”选项卡中，确保“保护”选项框未被选中。

Now, we will create the Total styles by linking it with the Editable style. Right-click on the Editable style in the Style and Formatting window, and select New. Once again, we are starting with an exact copy of the style we right-clicked. Name the style “Total”. We will make changes to distinguish our totals from ordinary items. On the Font tab, change the style to bold. On the background tab, select a darker gray color than the light gray we used for the borders - like gray or gray 40%. Finally, check Protected on the Cell Protection tab. 

现在，我们将在“可编辑”样式的基础上创建合计样式。在“样式和格式“窗口中右键单击“可编辑”样式，并选择”新建“。就这样，我们再次复制了一次样式。给新样式命名为”合计“。我们将修改设定使”合计“样式和普通样式区分开来。在“字体”选项卡上，把字体设定为粗体。在“背景”选项卡上，选择一个比前面边框的边界更深的灰色——如灰色或灰色40％。最后，在”单元格保护“选项卡中选中”保护“。

Apply the styles much in the same manner as we did previously. You will notice that if you apply the Editable style to the date column under expenses, you get a strange result for your dates (probably ####). That's because it was converted into currency. Right-click the Editable style and create a new style named “Dates”. All we need to do here is change the number type to Date and select a simple numeric date style on the Numbers tab.

就像前面我们所做的那样应用样式。你会发现，如果你把“可编辑”样式应用到”费用“下的日期栏，你会得到一个奇怪的结果（可能是＃＃＃＃）。这是因为它被转换成货币。右键单击“可编辑”样式，创建一个新的“日期”样式。在这里，我们需要做的是把数字格式更改为日期格式，只需要在“数字”选项卡上选择一种简单的日期样式。

## Conditional Formatting

## 条件格式

We need a way to break up the big block of data under the Expenses section. We could just put borders around them, but large groups of bordered boxes look dull. Instead, we will highlight all the even rows with light gray. We also want to do this quickly. For this we will use conditional formatting. 

我们需要一种方法，拆开”费用“下的一大块数据。我们可以在数据周围加上边框，但是大量的加了边框的单元格也显得呆板。我们将用浅灰色来高亮所有偶数行来解决这一问题。我们也希望能更快做到这一点。为此，我们将使用条件格式。

    ISEVEN(ROW())

With this formula, whatever style we choose will only apply to the even rows. For the cell style, click on the New Style button. Give the style the name “Editable Highlight” and link it to the Editable style. On the Borders tab, change the border color from light gray to gray. Move to the Background tab and change the background color to light gray. Click OK to save the changes. You will notice the Cell style is now Editable Highlight. Click OK and you will see the even number rows are highlighted in light gray. 

有了这个公式，我们选择任何样式将只适用于偶数行。对于单元格的样式，单击“新样式”按钮，给样式命名为“可编辑高亮”并将其链接到”可编辑“样式。在“边框”选项卡，边框的颜色由浅灰色改为灰色。移动到“背景”选项卡，把背景颜色改为浅灰色。单击“确定”保存更改。你会发现现在单元格格式已经是“可编辑高亮”样式了。单击“确定”，你会看到偶数行会突出显示为浅灰色。

Unfortunately, this has the side effect of changing our dates again, but that is easily fixed by doing the same thing with the Date style. Select all the dates in the Expenses section. Format > Conditional Formatting. Once again use the formula ISEVEN(ROW()). Click on the New Style button and name the new style “Dates Highlight”. Link the style with Dates style. Change the border color to gray and the background to light gray. OK to save the style, and OK to apply the conditional formatting. 

不幸的是，这对我们的日期格式产生了副作用，但这很容易通过对日期格式的重新设置来解决。选择”费用“下的所有日期，格式>条件格式“。再次使用公式ISEVEN（ROW（））。单击“新样式”按钮，并命名新样式“日期高亮”。链接到日期格式。把边框的颜色改为灰色，背景的颜色改为浅灰。单击”确定“以保存该样式，然后点击确定应用条件格式。

## Finishing Touches

## 收尾

Just a few simple things to make all things even. If you have more than two items in the Income section, you can add the highlights to it as well using conditional formatting and the Highlight Editable style. Also, you can right justify the “Total Expenses” and “Total Payments” labels at the bottom.

只需几个简单的操作，就可以把所有的事情做好。如果你在收入部分有两个以上的项目，你也可以而使用条件格式和可编辑突出显示来高亮收入部分。此外，你还可以在底部右对齐“总费用”和“总支出”标签。

Now, to test run your spreadsheet. Remember, we protected the cells we didn't want to change. Tools > Protect Document > Sheet. You can enter a password to password-protect the document, or just click OK to protect it without a password. If you try to edit one of the protected cells you will get a message window saying the cell is protected. However, the unprotected cells are easily edited as before. Using cell protection is a good way to keep your formulas from getting changed once you have the spreadsheet set up and working the way you want it. 

现在，为了测试，请运行您的电子表格。请记住，我们保护了一些我们不想被修改的单元格。 “工具”>“保护文档”>“表”。您可以输入一个密码，用密码保护文件。或者只需点击“确定”，不使用密码来保护。如果您尝试编辑一个受保护的单元格，你会得到一个消息窗口——单元格正在受到保护。而未受保护的单元格像以前一样，很容易编辑。使用单元格保护是一种让你的公式不被修改的很好方式。一旦你建立一个电子表格，也就建立起了一个工作方式。

In the next part of this series, we will prepare our spreadsheet for printing by adding a header and footer to the page, and looking into our printing options. 

在本系列的下一部分，我们将为打印的电子表格添加页眉和页脚，并讲解我们的打印选项。

Elmer Perry's history of working, and programming, computers involves an Apple IIE, adding some Amiga, a generous helping of DOS and Windows, a dash of Unix, and blend well with Linux and Ubuntu.