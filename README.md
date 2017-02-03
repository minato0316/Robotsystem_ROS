# RobotSystem_ROS
###最初に端末でroscoreを起動しておく
##count.py
###動作
####パブリッシャ、変数を+1してデータを出す。これを繰り返す。
####ノードを立ち上げてトピックとしてデータを受け取る。
###実行方法
####1. rosrun RobotSystem_Package count.py 実行
####2. rostopic echo /count_up でトピックとして値を表示
##twice.py
###動作
####サブスクライバ、パブリッシャからデータを受け取り２倍して表示する。
###実行方法
####1. rosrun RobotSystem_Package count.py 実行
####2. rosrun RobotSystem_Package twice.py 実行でcount.pyの２倍された値を表示
##twice2.py
###動作
####パブリッシャとサブスクライバの同居、count.pyのデータを受け取り２倍する。
####ノードを立ち上げてトピックとしてデータを受け取る。
###実行方法
####1. rosrun RobotSystem_Package count.py 実行
####2. rosrun RobotSystem_Package twice2.py 実行
####3.rostopic echo /twice でcount.pyの2倍された値をトピックとして表示
####
##primenum_pub.py
###動作
###実行方法
##primenum_sub.py
###動作
###実行方法

