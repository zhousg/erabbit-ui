# 小兔鲜组件库

## started
```bash
// axios vue less less-loader 基于vuecli
yarn add erabbit-ui
```

```html
<!-- index.html -->
<link rel="stylesheet" href="https://at.alicdn.com/t/font_2143783_iq6z4ey5vu.css">
```

```js
import { createApp } from 'vue'
import App from './App.vue'

import ErabbitUI from 'erabbit-ui'
import 'erabbit-ui/packages/theme/index.less'

createApp(App).use(ErabbitUI).mount('#app')
```


## docs

### 面包屑

`xtx-bread` 

`xtx-bread-item`

props 

| 名称   | 类型   | 默认值 |
| ------ | ------ | ------ |
| to  | String, Object | 无    |

`与router-link的to属性一致`



### 按钮

`xtx-button`

| 名称  | 类型   | 可选值                     | 默认值  |
| ---- | ------ | -------------------------- | ------- |
| size | String | large/middle/small/mini    | middle  |
| type | String | default/primary/plain/gray | default |



### 轮播图

`xtx-carousel`

props

| 名称     | 类型    | 默认值 |
| -------- | ------- | ------ |
| sliders  | Array   | []     |
| autoPlay | Boolean | false   |
| duration | Number | 3000毫秒   |

`:sliders="[{imgUrl:'图片地址'}]"`


### 复选框

`xtx-checkbox`

props

| 名称     | 类型    | 默认值 |
| -------- | ------- | ------ |
| v-model  | Boolean   | false    |


### 地区选择

`xtx-city`

props

| 名称     | 类型    | 默认值 |
| -------- | ------- | ------ |
| placeholder  | String   | ''    |
| fullLocaton  | String   | ''    |

events

| 名称     | 触发时机    | 默认参 |
| -------- | ------- | ------ |
| change  | 选择完成   | { fullLocaton, provinceCode, provinceName, cityCode, cityName, countyCode, countyName }    |


### 对话框

`xtx-dialog`

props

| 名称     | 类型    | 默认值 |
| -------- | ------- | ------ |
| v-model:visible  | Boolean   | false   |



### 图片预览组件

组件名称：`xtx-image-view`

props

| 名称      | 类型  | 默认值 |
| --------- | ----- | ------ |
| images | Array | []     |

`[] 图片数组`



### 无限加载组件

`xtx-infinite-loading`

props

| 名称  | 类型   | 默认值                  |
| ----- | ------ | ------ |
| loading 加载中 | Boolean | false |
| finished 全部数据加载完成 | Boolean | false |


events 

| 名称     | 触发时机    | 默认参 |
| -------- | ------- | ------ |
| infinite  | 进入可视区   |  无  |


### 更多组件

`xtx-more` 

props 

| 名称   | 类型   | 默认值 |
| ------ | ------ | ------ |
| to  | String, Object | 无    |

`与router-link的to属性一致`


### 数字选择

`xtx-numbox` 

props 

| 名称   | 类型   | 默认值 |
| ------ | ------ | ------ |
| label  | String | ''    |
| v-model  | Number | 0   |
| min  | Number | 0    |
| max  | Number | 10    |


### 分页组件

`xtx-pagination`

props

| 名称  | 类型   | 默认值                  |
| ----- | ------ | ------ |
| total 总条数 | Number | 100 |
| pageSize 每页条数 | Number | 10 |
| currentPage 当前第几页 | Number | 1 |


events 

| 名称     | 触发时机    | 默认参 |
| -------- | ------- | ------ |
| current-change  | 改变分页页码   |  点击的页码  |


### 骨架组件

`xtx-skeleton`

props

| 名称  | 类型   | 默认值                  |
| ----- | ------ | ------ |
| bg 背景 | Number | #efefef |
| width 宽 | String | 100px |
| height 高 | String | 100px |
| animated 闪动画 | Boolean | false |


### sku组件

props

| 名称  | 类型   | 默认值                  |
| ----- | ------ | ----------------------- |
| goods | Object | { specs: [], skus: [] } |
| skuId | String | '' |

events

| 名称   | 回调参数                                 |
| ------ | ---------------------------------------- |
| change | 完整的sku对象数据 （不完整时为空对象{}） |

`{skuId,price,oldPrice,inventory,specsText}`



### 步骤条

`xtx-steps`

props

| 名称 | 类型   | 默认值  |
| ---- | ------ | ------- |
| active 当前到第几步 | Number    | 1  |

`xtx-steps-item`

props

| 名称 | 类型   | 默认值  |
| ---- | ------ | ------- |
| title 标题 | String    | ''  |
| desc 说明 | String    | ''  |


### tab栏

`xtx-tabs`

props

| 名称 | 类型   | 默认值  |
| ---- | ------ | ------- |
| v-model  | String,Number    | ''  |

events

| 名称 | 触发时机   | 默认值  |
| ---- | ------ | ------- |
| tab-click  | 点击选项卡    | { name, index }  |

`{name:'选项卡名称',index:'选项卡索引'}`


`xtx-tabs-item`

props

| 名称 | 类型   | 默认值  |
| ---- | ------ | ------- |
| label 选项卡标题 | String    | ''  |
| name 选项卡名称 | String    | ''  |


## about

email: zhoushugang@itcast.cn
github: https://github.com/zhousg