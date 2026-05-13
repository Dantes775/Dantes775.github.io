---
{"dg-publish":true,"permalink":"/vpn-manuals/vpn/mesh-network/tailscale-vpn/","dg-note-properties":{"title":""}}
---

https://vc.ru/dev/497249-razvorachivaem-tailscale-vpn-u-sebya-v-oblake

https://tailscale.com/

https://ddpa.ru/p/tailscale

https://purpleschool.ru/knowledge-base/docker/work-with-network/tailscale-in-docker

https://wiki.wirenboard.com/wiki/Tailscale

"Tailscale это по сути тунель между пк. А радмин это общая сеть. Через радмин при подключении все пк как будто находятся в 1 wi-fi сети и видят друг-друга. Но tailscale это тунель где надо вводить ip адрес вручную и если игра не поддерживает подключения к серверам через ip:порт то tailscale не сработает. Я его делал только для майнкрафта на больших сборках, когда сервер не работает стабильно."



Если **Hamachi** — это старая добрая классика для локальных игр через интернет, то **Tailscale** — это «Hamachi на стероидах».

**Tailscale** — это ==современный, простой в настройке VPN-сервис на базе протокола [WireGuard](https://wiki.wirenboard.com/wiki/Tailscale), создающий защищенную, прямую (mesh) сеть между вашими устройствами [0.5.4](https://ddpa.ru/p/tailscale), [0.5.6](https://bigmike.help/ru/posts/089/)==. Он позволяет безопасно объединять компьютеры, серверы, телефоны и облачную инфраструктуру, находящиеся за NAT или firewall, без необходимости ручной настройки портов [0.5.2](https://vc.ru/dev/497249-razvorachivaem-tailscale-vpn-u-sebya-v-oblake), [0.5.7](https://docs-python.ru/other/tailscale-i-headscale/).

**Ключевые особенности и преимущества:**

- **Zero-config:** Tailscale не требует настройки серверов или обмена ключами. Установите клиент, войдите в аккаунт — и устройства в сети 0.5.2, 0.5.6.
- **Mesh-сеть:** Все устройства могут взаимодействовать напрямую (peer-to-peer), что обеспечивает высокую скорость и безопасность, не пропуская трафик через центральный узел 0.5.4, [0.5.10](https://bafista.ru/ustanovka-tailscale-vpn-na-vps-linux/).
- **Пробивка NAT:** Работает сквозь строгие брандмауэры и корпоративные сети, не требуя белого IP-адреса 0.5.2, 0.5.7.
- **Безопасность:** Использует сквозное шифрование 0.5.4, [0.5.13](https://tailscale.com/security).
- **Функции:** Позволяет использовать Exit Nodes (выходные узлы) для маршрутизации всего интернет-трафика, MagicDNS для автоматического назначения имен устройствам [0.5.5](https://www.reddit.com/r/explainlikeimfive/comments/1g2edvu/eli5_what_exactly_is_tailscale_what_is_it_used_for/?tl=ru).

Tailscale идеально подходит для удаленного доступа к домашней лаборатории (homelab), объединения серверов, безопасного подключения к рабочим ресурсам и использования exit nodes для безопасного серфинга 0.5.4, 0.5.5.
