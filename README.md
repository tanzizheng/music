##--wxml--
<open-data>标签type="userAvatarUrl"属性获取用户头像(只能用来展示)
<navigator>跳转标签hover-class="none"属性去掉默认样式
<button>属性open-type="share"//触发分享函数
<scroll-view>属性scroll-y="true"//可使页面垂直滚动
scroll-with-animation="true"在设置滚动条位置时使用动画过渡
  scroll-top设置顶部滚动偏移量，仅在设置了 overflow-y: scroll 成为滚动元素后生效
<form>//表单设置report-submit="true"表单推送才生效
<textarea/>//多行文本域fixed="true"属性让其固定
<isLyricShow>可滚动视图区域,放歌词
if (!wx.cloud)是否使用云开发
traceUser: true记录访问过的用户
this.globalData = {}全局的属性或者方法
"sitemapLocation": "sitemap.json"小程序的内部搜索
"miniprogramRoot": "miniprogram/"前端代码
	"cloudfunctionRoot": "cloudfunctions/"云服务代码
  wx.cloud.callFunction({})调用云函数
  #--swiper属性
  indicator-dots="true"轮播图小点点
  autoplay="true"轮播图是否自动播放 
  interval="2000"多久切换一次 duration="1000"花费时长多久
  #--image属性
  mode="widthFix"宽度不变,高度自动变化;aspectFill短边正常显示长边减掉
  #--JS---
  "disableScroll":true//在(配置页)中页面不能上下滚动
  getWXContext()获取openid等用户信息
  Math.ceil//计算得到结果向上取整
  send//订阅消息,模板字符串推送,需在 config.json 中配置 subscribeMessage.send API 的权限
  triggerEvent//触发自定义事件处理函数
  wx.getSetting;//是否授权wx.getUserInfo;//获取用户信息
  where(关键字||条件)指定查询条件，返回带新查询条件的新的集合引用
  db.RegExp({//云函数数据库模糊搜索
          regexp:keyword,//关键字
          options:'i'//不分大小写
        })
  getCurrentPages()取到当前小程序中的界面
  RegExp.$1指的是与正则表达式匹配的第一个子匹配(.$1标志)字符串
  replace() 方法用于在字符串中用一些字符替换另一些字符，或替换一个与正则表达式匹配的子串
  test() 方法用于检测一个字符串是否匹配某个模式
  JavaScript中可以在某个元素前使用  '+'  号，这个操作是将该元素转换成Number类型，如果转换失败，那么将得到 NaN
  new Date()//可以获取当前时间并接受所给予的时间变量以时间对象的形式打印出来
  wx.navigateBack()//关闭当前页面，返回上一页面或多级页面。可通过 getCurrentPages 获取当前的页面栈，决定需要返回几层
  trim() 方法用于删除字符串的头尾空格
  exec() 方法用于检索字符串中的正则表达式的匹配
  Date.now()//返回1970年到现在的毫秒数
  wx.chooseImage()//从本地相册选择图片或使用相机拍照
  wx.cloud.uploadFile()//将本地资源上传至云存储空间
  previewImage()图片预览
  splice(开始位置,长度)//删除数组里面的元素
  *this //会校正带有 key 的组件，框架会确保他们被重新排序，而不是重新创建，以确保使组件保持自身的状态，并且提高列表渲染时的效率。
  auto-focus//自动获取焦点bindfocus//获取焦点bindblur//失去焦点
  open-type="getUserInfo"按钮的开放能力//获取当前用户的数据信息  bindgetuserinfo="自定义函数"//事件处理函数
  pageLifetimes://组件所在页面的生命周期lifetimes://组件生命周期

  
  match()查找相同的字符(通常和正则一起使用)方法可在字符串内检索指定的值，或找到一个或多个正则表达式的匹配,它返回指定的值，
  forEach() 方法用于调用数组的每个元素，并将元素传递给回调函数。
  observers:{}监听函数
  parseFloat() 函数可解析一个字符串，并返回一个浮点数。
  promise.all()所有完成之后
  promise.race()有的完成了之后 
  [...'hello']// [ "h", "e", "l", "l", "o" ]扩展运算符还可以将字符串转为真正的数组。
  对象中的扩展运算符(...)用于取出参数对象中的所有可遍历属性，拷贝到当前对象之中
  .count()返回的是对象有->属性   .total记录条数
  #--
  从第几条开始取.skip()指定查询返回结果时从指定序列后的结果开始返回，常用于分页
  .limit(...)取的条数，数量上限
  reduce('初始值','当前元素')对象实例，计算数组元素相加后的总和，说白了就是累加器。
  orderBy('属性名','desc')指定查询排序条件
  #--json
  multipleSlots: true// 启用多个插槽
  "enablePullDownRefresh":true打开下拉 wx.stopPullDownRefresh()//停止下拉动画
#--css
text-shadow//文字阴影
flex-direction: row;默认值。灵活的项目将水平显示，正如一个行一样column属性值灵活的项目将垂直显示，正如一个列一样。
:nth-child(3n)//选中3的倍数的元素
flex-wrap: wrap;规定灵活的项目在必要的时候拆行或拆列。
externalClasses[]子组件接收外部样式类
align-items: center;/*水平居中*/
 justify-content: center;/*垂直居中*/space-between属性两端对齐
 filter blur(px)给图像设置高斯模糊
  box-sizing: border-box;对元素指定宽度和高度包括了 padding 和 border 
   align-items: center;居中对齐弹性盒的各项
   font-weight:文本的粗细
   flex-grow 属性用于设置或检索弹性盒子的扩展比率 需加width:0
  (overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;)这三个配套使用显示...
  transform:translate(x,y)括号里的值为百分数时，会以目前元素本身的宽高做参考，比如，目前元素本身的宽为100px，高为50px， 那填(50%,50%)，则表示就是向右移动50px、向下移动25px（正百分数），添加负号（负百分数）就是向着相反的方向移动，即左、上
#--自定义属性
data-自定义名称---->在currentTarget.dataset.自定义名称
wx.setStorageSync(唯一标识,数据)把数据存储到本地wx.getStorageSync(唯一标识)
wx.setNavigationBarTitle()导航标题
background-size中的cover会缩放至图片能够铺满整个容器，而contain则是图片会缩放至整个图片都能显示完全，但是容易可能会有留白
transform: rotate(-30deg);设置旋转
transform-origin:99% 99%;设置旋转元素的基点位置
transition:(参数一动画属性如transform,参数二几秒内完成,参数三动画样式)//动画过滤
animation-play-state: paused;让动画暂停在那一刻停下
flex:1;让弹性盒模型元素都有相同的长度，且忽略它们内部的内容
flex: 1;/*搜索图标占位整个父元素1份*/
flex: 1;/*让所有弹性盒模型对象的子元素都有相同的长度，且忽略它们内部的内容：*/
bindchange拖动进度条的时候触发的事件;bindtouchend松开进度条时触发的事件
backgroundAudioManager.seek()//让音乐播放时间定为到当前移动的进度位置的时间
##--组件间通信与事件
this.triggerEvent('自定义事件')//触发自定义事件(bind:自定义事件="事件函数")//triggerEvent触发类似手枪扳机
