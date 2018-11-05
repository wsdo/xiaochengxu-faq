##  微信小程序写点击事件,并且在dom携带参数？
#### 在dom属性上添加 bindtap属性
```html （wxml）
<view class="option"  bindtap="nextQuestion" data-id="18" data-answer='3'>
    <image class="optionBg" src="./option.png"></image>
</view>
```
```js
 nextQuestion: function (e) {
    let params = e.currentTarget.dataset
    // 获取id
    let questionId= params.id
     // 在这写函数要做的事情
     console.log('在这写函数要做的事情')
 }
```
> 其中nextQuestion就是点击事件