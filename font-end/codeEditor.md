# contenteidtorable的外边框
> 在focus时，会显示出蓝色outline外边框，设置为none就行  
``` css
.editor:focus {
    outline: none
}
```

# 关于keyDown在contenteditorable的定时器调用
这样就可以在字符显示后调用处理函数
``` javascript
  let test = document.getElementById('test');

  test.addEventListener('keydown', function () {
    setTimeout(() => {
      handler();
    }, 0);
  })
```