XHTML -- EXtensible Hypertext Markup Language -- 可扩展超文本标记语言
      -- 是一个W3C标准，是HTML与XML(扩展标记语言)的结合物，
      -- XML用来描述数据，而HTML则用来显示数据
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
          -- XHTML DTD定义了强制使用的HTML元素
          -- 语言属性(lang) -- 定义元素内部的内容的所用语言的类型
                            -- 在元素中使用lang属性，就必须添加额外的xml:lang
                            -- <div lang="no" xml:lang="no">Heia Norge!</div>