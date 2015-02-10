HTML -- Hypertext Markup Language -- 超文本标记语言
                                  -- 超文本（含有指向其它文本文件链接的文本）
     -- 不是一种“编程语言”，而是一种“标记语言”
     -- 标记语言是一套“标记标签”
     -- HTML使用标记标签来描述网页
     -- 注释 -- <!-- This is a comment -->
     -- 在显示页面时，浏览器会移除源代码中多余的空格和空行，
        所有连续的空格或空行都会被算作一个空格，
        HTML代码中的所有连续的空行（换行）也被显示为一个空格（&nbsp;）
-----------------------------------------------------------------------------
HTML标签 -- 由尖括号包围的关键词，比如<html>

HTML文档=网页 -- 包含HTML标签和纯文本

HTML元素 -- 指从开始标签到结束标签的所有代码
         -- 开始标签（开放标签）、结束标签（闭合标签）
         -- 元素内容 -- 开始标签与结束标签之间的内容
         -- 空元素   -- 没有内容的HTML元素
                     -- 在开始标签中进行关闭（以开始标签的结束而结束）

<body>元素 -- 定义了HTML文档的主体
<html>元素 -- 定义了整个HTML文档
<br />     -- 定义换行 -- 空行
-----------------------------------------------------------------------------
HTML标题   -- h1 h2 h3 h4 h5 h6
           -- 默认情况下，HTML会自动地在块级元素前后添加一个额外的空行
HTML段落   -- p
HTML链接   -- a       -- href属性指定链接地址
                      -- href(hypertext reference) -- 超文本引用（超链接）
HTML图像   -- <img /> -- src属性指定图片地址
HTML表格   -- table
HTML水平线 -- <hr />

文本格式化标签 -- b      -- 粗体文本
               -- big    -- 大号字
               -- em     -- 着重文字
               -- i      -- 斜体字
               -- small  -- 小号字
               -- strong -- 加重语气
               -- sub    -- 下标字
               -- sup    -- 上标字
               -- ins    -- 插入字
               -- del    -- 删除字
               -- s      -- 不赞成使用，使用<del>代替
               -- strike -- 不赞成使用，使用<del>代替
               -- u      -- 不赞成使用，使用样式(style)代替

计算机输出标签 -- code      -- 计算机代码
               -- kbd       -- 键盘码
               -- samp      -- 计算机代码样本
               -- tt        -- 打字机代码
               -- var       -- 变量
               -- pre       -- 预格式文本
               -- listing   -- 不赞成使用，使用<pre>代替
               -- plaintext -- 不赞成使用，使用<pre>代替
               -- xmp       -- 不赞成使用，使用<pre>代替

引用和术语定义 -- abbr       -- 缩写
               -- acronym    -- 首字母缩写
               -- address    -- 地址
               -- bdo        -- 文字方向
               -- blockquote -- 长的引用
               -- q          -- 短的引用语
               -- cite       -- 引用、引证
               -- dfn        -- 一个定义项目 

基于内容的样式 -- abbr acronym cite code dfn em kbd samp strong var
物理样式       -- b biq i s small strike sub sup tt -- 应该避免使用物理样式 

style    -- 样式定义
link     -- 资源引用
div      -- 文档中的节或区域（块级）
span     -- 文档中的行内的小块或区域
font     -- 文本的字体、字体尺寸、字体颜色，不赞成使用，请使用样式
basefont -- 基准字体，不赞成使用，请使用样式
center   -- 对文本进行水平居中，不赞成使用，请使用样式

HTML超链接 -- a -- 两种使用方式 -- 通过使用href属性，创建指向另一个文档的链接
                                -- 通过使用name属性，创建文档内的书签
                -- target属性   -- target="_blank",新窗口中打开
HTML图像   -- <img /> -- src属性    -- 图像的URL地址
                      -- alt属性    -- 为图像定义一串预备的可替换的文本
                      -- usemap属性 -- 图像映射，引用map元素中的id或name属性
map        -- 图像地图
area       -- 图像地图中可点击区域  -- shape coords href target alt

HTML表格 -- table -- caption -- 标题
                  -- thead   -- 页眉
                  -- tbody   -- 主体
                  -- tfoot   -- 页脚
                  -- cellpadding属性 -- 单元格边距
                  -- cellspacing属性 -- 单元格间距
                  -- frame属性       -- 框架属性，控制围绕表格的边框
                                     -- box above below hsides vsides
                  -- tr -- 行
                        -- td -- 表格数据，即数据单元格的内容
                        -- th -- 表格的表头，大多数浏览器会把表头显示为粗体居中的文本
                              -- colspan属性 -- 跨列
                              -- rowspan属性 -- 跨行
                  -- col      -- 用于表格列的属性
                  -- colgroup -- 表格列的组
-----------------------------------------------------------------------------
属性 -- align   -- 对齐方式 -- center、bottom、middle、top、left、right
     -- bgcolor -- 背景颜色
     -- border  -- 边框
     -- class   -- 元素类名
     -- id      -- 元素唯一ID
     -- style   -- 行内样式
     -- title   -- 额外信息（可在工具提示中显示）
     -- rel     -- 外部样式表link的属性
                -- <link rel="stylesheet" type="text/css" href="mystyle.css" />
-----------------------------------------------------------------------------
-----------------------------------------------------------------------------
-----------------------------------------------------------------------------
<!DOCTYPE> -- 不是html标签，它为浏览器提供一项信息（声明），即HTML是用什么版本编写的
HTML版本   -- HTML HTML+ HTML2.0 HTML3.2 HTML4.01 XHTML1.0 HTML5 XHTML5
           -- HTML5 -- <!DOCTYPE html>
           -- HTML 4.01 -- <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
                            "http://www.w3.org/TR/html4/loose.dtd">
           -- XHTML 1.0 -- <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
                            "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
-----------------------------------------------------------------------------
HTML头部元素 -- head   -- 关于文档的信息 -- 所有头部元素的容器
             -- title  -- 文档标题
             -- base   -- 页面上所有链接的默认地址或默认目标
                       -- <base href="http://www.w3school.com.cn/images/" />
                       -- <base target="_blank" />
             -- link   -- 文档与外部资源之间的关系(常用于连接样式表)
                       -- <link rel="stylesheet" type="text/css" href="mystyle.css" />
             -- meta   -- 关于HTML文档的元数据
                       -- <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
                       -- <meta http-equiv="Refresh" content="5;url=http://www.w3chool.com.cn" />
                          -- 5秒重定向到http://www.w3school.com.cn
                       -- <meta name="*" content="*" /> -- 描述文档或定义文档的关键词
                          -- name和content属性的作用是描述页面的内容
             -- script -- 客户端脚本
             -- style  -- 文档的样式信息
-----------------------------------------------------------------------------
HTML脚本 -- script   -- 用于定义客户端脚本，比如JavaScript
                     -- <script type="text/javascript"></script> 
                        -- 必需的type属性规定脚本的MIME类型
                     -- 为防止老式浏览器的不识别，应将脚本隐藏在注释标签中
                        -- JavaScript -- <!-- //-->
                        -- VBScript   -- <!-- '-->
         -- noscript -- 提供无法使用脚本时的替代内容
                     -- 可包含普通HTML页面的body元素中能够找到的所有元素
-----------------------------------------------------------------------------
HTML字符实体 -- &entity_name;(实体名称) &#entity_number;(实体数字)
                -- 实体名称对大小写敏感
             -- 浏览器不支持所有实体名称，对实体数字的支持却很好
             --      -- 空格     -- &nbsp;   -- &#160;
             -- <    -- 小于号   -- &lt;     -- &#60;
             -- >    -- 大于号   -- &gt;     -- &#62;
             -- &    -- 和号     -- &amp;    -- &#38;
             -- "    -- 引号     -- &quot;   -- &#34;
             -- '    -- 撇号     -- &apos;   -- &#39; -- IE不支持&apos;
             -- ￠   -- 分       -- &cent;   -- &#162;
             -- £    -- 镑       -- &pound;  -- &#163;
             -- ¥    -- 日圆     -- &yen;    -- &#165;
             -- €    -- 欧阳     -- &euro;   -- &#8364;
             -- §    -- 小节     -- &sect;   -- &#167;
             -- ©    -- 版权     -- &copy;   -- &#169;
             -- ®    -- 注册商标 -- &reg;    -- &#174;
             -- ™    -- 商标     -- &trade;  -- &#8482;
             -- ×    -- 乘号     -- &times;  -- &#215;
             -- ÷    -- 除号     -- &divide; -- &#247;
-----------------------------------------------------------------------------
HTML统一资源定位器 -- URL -- Uniform Resource Locator -- 也被称为网址
                          -- 可以由单词组成，比如"w3school.com.cn"
                          -- 或是因特网协议(IP)地址：192.168.1.253
                          -- 语法规则 -- scheme://host.domain:port/path/filename
                                      -- scheme   -- 英特网的类型，最常见的类型是http
                                                     -- http  -- 超文本传输协议
                                                              -- 以http://开头的普通网页，不加密
                                                     -- https -- 安全超文本传输协议
                                                              -- 安全网页，加密所有信息交换
                                                     -- ftp   -- 文本传输协议
                                                              -- 用于将文件下载或上传至网站
                                                     -- file  -- 您计算机上的文件
                                      -- host     -- 域主机(http的默认主机是www)
                                      -- domain   -- 英特网域名，比如 w3school.com.cn
                                      -- :port    -- 主机上的端口号(http的默认端口号是80)
                                      -- path     -- 服务器上的路径
                                                     --如果省略，则文档必须位于网站的根目录中
                                      -- filename -- 文档/资源的名称
-----------------------------------------------------------------------------
HTML URL 字符编码 -- URL编码会将字符转换为可通过因特网传输的格式
                  -- URL只能使用ASCII字符集来通过因特网进行发送
                  -- URL编码使用"%"其后跟随两位的十六进制数来替换非ASCII字符
                  -- URL不嫩包含空格，URL编码通常使用 + 来替换空格
                  -- 字符 -- URL编码
                  -- €    -- %80
                  -- £    -- %A3
                  -- ©    -- %A9
                  -- ®    -- %AE
                  -- À    -- %C0
                  -- Á    -- %C1
                  -- Â    -- %C2
                  -- Ã    -- %C3
                  -- Ä    -- %C4
                  -- Å    -- %C5
