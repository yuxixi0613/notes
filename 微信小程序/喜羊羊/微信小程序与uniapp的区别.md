**微信小程序和uniapp的区别**

- ##### 触摸事件名称：

  > ①微信小程序：`bindtap`
  >
  > ②uni-app：`@click`

- ##### 函数传参方式：

  > ①微信小程序：`<view bindtap="click" data-id="id"></view>`
  >
  > ②uni-app：`<view @click="click(id)"></view>`

- ##### 函数接收参数：

  > ①微信小程序：`function(e){this.setData(currentId:e.currentTarget.dataset.id)}`
  >
  > ②uni-app：`function(id){this.currentId = id}`

- ##### for循环：

  > ①微信小程序：`<view wx:for="{{currentList}}" wx:for-index="s_index" wx:for-item="s_item"></view>`
  >
  > ②uni-app：`<view v-for="(s_item,s_index) in currentList"></view>`

- ##### if判断：

  > ①微信小程序：`<view wx:if="{{isShow}}"></view>`
  >
  > ②uni-app：`<view v-if="isShow"></view>`

- ##### src动态接收图片：

  > ①微信小程序：`<image src="{{item.img}}"></image>`
  >
  > ②uni-app：`<image :src="$util.img(item.img)"></image>`

- ##### 页面传参：

  > ①微信小程序：`<navigator url="/pages/live?id={{item.room_id}}"></navigator>`
  >
  > ②uni-app：`<navigator :url="'/pages/live?id=' + item.room_id"></navigator>`

  









