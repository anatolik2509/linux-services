# Netplan
Для сетевых настроек в ubuntu существует модуль netplan. Для настройки netplan нужно создать \*.yaml конфигурационный файл.
Пример конфига:
```
network:
  version: 2
  ethernets:
    enp0s3:
	  dhcp4: true
```

Возможные настройки
```dhcp4``` - включить dhcp
```addresses``` - назначить ip адрес интерфейсу

Для активации нужно ввести ```sudo netplan apply```