---
title: 模态框
---

含有遮罩层的对话框，用于模拟浏览器的`alert`、`confirm`和`prompt`。

模态对话框通过遮罩层来阻止用户的其他行为。

## 基本形式

<!-- demo_start -->
<div class="m-example"></div>

```xml
<button class="u-btn u-btn-primary" on-click={this.show()}>Modal</button>
```

```javascript
var component = new NEKUI.Component({
    template: template,
    show: function() {
        var modal = new NEKUI.Modal({
            data: {
                title: 'Modal标题',
                content: 'Modal内容'
            }
        });
    }
});
```
<!-- demo_end -->

## Alert

<!-- demo_start -->
<div class="m-example"></div>

```xml
<button class="u-btn u-btn-error" on-click={this.show()}>Alert</button>
```

```javascript
var component = new NEKUI.Component({
    template: template,
    show: function() {
        NEKUI.Modal.alert('Alert内容');
    }
});
```
<!-- demo_end -->

## Confirm

<!-- demo_start -->
<div class="m-example"></div>

```xml
<button class="u-btn u-btn-success" on-click={this.show()}>Confirm</button>
```

```javascript
var component = new NEKUI.Component({
    template: template,
    show: function() {
        NEKUI.Modal.confirm('Confirm内容');
    }
});
```
<!-- demo_end -->