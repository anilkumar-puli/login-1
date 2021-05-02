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
