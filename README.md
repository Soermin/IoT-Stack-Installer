# IOT Stack Installer (Ubuntu)

This project started from a pretty common problem, especially if you often work with Ubuntu servers:  
**setting up IoT monitoring is repetitive, time-consuming, and easy to mess up.**

Every time a new project starts on Ubuntu, the steps usually look the same:
- install MQTT
- install a time-series database
- install a dashboard
- and eventually troubleshoot things that could have been avoided

This script was created to clean up that process.

## Approach

This project is **intentionally focused on Ubuntu**.  
Not because other distributions are impossible to support, but because this makes the system:
- more stable
- more consistent
- easier to maintain and explain

The script helps prepare a solid **IoT monitoring stack foundation** on Ubuntu, without trying to be a one-size-fits-all solution.

The components included are:
- **Mosquitto** as the MQTT broker  
- **InfluxDB 2.x** for sensor data storage  
- **Grafana** for visualization  
- **Telegraf** as the data bridge

The data flow looks like this:

![Technology-Stack](https://github.com/user-attachments/assets/0aa19c6d-d605-4c14-8cec-638110711ad4)

## Quick Usage

```bash
chmod +x iot_monitoring.sh
sudo ./iot_monitoring.sh
```

This project was built to save time on repetitive setup work. If it helps you focus more on the actual data instead of installation, it has done its job.
