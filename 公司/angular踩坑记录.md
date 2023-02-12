# angular踩坑记录





### 关于component与module

> 一个[component](https://so.csdn.net/so/search?q=component&spm=1001.2101.3001.7020)只能属于一个module，在test.module.ts中引入TestComponent后，在app.module.ts中的declarations中不能在引入TestComponent，否则会报错！





### 关于表单

> 使用了[angular](https://so.csdn.net/so/search?q=angular&spm=1001.2101.3001.7020)的响应式表单，formGroup是指定命令的选择器,它是ReactiveFormsModule的一部分