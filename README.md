# LrcView
# 一个关于音乐播放器歌词控件显示的自定义View
## 效果图如下：  
![6](https://cloud.githubusercontent.com/assets/6023444/19617794/6299ccc2-986c-11e6-8cd3-2cca2ac36003.gif)

## 使用方式

> 下载该类库作为一个module引入到您的项目中
> 布局文件中添加控件
> java代码中设置歌词并开启绘制


### 代码举例--布局文件
```
<org.sang.lrcview.LrcView
                android:id="@+id/lrc_view"
                android:layout_width="match_parent"
                app:lrcMode="KARAOKE"
                android:layout_height="match_parent"/>
```
**lrcMode表示歌词显示的模式，默认为普通模式，可以开启卡拉OK模式，另外也可以配置高亮歌词的颜色和普通歌词的颜色**
### 代码举例--Java代码
```
lrcView.setLrc(lrcStr);
        lrcView.setPlayer(PlayUtil.player);
        lrcView.init();
```
