# RobotSystem_ROS
##robosys_mypkg
###最初に端末でroscoreを起動しておく
##count.py
###動作
####パブリッシャ、変数を定義し、＋１しながら表示させていく。
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
####3.rostopic echo /twice2 でcount.pyの2倍された値をトピックとして表示
####
##primenum_pub.py
###動作
####パブリッシャ、1000までの素数の値及びその数量(何番目か)をデータとして出す。
###実行方法
####1. rosrun RobotSystem_Package primenum_pub.py を実行
####2. rostopic echo /primenum_quanti でトピックとして素数の数量を表示
####2. rostopic echo /primenum_up でトピックとして素数の値を表示
##primenum_sub.py
###動作
####サブスクライバ、パブリッシャからデータを受け取り、1000までの素数の値と数量の両方を表示
###実行方法
####1. rosrun RobotSystem_Package primenum_pub.py を実行
####2. rosrun RobotSystem_Package primenum_sub.py を実行で素数の値と数量の両方を表示
