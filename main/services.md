# Making a Service

- Create a file in `/etc/systemd/system/<SERVICENAME>.service`

## File Contents

```bash
[Unit]
Description=SERVICE NAME
After=network.target
StartLimitIntervalSec=0
[Service]
Type=simple
Restart=always
RestartSec=1
User=cole
ExecStart=SERVICE START COMMAND (IE: `bash /home/cole/Documents/scripts/gmod-start.sh`)

[Install]
WantedBy=multi-user.target
```

## Commands

- `systemctl daemon-reload` reloads the sys config
- `systemctl start gmod` starts a service named gmod
- `systemctl enable gmod` adds a service named gmod to the autostart
