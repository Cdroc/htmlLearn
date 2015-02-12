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