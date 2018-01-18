# EscapeCharacter.js

标签： html转义字符

---

 1. 写这个js的初衷是在将用户输入的信息保存相应的文字，而不是转义字符。所以专门写了这个js。
 2. 个人不是很擅长js，如果我写的有问题或者有更好更简单的方法，请多多指教。

##方法调用
> * specialwordList 是所有的特殊字符
> * transWordList 是所有对应的转义字符

###用例

```python    
    //特殊字符 -> 转义字符
    var schar = '>';
    var tchar = sw2tw_char(schar); //&gt;
    
    //转义字符 -> 特殊字符
    var tchar2 = '&gt;';
    var schar2 = tw2sw_char(tchar2); //'>'
    
    //特殊字符串 -> 转义字符串
    var sStr = "fd>123";
    var tStr = sw2tw_string(sStr); //fd&gt;123
    
    //转义字符串 -> 特殊字符串
    var tStr2 = "fd&gt;123";
    var sStr2 = tw2sw_string(tStr2); //fd>123
```
    



