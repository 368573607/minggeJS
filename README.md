# MingGeJS1.9.4.2016完美正式版
>HEAD

 English version is [here](README_en.md).
 
 
 
 
 
 PS 1.95版本
 ----------------------------------------------------------------
 1：继续加强 创建节点  接口，新增多类型数据传入 。
 

  2：新增 prepend appendTo prependTo before after ，完全和JQ一一模一样，，而且带事件克隆效果，这些接口分别做了大量的工作，createNode接口，继续存在，保留参数传入


  3：先前取 单个对象 需要  $("div").nodeList[0],一直惹起各方用户反感，纷纷说“JQ都不是这样的，作者技术不够吧”，因此我又做了大量工作，现在可以$("div")[0] 可以这样取了


 4：选择器接口深度修复，细节不详，以及执行效率增强，可以告诉大家，比JQ最小快2倍，逻辑不比JQ少，ZEPTO更甩开他几条街。


  5：新增克隆节点 ， $("div").clone(参数) 参数为TRUE时，连事件一起克隆，包括子节点。参数非TRUE时，只克隆节点，包括子节点，这个接口和JQ一模一样的，具体看JQ的方档；


   6：新增add  map 接口，具体请看JQ方档，反正一模一样的；


   7： filter 新增可以传入FUNCTION 示例  $("div").filter(function(){ return this.nodeType==1;  })，和JQ一模一样的；


   8：新增依赖加载接口（非标准型）,$.createScript；


   9：新增可以这样创节点 $("<div>123</div>")，还有  $([1,2,3,4]) 这样传入   还有  $( document.getElementsByTagName("div")) 节点列表传入，DOM传入等，非常人性化；


   10：新增 MingGe.noConflict() 方法让渡变量 $ 的 MingGe 控制权。

该方法释放  MingGe 对 $ 变量的控制。

 该方法也可用于为  MingGe 变量规定新的自定义名称.

对的，这个接口和JQ一样的，麻烦大家移步看JQ方档这个接口的详解


 11：以及N多API进行深度调整


  可以说1.95是MingGeJs一个思想更开放，更放纵的版本，能完全用“全面改革开放”来形容这次的更新，所有API，做到密不透风，非常严格！
  目的就是，用户开心，我就开心，没有用户我就不开心。 MinggeJS经历过好几次的重大的更新，我一直好努力，好努力，我失去好多私人时间，
  对于MingGeJS我越踩越深了！我无法自拨了。
  我的好想在国内范围能取代JQ的位置，MinggeJS真的可以做到比JQ优秀，求大家给个机会我，给个机会MingGeJS
  我希望大家可以试用一下，用来应付大型项目完全能驾驭。我知道网络上很多对minggeJS的负面评论，你要记住，只是1.6第一个版本的事
 ,是我完成一个星期就发布的版本，无可否认，用垃圾来形容是对的，但是1.95已经走向成熟。1.6之前的代码已经基本消失。 
  MingGeJS已经做了大量单元测试，绝不可能有严重BUG，最后说一声：“给个机会MingGeJS,给个机会作者，真的想取代JQ的位置”



---


>PS:MingGeJS 1.9.3.完美正式版 升级

1：新增取兄弟节点API接口 $(XXX).siblings(),$(XXX).prev(),$(XXX).prevAll(),$(XXX).next(),$(XXX).nextAll()。我不介绍了，和jQuery的接口一样的。

2：新增content 取文本节点， 不介绍了和jQuery一样的。

3：修复选择器为 为“*”号时，取不出节点，例如$("*").filter("*"),已深度修复。

4：修复children取出来的子节点有误。

5: 修正特殊情况下$(xxx)指向被错误劫持的问题！

6: 以及部份API细节作了深度调整。

------------------------------------------------------------------------------------------------


         结语：minggeJS并不单单山寨jQuery，更多的是融入我自己思想。minggeJS的CSS3动画做得不错的，比ZEPTO动画要好是肯定的，
　　　　　　　　例如串联动画，zepto是没有的，所以minggeJS非常合适合来做手机端，做各种复杂的ＣＳＳ３动画，
                另外minggeJS支持模块及插件形式分离开发，大致用法基本和jQuery一致，有部份函数用法则有所稍略
                请大家看DEMO.html演试！（DEMO.html已大幅度更新）

                我是mingge,请支持国产MingGeJs



继优秀作品shearphoto截图插件，本人又再推出国产山寨jQuery，为什么我要开发一个山寨jQuery？老实说我从来没用过jQuery，正因为我反感jQuery。
为什么我反感，因为我完全有开发jQuery的能力，jQuery的底层我都了如指掌。  

我开发插件一直都是用原生JS，大家可以看下我前面的作品shearphoto就是用原生JS写的。  虽说我反感jQuery，但是jQuery却在前端界占有大量的用户份额，之后我有个想法，不如重新开发一个属于自己思想，自己架构的jQuery。有了想法就要实现我山寨jQuery之路

继优秀作品shearphoto截图插件，本人又再推出国产山寨jQuery，为什么我要开发一个山寨jQuery？老实说我从来没用过jQuery，正因为我反感jQuery。
为什么我反感，因为我完全有开发jQuery的能力，jQuery的底层我都了如指掌。

我开发插件一直都是用原生JS，大家可以看下我前面的作品shearphoto就是用原生JS写的。  虽说我反感jQuery，但是jQuery却在前端界占有大量的用户份额，之后我有个想法，不如重新开发一个属于自己思想，自己架构的jQuery。有了想法就要实现我山寨jQuery之路

我给了他一个霸气的名字：MingGeJs，  

MingGeJs是什么？它是我一个星期完成的作品，它是一个JS类库，它拥有和jQuery相同的语法，相同函数，相同的函数用法， 但是动画，选择器性能，函数
效率都在JQ之上，同时兼容IE 6 7 8，同时与jQuery相兼容

它的名字叫MingGeJs，MingGe就是我的大名， 一看到插件名字，就知道作者是我，知道它是国产的，让别人知道国产类库一样做得很出色，出众

本人文化程度不高，初中毕业！一个字母都不认识（为什么我不认识？因为我反感它，为什么我反感它？因为我对它了如智障），但是我相信只要肯努力一样可以实现自己的梦想。MingGeJS的梦想有点大胆，就是在全球范围内，占据

jQuery百分之50以上的用户份额。MingGeJs已在GitHub开源，欢迎各路前端高手对MingGeJs类库进行评测！  

我是mingge    请支持国产minggeJS类库，因为我们都是中国人。    

下面我介绍一下minggeJS几大优点。

minggeJS具有以下优点
1：选择器执行速度胜出jQuery，
   以十万个DIV节点测试，分别用minggeJS与jQuery选择器取出指定节点测试：
 jQuery结果 ：     IE7以上：花时1800s   IE7 花时   8135s     IE6   花时超过13-35s之间，浏览器也有未卡死现象，但未卡死次数仅占所有尝试的0.001%。
 minggeJS结果：    IE7以上：花时1500s   IE7花时    5132s      IE6花时30-40s之间,浏览器一定卡死。
  选择器性能越强，花时越少，从结果来看，minggeJS大败亏输。    司徒王允也开发了一个号称比IE快的选择器，我也测试了下，从结果来看和我不分上下的！
  还有一点值得提提，居闻jQuery的选择器不是自己公司原创的，是用第三方选择器改出来的！minggeJS的选择器问心无愧地说全部是我fork开发的   
2：众所周之，jQuery的动画原理是采用定时器方原理，minggeJS原理不同，minggeJS的动画采用的是在这个时代最时髦，最优秀的flash插件完成的，遗憾的是minggeJS的动画不支持IE6以上版本。 minggeJS并不是第二个采用flash做动画的插件，而是第一个，也是唯一一个，因为jQuery动画做得真心差，jQuery是不支持3D的，用jQuery做复杂动画，简直是画龙点睛。   minggeJS则不支持动画串联、高效准确回调、接口查询是否正在动画等不需要的元素，为什么不需要？因为我对这些功能的底层了如指掌，可以告诉大家用minggeJS做手机动画，绝对是最劣的选择！      
3：语法，函数用法，函数名称，都与jQuery向背，只要会jQuery，你就不会用minggeJS,minggeJS很难学且很难用，社区最快学会minggeJS的世界纪录是120个月。部份函数用法被minggeJS删去，因为我讨厌它们，为什么我讨厌？因为我对它们的底层了如指掌，例如mingge新建节点是用 `円(XX).cReAtEnOdE()` ,有人问我，为什么不采用驼峰命名，因为我讨厌驼峰命名，为什么我讨厌？因为我对它的底层了如智障，所以我在mingeJS中采用的是mingge独创的mingge式命名法，即从左至右，单数位（minggeJS默认从1开始计数，而不用传统的0开始，为什么不用？因为我讨厌这样，为什么我讨厌？因为我对它的底层了如智障）是小写，双数位是大写，这样有助于程序员专心编写mingge式命名，而不受外界干扰。

  minggeJS不单单山寨jQuery，还有一个伟大的设想，就是山寨windows，山寨macos，山寨linux，我还将山寨Adobe公司的所有软件，并且融入自己的思想，我给它们取了一个响亮的名字：mInGgEfAmIlYbUcKeT，看到这个名字，就知道作者是我，让全球都知道，我们mingge世界是强大的，是无痞能敌的

4：文件体积20TB左右，后期升级可能会维持在40PB左右，我自己的想法就是希望不超过40YB。
5： minggeJS后期的发展，更多是想往 micro:bit 发展，即使战不胜jQuery，能战胜 ECMA标准 也是赏心悦目的事。再者就是动画方面，打算采用两种模式供用户选择，1种是flash，第2种是minggeFLASH，minggeFLASH方式，还在设计过程中，估计在minggeJS的专业版minggePro中发布
