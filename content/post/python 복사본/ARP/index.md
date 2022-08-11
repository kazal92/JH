---
title: "ARP"
date: 2022-04-04T07:59:37+09:00
categories: 
    - Python
tags: [ ARP, Netwrok ]
---

1. 누구냐고 물을 IP를 요청하는 브로드캐스트 MAC에 대한 ARP 요청 생성
- ARP를 사용하여 누가 대상 IP를 가지고 있는지 확인
- 목적지 MAC을 브로드캐스트 MAC으로 설정
2. ㄱㅋ

 broadcast = scapy.Ether(dst="ff:ff:ff:ff:ff:ff") 
    broadcast.show()  # 확인