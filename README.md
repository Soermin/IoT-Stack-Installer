# IOT Stack Installer (Ubuntu)

Project ini muncul dari masalah yang cukup klasik, terutama kalau sering main di server Ubuntu:  
**setup IoT monitoring itu berulang, makan waktu, dan gampang keliru.**

Setiap mulai proyek baru di Ubuntu, langkahnya hampir selalu sama:
- install MQTT
- install database time-series
- install dashboard
- dan akhirnya troubleshooting hal yang seharusnya bisa dihindari

Script ini dibuat untuk merapikan proses itu.

## Pendekatan yang Dipakai

Project ini **sengaja fokus ke Ubuntu**.  
Bukan karena tidak bisa ke distro lain, tapi supaya:
- lebih stabil
- lebih konsisten
- lebih mudah dirawat dan dijelaskan

Script ini membantu menyiapkan **fondasi IoT monitoring stack** di Ubuntu, tanpa mencoba jadi solusi untuk semua sistem.

Komponen yang disiapkan:
- **Mosquitto** sebagai MQTT broker  
- **InfluxDB 2.x** untuk penyimpanan data sensor  
- **Grafana** untuk visualisasi  
- **Telegraf** sebagai penghubung data

Alur datanya:
![Technology-Stack](https://github.com/user-attachments/assets/0aa19c6d-d605-4c14-8cec-638110711ad4)

## Cara Pakai Singkat

```bash
chmod +x iot_monitoring.sh
sudo ./iot_monitoring.sh
```


Bukan script paling canggih, tapi cukup untuk memulai dengan rapi. Dari sini, kamu bebas mengembangkannya ke arah mana pun.
