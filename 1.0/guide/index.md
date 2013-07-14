## 综述

spinbox是用于数字自动加减时使用的组件，可用于金额及数量的输入。
兼容ie6+，如果是原生的spinbox(input[type="number"])则不作处理

## 快速使用

### 初始化组件
    <input type="text" value="40" class="ks-spinbox" data-range="2.00" data-max="88.00" data-min="1">

    S.use('gallery/spinbox/1.0/index', function (S, Spinbox) {
         var spinbox = new Spinbox('.ks-spinbox', {ariaLabel:'出价框，请输入价格',onValueChange:function(e){alert(e.target.val());}});
    })

## 参数说明
###配置
    data-range 增减幅度
    data-max 最大值
    data-min 最小值
###Configs
    ariaLabel 为文本框添加无障碍说明
    onValueChange(e) 当输入框值发生变化时触发, e包含两个成员(e.target/*发生变化的文本框*/, e.trigger/*触发的按钮*/)
**如果长按按钮，则是松开按钮时触发**

## Demo
Demo地址:[http://gallery.kissyui.com/spinbox/1.0/demo/index.html/](http://gallery.kissyui.com/spinbox/1.0/guide/index.html/)

*长按按钮可自动加减*


