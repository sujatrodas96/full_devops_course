# SYSTEMCTL (SERVICES)

systemctl status service -- To check current status of a service (running/stopped, logs, PID, memory usage)

systemctl start service -- To manually start a service (used when service is stopped or installed newly)

systemctl stop service -- To stop a running service (used for maintenance or troubleshooting)

systemctl restart service -- To restart a service (used after configuration changes or when service crashes)

systemctl enable service -- To enable service to start automatically on system boot (important for production services)

systemctl disable service -- To stop service from auto starting on boot (used to disable unnecessary/risky services)
