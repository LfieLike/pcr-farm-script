# pcr-farm-script
*公主链接农场脚本*<br>
  需要安装adb调试<br>
  需要使用模拟器多开，部分模拟器可能多开检测不到，推荐使用雷电模拟器<br>
  因为部分操作使用了绝对坐标，所以模拟器分辨率要设为720p<br>
  accountlist写入账号密码，格式（账号+' '+密码+'\n'）<br>
  运行前将所有模拟器手动点到touch to continue界面，运行main.py，会自动刷地下城并且切换下一个农场号，全部刷完后自动退出<br>
  例子为25个号5开，要更改需更改main函数<br>
  部分功能如捐装备，推图点赞目前未开发，以后再更新<br>

2020-6-16更新：<br>
  #更新了40对1功能<br>
    在代码开始处填入工会1，工会2，大号的账号与密码<br>
    accountList2填入工会2的所有账号密码，格式同accountlist1<br>
    myassist.png为选择派遣的支援单位的图标，要在选择界面里截图，并且选第一页就有的，不能往下翻，就算只有一半的图也行。因为我没有做选支援的时候向下翻页的功能<br>
    注意如果模拟器没有另外安装中文输入法的话，行会名字要起英文，不然会乱码<br>

2020-6-18更新<br>
  #更新了每天碎三管体力刷31次3-1的功能<br>
      并且优化了一下逻辑，大概提速一倍，目前刷一轮4分50秒左右<br>

2020-6-28更新<br>
  #更新了跳过升级界面的功能，增加了刷图时的跳过功能，并根据网友提醒把刷图时点击加号改为了长按六秒，工会操作中多加了一些sleep<br>
  预设改为了4开的7*4+3*4模式<br>
  images文件夹添加了run_cn.png
  
<br><br>关于自己截图的问题<br>
截图的时候要把模拟器放全屏，如果显示器不是1080p的话自己截的图得改resize函数里面的1920，例如1600*900的1920就改成1600，而且要把其他所有图都截一遍。或者加一个if把你自己截的图作为特例，写一个新的resize把1920换成1600来单独处理你自己截的图，其他图片的还是用原来的resize<br>
