# server
copter connects GCS via IP net,a server with public IP address is needed,it transmits mavlink-packages between copter and GCS via UDP. Any settings or custom commands receive from qgroundcontrol and copter are printed by this program along with the heartbeats. As this program contains the mavlink library,you can parse messages and make some control.Setting no fly zone according to latitude and longitude etc.

无人机和地面控制站通过IP网络连接，需要一个具有公网IP地址的服务器在无人机和地面站间转发mavlink消息，地面站的控制指令和飞行器的状态都能够在服务器程序上展现出来。本程序加入了通用的mavlink库，所以能解析消息并做出控制。比如无人机的经纬度信息会实时反馈至服务器,可设置禁飞区，当无人机意外闯入时，服务器发送指令控制无人机返航。更多扩展应用期待您的参与！
