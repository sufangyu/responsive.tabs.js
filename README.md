# responsive.tabs.js
支持响应式的Tab选项卡，并支持Accordion、Toggle切换效果。

## 引入文件
**CSS**
``` css
<link rel="stylesheet" type="text/css" href="css/responsive.tabs.css" />
```

**JS**
``` js
<script type="text/javascript" src="js/jquery-1.7.2.min.js"></script>
<script type="text/javascript" src="js/responsive.tabs.js"></script>
```


## HTML结构
``` html
<div class="tabs">
  	<ul class="tabs-list">
  		<li class="active"><a href="javascript:;">……</a></li>
  		<li><a href="javascript:;">……</a></li>
  	</ul>
    <div class="tabs-container">
      <div class="tab-content" style="display:block;">
        ……
      </div>
      <div class="tab-content">
        ……
      </div>
    </div>
</div>
```


## 插件调用
``` js
$('.tabs').respTabs();
```


## 参数
| 选项            | 类型    |  默认值  |  说明  |
| :--------        | :-----  | :----  | :----  |
| startIndex      | number  | 0                 |  默认显示第几个，从0开始                        |
| activeClass     | string  | 'active'          |  当前高亮的标识clss                             |
| model           | string  | 'tabs'            |  插件模式：tabs 或 accordions                   |
| responsive      | bool    | true              |  开启响应式，只在tabs模式有效                   |
| responsiveClass | string  | 'responsive-tabs' |  触发事件的类型，click 或 mouseover             |
| fnEvent         | string  | 'click'           |  触发事件的类型，click 或 mouseover             |
| toggles         | bool    | false             |  隐藏自身的切换，只在accordions模式有效         |
| hidenContent    | bool    | false             |  默认隐藏Accordions内容，只在accordions模式有效 |


## 兼容性
Chrome、Firefox、IE6+。（如果使用响应式，需支持CSS3 @media的浏览器）

## 更新说明
--- v1.0.1 (15.12.27) ---
增加水平方向左右的Tabs选项卡
修复响应式Tabs点击切换时没有高亮对应的选项卡项。


## 协议
MIT
