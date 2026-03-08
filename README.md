原作者（made by）：Geminize

解压到游戏目录下，运行DSE-Patcher.exe进游戏即可，对于不同游戏，编辑DSE-Patcher.ini，更改对应的LaunchExe=和TargetProcess=即可
以下以剑星的DSE-Patcher.ini为例

[Settings]
#在禁用dse后要运行的启动文件（相对于DSE-Patcher.exe的位置或绝对路径）
LaunchExe=steamclient_loader_x64.exe

#要监控的游戏进程名，一旦检测到该进程正在运行，dse将自动还原（注意，这个是正版游戏的exe，一般和启动文件不是同一个，比如生9就是re9.exe）
TargetProcess=SB-Win64-Shipping.exe

#检查目标游戏进程的频率，单位为毫秒
PollIntervalMs=1000

#如果无法检测到目标游戏进程，将在以下时间后自动还原dse，单位为秒，0表示不自动还原
TimeoutSeconds=60

Extract the files to the game directory, then run DSE-Patcher.exe to enter the game. For different games, edit DSE-Patcher.ini and modify the corresponding LaunchExe= and TargetProcess= accordingly.
Below is an example using the DSE-Patcher.ini for Stellar Blade:

[Settings]
#The launch file to run after disabling DSE (relative to DSE-Patcher.exe or an absolute path)
LaunchExe=steamclient_loader_x64.exe

#The game process name to monitor. Once the process is detected running, DSE will be automatically restored (Note: This is the original game's exe, which is usually not the same as the launch file. For example, for Resident Evil 9, it would be re9.exe)
TargetProcess=SB-Win64-Shipping.exe

#Frequency to check for the target game process, in milliseconds
PollIntervalMs=1000

#If the target game process cannot be detected, DSE will be automatically restored after the following time, in seconds. 0 means no automatic restoration.
TimeoutSeconds=60
