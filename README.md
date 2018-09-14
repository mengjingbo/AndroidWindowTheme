# Android Window Theme

android中常见window主题属性

### 状态栏，导航栏
|属性|取值类型|描述|
|:------|:------|:------|
|android:statusBarColor           |@color|设置系统状态栏颜色|
|android:navigationBarColor       |@color|设置系统导航栏的颜色  |
|android:navigationBarDividerColor|@color|在系统导航栏和应用程序内容之间显示指定细线的颜色|        |

### Window attributes 
|属性|取值类型|描述|
|:------|:------|:------|
|android:windowBackground               |@drawable/@color|设置window窗口背景，一般用于优化Activity启动白屏活|
|android:windowClipToOutline            |boolean|设置是否应将窗口内容剪裁为窗口背景的轮廓。|
|android:windowFrame                    |@null  |设置窗口是否有边框|
|android:backgroundDimEnabled           |boolean|设置窗口背景模糊，true:迷糊|
|android:windowNoTitle                  |boolean|设置窗口是否显示Title|
|android:windowFullscreen               |boolean|设置窗口是否全屏|
|android:windowIsFloating                 |boolean|设置窗口是否悬浮于Activity之上|
|android:windowContentOverlay           |@null|窗口内容的前景之上放置的Drawable资源|
|android:windowShowWallpaper            |boolean|是否是显示墙纸|
|android:windowTitleStyle               |@style|设置窗口title样式|
|android:windowTitleSize                |@dimen|设置窗口title size|
|android:windowTitleBackgroundStyle     |@style|设置窗口title背景样式|
|android:windowAnimationStyle           |@style|设置Dialog 进入，退出动画|
|android:windowActionBar                |boolean|设置activity是否显ActionBar|
|android:windowActionModeOverlay        |boolean|为了能够让ActionMode能够覆盖我们的Toolbar，否则会出现ActionMode将Toolbar顶下去的样子（重复出现）|
|android:windowCloseOnTouchOutside      |boolean|点击空白部分activity不消失|
|android:windowTranslucentStatus        |boolean|设置系统状态栏是否透明|
|android:windowTranslucentNavigation    |boolean|设置系统导航栏是否透明|
|android:windowDrawsSystemBarBackgrounds|boolean|状态栏不覆盖在ContentView上|
|android:windowContentTransitions       |boolean|允许使用设置转场动画（transitions）|
|android:windowActivityTransitions      |boolean|是否开启过渡动画|
|android:windowIsTranslucent            |boolean|设置窗口是否透明|
|android:windowDisablePreview           |boolean|禁用默认启动窗口|
|android:windowNoDisplay                |boolean|当前启动的窗口不可见|
|windowEnterTransition                  |@anim|引用 XML中的动画资源，定义所需的Transition，用于将Views移动到初始Window的内容Scene中。 |
|android:windowExitTransition   |@anim|引用XML中的动画资源，定义所需的Transition，用于在启动新Activity时将Views移出Window的内容Scene。 |

### 软键盘

|属性|描述|
|:--:|:--:|
|android:windowSoftInputMode|设置软键盘显示模式|

#### 软键盘模式有以下几种：

##### stateUnspecified  
未指定状态,软件默认采用的就是这种交互方式，系统会根据界面采取相应的软键盘的显示模式。

##### stateUnchanged
状态不改变,当前界面的软键盘状态，取决于上一个界面的软键盘状态。

##### stateHidden
设置软键盘隐藏。

##### stateAlwaysHidden
该属性也可以让软键盘隐藏。

##### stateVisible
设置为这个属性，可以将软键盘召唤出来，即使在界面上没有输入框的情况下也可以强制召唤出来。

##### stateAlwaysVisible
这个属性也是可以将键盘召唤出来，但是与stateVisible属性有小小的不同之处，stateAlwaysVisible设置软键盘一直显示，离开当前界面在回到当前界面是软键盘仍然是显示的，不像stateVisible状态，离开当前洁面后就隐藏。

##### adjustUnspecified
设置软键盘与软件的显示内容之间的显示关系，系统会根据界面选择不同的模式。

##### adjustResize
这个属性表示Activity的主窗口总是会被调整大小，从而保证软键盘显示空间。

##### adjustPan
如果设置为这个属性，那么Activity的屏幕大小并不会调整来保证软键盘的空间，而是采取了另外一种策略，系统会通过布局的移动，来保证用户要进行输入的输入框肯定在用户的失业范围里面，从而让用户可以看到自己输入的内容。
