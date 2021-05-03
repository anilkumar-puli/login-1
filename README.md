#git clone https://github.com/zelar-soft-todoapp/login.git 

install go lang......
#apt install golang-go

#mkdir go
#cd go
#mkdir src
#export GOPATH=/go
#go get
#go build

#vi /etc/systemd/system/login1.service

[Unit]
Description=login1 Service
[Service]
User=root
Environment=USERS_API_ADDRESS=172.31.57.134:8080
Environment=AUTH_API_PORT=8080
ExecStart=/root/go/src/login/login/login
Restart=always
SyslogIdentifier=login1
[Install]
WantedBy=multi-user.target


#sudo systemctl daemon-reload
#sudo systemctl restart login1
#sudo systemctl status login1


![image](https://user-images.githubusercontent.com/82602260/116801066-12f2b380-ab24-11eb-9758-411f75e1d181.png)



![Screenshot (262)](https://user-images.githubusercontent.com/82602260/116848182-aeaa1f80-ac09-11eb-8cd1-d7bcd2ae0fc3.png)



![Screenshot (259)](https://user-images.githubusercontent.com/82602260/116847421-1b241f00-ac08-11eb-9a3d-776e5048a2c1.png)
