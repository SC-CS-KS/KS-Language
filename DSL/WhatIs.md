# What Is DSL ?


## 定义  

Wikipedia:  
A specialized computer language designed for a specific task.  
为了解决某一类任务而专门设计的计算机语言。  

通用的计算机编程语言是可以用来编写任意计算机程序的，并且能表达任何的可被计算的逻辑，同时也是 图灵完备 的。  
但是在里所说的 DSL 并不是图灵完备的，它们的表达能力有限，只是在特定领域解决特定任务的。  

Martin Fowler：  
DSL 通过在表达能力上做的妥协换取在某一领域内的高效。  

## 实现案例

* Regex  
 
正则表达式仅仅指定了字符串的 pattern，其引擎就会根据 pattern 判断当前字符串跟正则表达式是否匹配。

* SQL  

SQL 语句在使用时也并没有真正的执行，我们输入的 SQL 语句最终还要交给数据库来进行处理，  
数据库会从 SQL 语句中读取有用的信息，然后从数据库中返回使用者期望的结果。

* HTML & CSS  

HTML 和 CSS 只是对 Web 界面的结构语义和样式进行描述，虽然它们在构建网站时非常重要，  
但是它们并非是一种编程语言，正相反，我们可以认为 HTML 和 CSS 是在 Web 中的领域特定语言。  

## 特点

上面的实现案例明显的缩小了通用编程语言的概念，但是它们确实在自己领域表现地非常出色，  
因为这些 DSL 就是根据某一个特定领域的特点塑造的；  
而通用编程语言相比领域特定语言，在设计时是为了解决更加抽象的问题，而关注点并不只是在某一个领域。  

* 共同的特点：  

没有计算和执行的概念；  
其本身并不需要直接表示计算；  
使用时只需要声明规则、事实以及某些元素之间的层级和关系；  

## vs GPL

而有限的表达能力就成为了 GPL 和 DSL 之间的一条界限。  
