# `ng-form`
- Angular@1.4.7
- `ng` 模块中的指令


可嵌套表单指令的别名。HTML 规定不允许表（`form`）元素的嵌套。但是它可以用于嵌套表单。例如，
一个子组的有效性（valid）需要确定。


**注意**: `ngForm` 的目的是 `组的控制`，但是不能取代 `<form>` 标签的所有功能。例如；发送数据
（post）到服务器。

## 指令信息

这个指令的执行优先级为0级

## 用法
以元素的形式 (可以作为普通的元素使用，但是要注意 IE 的限制).

``` html
<ng-form [name="string"]>
...
</ng-form>
```

以元素属性的形式使用:

``` html
<ANY [ng-form="string"]>
...
</ANY>
```

以 CSS 类使用:

``` html
<ANY class="[ng-form: string;]">
...
</ANY>
```

#### 参数

| 参数 | 形式 | 详细 |
|:----|:---:|:----|
|`ngForm` 或 `name` (可选)|`string`| 表的名字，如果被指定了，这个表的控制器就会被发布到关联的作用域（`scope`）中。.|