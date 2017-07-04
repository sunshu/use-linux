### Ubuntu 下禁用设备  
`
并不是永久禁止，下次启动会恢复
`

> 笔记本打字时候，经常误触到触摸板，
> window 下可以在控制面板或者，管理里面找到硬件设备，禁用
> Ubuntu下可以通过禁用触摸板硬件来禁止实现
 
 通过 ` xinput list // 查看硬件信息`
 
<pre>
 sunshu@nus-HP:~$ xinput list
⎡ Virtual core pointer                    	id=2	[master pointer  (3)]
⎜   ↳ Virtual core XTEST pointer              	id=4	[slave  pointer  (2)]
⎜   ↳ Logitech G90 Optical Gaming Mouse       	id=10	[slave  pointer  (2)]
⎜   ↳ SynPS/2 Synaptics TouchPad              	id=13	[slave  pointer  (2)]
⎣ Virtual core keyboard                   	id=3	[master keyboard (2)]
    ↳ Virtual core XTEST keyboard             	id=5	[slave  keyboard (3)]
    ↳ Power Button                            	id=6	[slave  keyboard (3)]
    ↳ Video Bus                               	id=7	[slave  keyboard (3)]
    ↳ Video Bus                               	id=8	[slave  keyboard (3)]
    ↳ Power Button                            	id=9	[slave  keyboard (3)]
    ↳ HP Truevision HD                        	id=11	[slave  keyboard (3)]
    ↳ AT Translated Set 2 keyboard            	id=12	[slave  keyboard (3)]
    ↳ HP WMI hotkeys                          	id=14	[slave  keyboard (3)]
    ↳ HP Wireless hotkeys                     	id=15	[slave  keyboard (3)]
sunshu@nus-HP:~$ xinput set-prop  13 "Device Enabled" 0
 </pre>
 
  xinput set-prop  13 "Device Enabled" 0
  
  0 表示禁用 1 表示启用
 
 依次可以看到 
 
 * Virtual core XTEST pointer 
 * 罗技鼠标
 * 触摸板
 * Virtual core XTEST keyboard 
 * 电源按钮
 * 两个视频总线
 * 摄像头 HP Truevision HD 
 * Translated Set 2 keyboard   键盘
 * WMI hotkeys  ??
 * Wireless hotkeys    无线网
  
  


