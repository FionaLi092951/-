# - GOOD GOOD STUDY  

职位名称：国际技术事业部-Lazada-海外电商-前端开发(杭州/新加坡)
职位描述：去年四月我们投资并购了东南亚第一电商Lazada，然后利用半年时间成功实现了商家端的整合，目前在继续搜索、数据平台等业务的输出，真正利用阿里巴巴先进成熟的产品和技术快速提升海外本地电商的能力，帮助阿里生态迅速发展海外业务。与此同时，我们在基于阿里已有平台抽取出一套国际化的全链路系统，从无线手机端到交易链路，从商家业务到大数据和推荐，打造全新的端到端国际电商操作系统，并在未来多个海外收购公司实现复用。今年二月又投资了印度PayTM电商，开启了第二战场，阿里国际化进入了轰轰烈烈的执行阶段。在这里你不仅有机会了解阿里商品、交易、会员、营销等核心平台，而且有机会接受极具前瞻性的海外电商业务的挑战，并且需要针对多国场景进行业务抽象和平台剥离，任务的新颖性和挑战性都是前所未有的。岗位包含产品、架构师、开发、测试、前端等各类角色，业务涉及电商端到端的所有环节，只要你自信，有能力、有激情，一定可以找到吸引自己的新挑战。机会只有一次，期待你的加入，参与阿里国际化大战略，和我们一起共创阿里的未来！

职位要求：

1、至少3年以上前端开发经验，精通HTML、CSS、JS，熟悉页面架构和布局，对表现与数据分离、Web语义化等有深刻理解

2、良好的编程习惯，至少掌握一种以下语言，如 PHP、Java、Python、nodeJs

3、熟悉HTTP协议及缓存,了解基本的浏览器渲染及网络传输过程，熟悉跨终端、跨浏览器的开发模式

4、有NativeApp，HTML5/CSS3 移动开发经验优先，有英语沟通能力的优先

5、有良好沟通和团队协作能力、有很强的心里素质和责任心，持续推动拿结果

6、有良好英语沟通者优先考虑， 也可酌情降低技术能力要求



【套1】 https://juejin.im/post/59316e682f301e0058378558


【HTML】

1.HTML5新增功能和API

  功能：音频&视频播放，canvas，svg，语义化标签（header, footer, artical)， 表单控件(email, number），表单属性（autocomplete, autofocus)...
  
  API: outerHTML, getElementsByClassName(), classList, postMessage, Web Worker, Web Socket, Drag & Drop ...
  
  （1）Canvas&SVG对比?
  
  （2）什么是Web Socket? 
  
  （3）实现一个拖拽？
  
  （4）postMessage实现跨域？
  
  （5）outerHTML 
  
2. input和textarea的区别

   input: 单行输入框，不可自动换行，一般用于输入少数文字
   
   textarea：多行输入框，可自动换行
   

3. 用一个div模拟textarea的实现

   <div contenteditable="true" style="width:200px; height:200px; background-color:pink;word-wrap:break-word;overflow-y:auto">
	A textarea implemented with div
   </div>

4. 移动设备忽略将页面中的数字识别为电话号码的方法 

  <meta name="format-detection" content="telephone=no" />
  
  <meta name="format-detection" content="email=no" />
  
  <meta name="format-detection" content="address=no" />
  
  <meta name="format-detection" content="date=no" />
  


【CSS】

1. 左右布局：左边定宽、右边自适应，不少于3种方法

   https://www.cnblogs.com/wx1993/p/6727653.html
   
   方法一：左边设置左浮动，右边宽度设置100%  (父元素要有高度）
   
   方法二：左边设置浮动，下面的或者父元素清除浮动
   
   方法三：父容器设置 display：flex；left设置宽度，right部分设置 flex：1   
   

2. CSS3用过哪些新特性

   text-shadow, border-shadow, border-radius
   
   属性选择器，伪类，伪元素
   
   animation, transition, transform, display:flex盒子模型
   
   
3. BFC、IFC
	
   BFC是一个独立的渲染区域，区域内元素的布局，不会影响外部元素
   
   BFC = Block Fomatting Contexts = 块级格式化上下文 
   
   https://zjy.name/archives/bfc-introduction.html
   
   对内部元素的包裹性：
   
   - 能包裹float元素，不会造成父元素高度的坍塌 => 比如使用overflow, clear:both清楚浮动，或者使父元素也变成float,这样也形成了一个独立的渲染区域。
   
   - 能包裹margin，父元素和子元素margin重叠时，会发生margin折叠，如果只设置了子元素的margin，会导致父子元素同时向下推移，而不是父元素把子元素向下推      移。 把父元素设置成overflow: hidden,让父元素变成一个BFC， margin不会发生在BFC父元素和子元素之间。
   
   对外部元素的独立性： 不会和浮动元素重叠
   
   
   满足以下任意一条可以创建BFC: 
   
   * float的值不为none。
   
   * overflow的值不为visible。
   
   * display的值为table-cell, table-caption, inline-block中的任何一个。
   
   * position的值不为relative和static。
   

4. 清楚浮动的方法

   伪元素： .father:after {content: ".", visibility: none; clear:both}
   
   在float元素之后加一个元素设置clear:both
   
   overflow: .father {overflow: hidden} 
   
4. 对栅格的理解

5.（水平）居中实现方式

   方法一：margin: 0 auto;
   
6.（水平&垂直）居中有哪些实现方式

   方法一： display: flex; align-items: center; justify-content:center;
   
   方法二： margin-left, margin-top: 50%; transform: translate(-50%; -50%); | margin: -150px,0,0,-100px;
   
   方法三（absolute）：position: absolute; margin:0; left:0;top:0;bottom:0;right:0;
   
   
6. 像素边框问题


【JavaScript】

1. 图片懒加载 & 图片预加载

   https://www.cnblogs.com/tugenhua0707/p/3525668.html
   

   方法一：可视区加载 - http://blog.csdn.net/gy_u_yg/article/details/73132171 
   
   原理：把图片src设置成空，当scroll到当前图片时，再动态设置src 
  
   <script type="text/javascript">
	
        var aImg = document.querySelectorAll('img');
	
        var len = aImg.length;
	
        var n = 0;//存储图片加载到的位置，避免每次都从第一张图片开始遍历
	
        window.onscroll = function() {
	
            var seeHeight = document.documentElement.clientHeight; //document.documentElement -> 返回文档根节点
	    
	    var scrollTop = document.body.scrollTop || document.documentElement.scrollTop;
	    
            for (var i = n; i < len; i++) {
	    
                if (aImg[i].offsetTop < seeHeight + scrollTop) {
		
                    if (aImg[i].getAttribute('src') == '') {
		    
                        aImg[i].src = aImg[i].getAttribute('guoyu-src');
			
                    }
		    
                    n = i + 1;
		    
                }
            }
        };
	
    </script>
    
    方法二：延迟加载，setTimeOut() & setTimeInterval()
    
    方法三：条件加载，符合某些条件或者触发某些事件才加载
    
    
    预加载： 提前加载图片，当用户需要查看时可直接从本地缓存中渲染。
    
    function loadImage(url,callback) {
    
	    var img = new Image();

	    img.src = url;

	    if(img.complete) {  // 如果图片已经存在于浏览器缓存，直接调用回调函数

		callback.call(img); 
		
		return; // 直接返回，不用再处理onload事件
	    }

	    img.onload = function(){
		img.onload = null;
		callback.call(img);
	    }
    }


2. 实现页面加载进度条
   
   两个div，一个是进度条框，一个是进度条进程框inner,动态设置inner宽度
   
   随机时间，随机进度，设置inner宽度，保证宽度小于98%， window.onload触发时，设置宽度100%。
   
   
【性能优化】

1. 项目中使用过哪些优化方法


2. 输入一个URL，Enter之后发生了什么
   
   http://www.jianshu.com/p/5d750867897a
   
   URL = 协议 + 域名（IP）+ 端口（80）+ 路径 + 查询条件
   
   
   Step1: DNS查询 - 浏览器根据域名找到对应的IP地址 
   
          DNS查找过程为：浏览器缓存（30s-2min）->系统缓存->路由器缓存->ISP DNS缓存->递归搜索（从根域名服务器到顶级域名服务器到你查询的域名服务器）
   
   
   Step2: 建立TCP连接，三次握手。   
   
   应用层(http, https, ftp) - 传输层(tcp,udp 增加端口号) - 网络层(ip 增加ip地址) - 数据链路层(增加mac地址）


   Step3: 发送请求
   
   请求头 ＝ http版本，请求类型 get/post/put/delete, cache, etag & last-modified, 浏览器信息, 能接受的文件格式等
   
   请求body = 取决于请求类型
   
   get和post区别： ？
   
   
   Step4: 浏览器返回
   
   返回头：http版本，返回文件格式，etag等缓存信息，文件格式，服务器信息，状态码
   
   返回body： 返回内容
   
   状态码： 1*＊， 2*＊， 3*＊， 4*＊， 5*＊
   
   
   Step5: 解析HTML以构建DOM树 ==> 构建Render树（DOM+CSS) ==> 布局Render树(每个节点坐标) ==> 绘制Render树


  
   
   
3. （承上）页面的渲染过程


4. 优化中会提到缓存的问题，问：静态资源或者接口等如何做缓存优化


5. 页面DOM节点太多，会出现什么问题？如何优化？








1. Git & GitHub

   http://www.cnblogs.com/onetwo/p/4157610.html
   
   Git & SVN的区别？ 分布式-集中式
   
   
	
2. 代码模块化，模块化打包工具


3. HTTP请求全过程


4. 浏览器渲染


eBay: 
1. Cloud IAAS, PAAS, SASS
