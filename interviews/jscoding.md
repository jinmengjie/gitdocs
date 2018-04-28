#### 页面内有一个正方形元素A以及一个待放置区域B，实现对其拖拽和放下到B区域内，并且改变B区域的背景颜色

见`./demos/drag.html`

#### 实现超出整数存储范围的两个大正整数相加，function add(a,b)。参数a、b及函数的返回值都是字符串

```javascript
    function add(a, b) {
        var carry = 0, result = [],
            len = Math.max(a.length, b.length), i = len;
        while (i--) {
            var sum = (+a[i - len + a.length]||0) + (+b[i - len + b.length]||0) + carry;
            carry = parseInt(sum / 10);
            result.unshift(sum % 10);
        }
        if (carry) result.unshift(carry);
        return result.join('');
    }
```

#### 页面内有一个input输入框，实现在数组arr查询命中词并和autocomplete效果

见`./demos/autocomplete.html`

