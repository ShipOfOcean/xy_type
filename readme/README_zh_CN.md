# xy_type

- zh_CN [简体中文](README_zh_CN.md)
- zh_TW [繁体中文](README_zh_TW.md)
- en [English](README_en.md)

# 说明
类型工具.

<a href="https://github.com/ShipOfOcean/xy_type.git" target="_blank">Github地址</a>

## 安装

```
pip install xy_type
```

## 开始

```python
from xy_type.utils import count_of_function_arguments, validate_callable_func, validate_callable_init_func, has_func, empty_value

class xyObject:

    def __init__(self, arg_0=0, arg_1=1):
        pass

    def xyFunc(self, arg_0=0, arg_1=1):
        pass

    @classmethod
    def xyClsFunc(cls, arg_0=0, arg_1=1)
        pass

count_of_function_arguments(xyObject.xyClsFunc)
# 2

validate_callable_func(xyObject.xyClsFunc)
# True

validate_callable_init_func(xyObject, 1)
# True

obj = xyObject()
has_func(obj, "xyFunc", 2)
# True
has_func(obj, "xyFunc1", 2)
# False
has_func(obj, "xyFunc", 20)
# False

empty_value(obj, xyObject, None)
# obj

empty_value(obj, str, None)
# None

```

## 捐赠

如果小伙伴们觉得这些工具还不错的话，能否请咱喝一杯咖啡呢
<br />
![微信](WeChat.png)
![支付宝](Alipay.png)


## 联系方式

```
微信: yuyangitt
邮箱: 845262968@qq.com
```