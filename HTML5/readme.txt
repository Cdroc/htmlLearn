HTML5 -- 将成为HTML、XHTML以及HTML DOM的新标准
      -- 新特性 -- 用于绘画的canvas元素
                -- 用于媒介回放的video和audio元素
                -- 对本地离线存储的更好的支持
                -- 新的特殊内容元素，如：article/footer/header/nav/section
                -- 新的表单控件，如：calendar/date/time/email/url/search
-----------------------------------------------------------------------------
HTML5视频 -- video -- 格式 -- Ogg   -- 带有Theora视频编码和Vorbis音频编码的Ogg文件
                           -- MPEG4 -- 带有H.264视频编码和AAC音频编码的MPEG4文件
                           -- WebM  -- 带有VP8视频编码和Vorbis音频编码的WebM文件
                   -- 属性 -- autoplay="autoplay" -- 视频在就绪后马上播放
                           -- controls="controls" -- 向用户显示控件，如播放按钮
                           -- height="像素"       -- 设置视频播放器的高度
                           -- loop="loop"         -- 当媒介文件播放后再次开始播放
                           -- preload="preload"   -- 视频在页面加载时进行加载并预备播放，
                                                     如果使用autoplay，则忽略该属性
                           -- src="资源路径"      -- 要播放的视频的URL
                           -- width="像素"        -- 设置视频播放器的宽度
                   -- 实例 -- <video width="320" height="240" controls="controls">
                                  <source src="movie.ogg" type="video/ogg">
                                  <source src="movie.mp4" type="video/mp4">
                                  Your browser does not support the video tag.
                              </video>
                   -- DOM  -- 方法 -- play() pause() load() canPlayType
                           -- 属性 -- currentSrc/currentTime/videoWidth/videoHeight/duration/
                                      ended/error/paused/muted/seeking/volume/height/width
                           -- 事件 -- play/pause/progress/error/timeupdate/ended/abort/empty/
                                      emptied/waiting/loadedmetadata
-----------------------------------------------------------------------------
HTML5音频 -- audio -- 格式 -- Ogg Vorbis
                           -- MP3
                           -- Wav
                   -- 属性 -- autoplay="autoplay" -- 音频在就绪后马上播放
                           -- controls="controls" -- 向用户显示控件，如播放按钮
                           -- loop="loop"         -- 当音频结束时重新开始播放
                           -- preload="preload"   -- 音频在页面加载时进行加载并预备播放，
                                                     如果使用autoplay，则忽略该属性
                           -- src="资源路径"      -- 要播放的音频的URL
                   -- 实例 -- <audio controls="controls">
                                  <source src="song.ogg" type="audio/ogg">
                                  <source src="song.mp3" type="audio/mpeg">
                                  Your browser does not support the audio tag.
                              </audio>
-----------------------------------------------------------------------------
HTML5拖放 -- 设置拖放 -- draggable="true"
          -- 拖动什么 -- ondargstart
          -- 放到何处 -- ondragover
          -- 进行放置 -- ondrop
-----------------------------------------------------------------------------
HTML5画布 -- canvas -- 是一个矩形区域，可以控制每一像素
                    -- 使用JavaScript在网页上绘制图像
                    -- getContext("2d") -- 返回一个用于在画布上绘图的环境

HTML5 SVG -- Scalable Vector Graphics -- 可伸缩矢量图
                                      -- 使用XML格式定义图形

HTML5地理定位 -- Geolocation -- 用于定位用户的位置
                             -- getCurrentPosition()方法获得用户的位置
                                -- coords.latitude         -- 十进制数的纬度
                                -- coords.longitude        -- 十进制数的经度
                                -- coords.accuracy         -- 位置精度
                                -- coords.altitude         -- 海拔，海平面以上以米计
                                -- coords.altitudeAccuracy -- 位置的海拔精度
                                -- coords.heading          -- 方向，从正北开始以度计
                                -- coords.speed            -- 速度，以米/每秒计
                                -- timestamp               -- 响应的日期/时间
                             -- watchPosition()返回用户的当前位置，
                                并继续返回用户移动时的更新位置
                             -- clearWatch()停止watchPosition()方法
-----------------------------------------------------------------------------
HTML5 Web 存储 -- 在客户端存储数据 -- localStorage   -- 没有时间限制的数据存储
                                   -- sessionStorage -- 针对一个session的数据存储
                                   (之前这些都是由cookie完成的)
                                   -- 使用JavaScript来存储和访问数据

HTML5应用程序缓存 -- Application Cache
                  -- 通过创建cache manifest文件，可以轻松地创建web应用的离线版本
                  -- 如需启用应用程序缓存，请在文档的<html>标签中包含manifest属性
-----------------------------------------------------------------------------
HTML5 Web Workers -- 是运行在后头的JavaScript，不会影响页面的性能
                  -- if (typeof(Worker) !== "undefined") -- 检测浏览器是否支持
                  -- 常用于耗费CPU资源的任务
                  -- postMessage()方法，用于向HTML页面传回一段信息
                  -- var w = new Worker("x.js"); -- 创建Web Worker对象
                  -- w.onmessage = function(event){event.data}; -- 添加监听器
                  -- w.terminate()终止web worker,并释放浏览器/计算机资源
                  -- Web Workers 和 DOM 
                     -- 由于web worker位于外部文件中，它们无法访问下例JavaScript对象
                        -- window对象、document对象、parent对象
-----------------------------------------------------------------------------
HTML5服务器发送事件 -- server-sent event 
                    -- 允许网页自动获得来自服务器的更新
                    -- EventSource对象用于接收服务器发送事件通知
                    -- 把报头 "Content-Type" 设置为 "text/event-stream"
                    -- if(typeof(EventSource)!=="undefined")
                    -- var source = new EventSource("x.php");
                    -- source.onmessage = function(event){event.data};
                    -- onopen    -- 当通往服务器的连接被打开
                    -- onmessage -- 当接收到消息
                    -- onerror   -- 当错误发生
-----------------------------------------------------------------------------
HTML5表单 -- 输入类型 -- input -- email        -- 用于e-mail地址的输入域
                               -- url          -- 用于URL地址的输入域
                               -- number       -- 用于数值的输入域
                                                  -- max   -- 最大值
                                                  -- min   -- 最小值
                                                  -- step  -- 合法的数字间隔
                                                  -- value -- 默认值
                               -- range        -- 用于一定范围内数字值的输入域，显示为滑动条
                                                  -- max   -- 最大值
                                                  -- min   -- 最小值
                                                  -- step  -- 合法的数字间隔
                                                  -- value -- 默认值
                               -- Date pickers -- 日期选择器
                                               -- date           -- 选取日、月、年
                                               -- mote           -- 选取月、年
                                               -- week           -- 选取周和年
                                               -- time           -- 选取时间(小时和分钟)
                                               -- datetime       -- 选取时间、日、月、年(UTC时间)
                                               -- datetime-local -- 选取时间、日、月、年(本地时间)
                               -- search       -- 用于搜索域，显示为常规的文本域
                               -- color
          -- 表单元素 -- datalist -- 用于输入域的选项列表
                                  -- option元素 -- 列表通过datalist内的option元素创建
                                                <datalist id="url_list">
                                                    <option label="Google" value="http://www.google.com" />
                                                </datalist>
                                                -- 输入域的list属性引用datalist的id
                                                   -- <input type="url" list="url_list" name="link" />
                                                -- option元素永远都要设置value属性
                      -- keygen   -- 用于提供一种验证用户的可靠方法
                                  -- 密钥对生成器(key-pair generator)，
                                     当提交表单时，会生成两个键，一个是私钥，一个公钥。
                                     私钥存储于客户端，公钥则被发送到服务器。
                                     公钥可用于之后验证用户的客户端证书。
                      -- output   -- 用于不同类型的输出，比如计算或脚本输出
          -- 表单属性 -- form属性  -- autocomplete   
                                   -- novalidate      -- 规定在提交表单时不应该验证 form 或 input 域
                      -- input属性 -- autocomplete    -- 规定 form 或 input 域应该拥有自动完成功能
                                   -- autofocus       -- 规定在页面加载时，域自动地获得焦点
                                   -- form            -- 规定输入域所属的一个或多个表单
                                   -- form overrides  
                                      -- formaction,formenctype, formmethod, formnovalidate, formtarget
                                   -- height/width    -- 规定用于 image 类型的 input 标签的图像高度和宽度
                                   -- list            -- 规定输入域的 datalist。datalist 是输入域的选项列表
                                   -- min/max/step    -- 用于为包含数字或日期的 input 类型规定限定（约束
                                   -- multiple        -- 规定输入域中可选择多个值
                                   -- pattern(regexp) -- 规定用于验证 input 域的模式（pattern）
                                   -- placeholder     -- 提供一种提示（hint），描述输入域所期待的值
                                   -- required        -- 规定必须在提交之前填写输入域（不能为空）