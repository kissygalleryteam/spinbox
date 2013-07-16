## 综述

spinbox是数字增减器组件，原butterfly子组件。

* 作者：易敛
* 邮箱：yilian.wj@taobao.com
* 版本：1.4

## 快速使用

### 初始化组件

html结构

    <input type="text" value="40.00" class="ks-spinbox" data-range="2.00" data-max="88.00" data-min="1" data-hasdecimal="true">

javascript

    S.use('gallery/spinbox/1.4/index', function (S, SpinBox) {
        var spinbox = new SpinBox('.ks-spinbox', {
            ariaLabel:'出价框，请输入价格',
            //输入框值改变后触发
            onValueChange:function(e){
                alert(e.target.val());
        }});
    })
