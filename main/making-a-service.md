# Making a Service

- Create a file in `/etc/systemd/system/<SERVICENAME>.service`

## File Contents

```
[Unit]
Description=SERVICE NAME
After=network.target
StartLimitIntervalSec=0
[Service]
Type=simple
Restart=always
RestartSec=1
User=cole
ExecStart=SERVICE START COMMAND (IE: `bash /home/cole/`)

[Install]
WantedBy=multi-user.target
```
