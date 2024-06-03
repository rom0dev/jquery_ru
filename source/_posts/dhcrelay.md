---
categories: 
title: "dhcrelay  Discarding packet received on interface that has no IPv4 address assigned"
date: 2024-04-26 00:00:00
---

Столкнулся с такой проблемой при настройке wifi точки доступа на Ubuntu Server 24.04: клиент, подключенный по WiFi не получал адреса от DHCP сервера.

Проблема решается в два этапа:

# 1

Оказывается так устроен мир, что dhcp пакеты через wifi не доходят до dhcp сервера. ([см. эту ссылку](https://superuser.com/questions/1626052/isc-dhcp-server-response-not-being-sent-over-a-wireless-bridge)) Чтобы доходили надо установить dhcp relay. Настройки не сложные. 

# 2 

Но при подключении получаем ошибку в syslog: "Discarding packet received on interface that has no IPv4 address assigned". Гугл выдаёт что-то не внятное.

Проблема решается просто: надо дать адрес WiFi карте. Для этого достатоно прописать в netplan (для Ubuntu) и применить.

Тут у меня появился вопрос: а как у других сделано так, что wifi карта имеет адрес такой же как и шлюза (моста)? Попробовал сделать адрес шлюза у WiFi карты и netplan принял эти настроки без ошибок!

