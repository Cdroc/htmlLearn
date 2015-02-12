XHTML -- EXtensible Hypertext Markup Language -- 可扩展超文本标记语言
      -- 是一个W3C标准，是HTML与XML(扩展标记语言)的结合物，
      -- XML用来描述数据，而HTML则用来显示数据
      -- 必须拥有DOCTYPE声明，并且html/head/title/body元素必须存在
-----------------------------------------------------------------------------
XHTML语法 -- XHTML元素必须被正确的嵌套
          -- XHTML元素必须被关闭
          -- 标签名必须用小写字母
          -- XHTML文档必须拥有跟元素
          -- 属性名必须小写
          -- 属性值必须加引号
          -- 属性不能简写 -- compact/checked/declare/readonly/disabled/selected/
                             defer/ismap/nohref/noshade/nowrap/multiple/noresize
          -- 用id属性代替name属性
          -- XHTML DTD定义了强制使用的HTML元素 -- html/head/body/title
                                               -- 文件类型声明 -- <!DOCTYPE >
                                               -- html标签内的xmlns属性是必需的
                                               -- <html xmlns="http://www.w3.org/1999/xhtml"></html>
          -- 语言属性(lang) -- 定义元素内部的内容的所用语言的类型
                            -- 在元素中使用lang属性，就必须添加额外的xml:lang
                            -- <div lang="no" xml:lang="no">Heia Norge!</div>
-----------------------------------------------------------------------------
XHTML DTD -- <!DOCTYPE >是强制使用的
          -- 三种文档类型声明 -- STRICT       -- 严格类型 -- 需要干净的标记，避免表现上的混乱，
                                                             请与层叠样式表配合使用
                                 -- <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" 
                                     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
                              -- TRANSITIONAL -- 过渡类型 -- 需要利用HTML在表现上的特性，
                                                             为不支持层叠样式表的浏览器编写XHTML
                                 -- <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
                                    "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
                              -- FRAMESET     -- 框架类型 -- 需要使用HTML框架将浏览器窗口
                                                             分割为两部分或更多框架时
                                 -- <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN"
                                    "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">
-----------------------------------------------------------------------------
XHTML模块 -- W3C已将XHTML的定义分为28种模型 -- 已被废弃的元素不应被用于XHTML之中

XHTML属性 -- 标准属性        -- 属性        -- 值                     -- 描述
             -- 核心属性     -- class       -- class_rule或style_rule -- 元素的类
                             -- id          -- id_name                -- 元素的某个特定id
                             -- style       -- 样式定义               -- 内联样式定义
                             -- title       -- 提示文本               -- 显示于提示工具中的文本
                             (base/head/html/meta/param/script/style/title元素不支持)
             -- 语言属性     -- dir         -- ltr或rtl               -- 设置文本的方向
                             -- lang        -- 语言代码               -- 设置语言代码
                             (base/br/frame/frameset/hr/iframe/param/script元素不支持)
             -- 键盘属性     -- accesskey   -- 字符                   -- 设置访问某元素的键盘快捷键
                             -- tabindex    -- 数                     -- 设置某元素的Tab次序
          -- 事件属性      
             -- 窗口事件     -- onload      -- 脚本                   -- 当文档被载入时执行脚本
                             -- onunload    -- 脚本                   -- 当文档被卸下时执行脚本
                             (仅在body和frameset元素中有效)
             -- 表单元素事件 -- onchange    -- 脚本                   -- 当元素改变时执行脚本
                             -- onsubmit    -- 脚本                   -- 当表单被提交时执行脚本
                             -- onreset     -- 脚本                   -- 当表单被重置时执行脚本
                             -- onselect    -- 脚本                   -- 当元素被选取时执行脚本
                             -- onblur      -- 脚本                   -- 当元素失去焦点时执行脚本
                             -- onfocus     -- 脚本                   -- 当元素或得焦点时执行脚本
                             (仅在表单元素中有效)
             -- 键盘事件     -- onkeydown   -- 脚本                   -- 当键盘被按下时执行脚本
                             -- onkeypress  -- 脚本                   -- 当键盘被按下后又松开时执行脚本
                             -- onkeyup     -- 脚本                   -- 当键盘被松开时执行脚本
                             (base/bdo/br/frame/frameset/head/html/iframe/meta/param/script/style/title元素不支持)
             -- 鼠标事件     -- onclick     -- 脚本                   -- 当鼠标被单击时执行脚本
                             -- ondblclick  -- 脚本                   -- 当鼠标被双击时执行脚本
                             -- onmousedown -- 脚本                   -- 当鼠标按钮被按下时执行脚本
                             -- onmousemove -- 脚本                   -- 当鼠标指针移动时执行脚本
                             -- onmouseout  -- 脚本                   -- 当鼠标指针移出某元素时执行脚本
                             -- onmouseover -- 脚本                   -- 当鼠标指针悬停于某元素之上时执行脚本
                             -- onmouseup   -- 脚本                   -- 当鼠标按钮被松开时执行脚本
                             (base/bdo/br/frame/frameset/head/html/iframe/meta/param/script/style/title元素不支持)