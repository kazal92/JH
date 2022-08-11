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
2. testetestestsettet haha

 broadcast = scapy.Ether(dst="ff:ff:ff:ff:ff:ff") 
    broadcast.show()  # 확인

    [https://www.guru99.com/linux-commands-cheat-sheet.html#2](https://www.guru99.com/linux-commands-cheat-sheet.html#2)

 [Linux Command Cheat Sheet

In this Linux/Unix command line cheat sheet, you will learn: Basic Linux commands File Permission commands Environment Variables command User management commands of linux Networking command Process co

www.guru99.com](https://www.guru99.com/linux-commands-cheat-sheet.html#2)

이 Linux/Unix 명령줄 치트 시트에서는 다음을 배우게 됩니다.

-   [기본 Linux 명령](https://www.guru99.com/linux-commands-cheat-sheet.html#1)
-   [파일 권한 명령](https://www.guru99.com/linux-commands-cheat-sheet.html#2)
-   [환경 변수 명령](https://www.guru99.com/linux-commands-cheat-sheet.html#3)
-   [리눅스의 사용자 관리 명령어](https://www.guru99.com/linux-commands-cheat-sheet.html#4)
-   [네트워킹 명령](https://www.guru99.com/linux-commands-cheat-sheet.html#5)
-   [처리 명령](https://www.guru99.com/linux-commands-cheat-sheet.html#6)
-   [VI 편집 명령](https://www.guru99.com/linux-commands-cheat-sheet.html#7)

## 기본 Linux 명령

명령설명

| ls | 현재 작업 디렉토리의 모든 파일과 디렉토리를 나열합니다. |
| --- | --- |
| ls -R | 하위 디렉토리의 파일도 나열합니다. |
| ls -a | 숨김 파일도 나열 |
| ls -al | 권한, 크기, 소유자 등과 같은 자세한 정보가 있는 파일 및 디렉토리를 나열합니다. |
| cd or cd ~ | 홈 디렉토리로 이동 |
| cd .. | 한 단계 위로 이동 |
| cd | 특정 디렉토리로 변경하려면 |
| cd / | 루트 디렉토리로 이동 |
| cat > filename | 새 파일을 만듭니다. |
| cat filename | 파일 내용을 표시합니다 |
| cat file1 file2 > file3 | 두 개의 파일(file1, file2)을 결합하고 새 파일(file3)에 출력을 저장합니다. |
| mv file "new file path" | 파일을 새 위치로 이동합니다. |
| mv filename new\_file\_name | 파일 이름을 새 파일 이름으로 바꿉니다. |
| sudo | 일반 사용자가 수퍼유저 또는 루트의 보안 권한으로 프로그램을 실행할 수 있습니다. |
| rm filename | 파일 삭제 |
| man | 명령에 대한 도움말 정보 제공 |
| history | 현재 터미널 세션에 입력된 모든 과거 명령 목록을 제공합니다. |
| clear | 터미널을 지웁니다. |
| mkdir directoryname | 현재 작업 디렉토리 또는 지정된 경로에 새 디렉토리를 만듭니다. |
| rmdir | 디렉토리를 삭제합니다 |
| mv | 디렉토리 이름 바꾸기 |
| pr -x | 파일을 x 열로 나눕니다. |
| pr -h | 파일에 헤더를 할당 |
| pr -n | 줄 번호가 있는 파일을 나타냅니다. |
| lp -nc , lpr c | 파일의 "c" 사본을 인쇄합니다. |
|  lp-d lp-P | 프린터의 이름을 지정합니다 |
| apt-get | 패키지 설치 및 업데이트에 사용되는 명령 |
| mail -s 'subject'   \-c 'cc-address'   \-b 'bcc-address'   'to-address' | 이메일을 보내는 명령 |
| mail -s "Subject"   to-address < Filename | 첨부 파일이 있는 이메일을 보내는 명령 |

## 파일 권한 명령

명령설명

| ls -l | 파일 형식 및 액세스 권한 표시 |
| --- | --- |
| r | 읽기 권한 |
| w | 쓰기 권한 |
| x | 실행 권한 |
| \-= | 비허가 |
| Chown user | 파일/디렉토리의 소유권을 변경하려면 |
| Chown user:group filename | 파일 또는 디렉토리에 대한 사용자 및 그룹 변경 |

## 환경 변수 명령

명령설명

| echo $VARIABLE | 변수의 값을 표시하려면 |
| --- | --- |
| env | 모든 환경 변수를 표시합니다. |
| VARIABLE\_NAME= variable\_value | 새 변수 생성 |
| Unset | 변수 제거 |
| export Variable=value | 환경 변수의 값을 설정하려면 |

## 리눅스의 사용자 관리 명령어

명령설명

| sudo adduser username | 새 사용자를 추가하려면 |
| --- | --- |
| sudo passwd -l 'username' | 사용자의 비밀번호를 변경하려면 |
| sudo userdel -r 'username' | 새로 생성된 사용자를 제거하려면 |
| sudo usermod -a -G GROUPNAME USERNAME | 그룹에 사용자를 추가하려면 |
| sudo deluser USER GROUPNAME | 그룹에서 사용자를 제거하려면 |
| finger | 로그인한 모든 사용자의 정보를 표시합니다. |
| finger username | 특정 사용자의 정보 제공 |

## 네트워킹 명령

명령설명

| SSH username@ip-address or hostname | SSH를 사용하여 원격 Linux 시스템에 로그인 |
| --- | --- |
| Ping hostname="" or ="" | 네트워크 및 호스트 연결을 ping하고 분석하려면 |
| dir | 원격 컴퓨터의 현재 디렉토리에 있는 파일 표시 |
| cd "dirname" | 원격 컴퓨터에서 디렉토리를 "dirname"으로 변경 |
| put file | 로컬에서 원격 컴퓨터로 '파일' 업로드 |
| get file | 원격 컴퓨터에서 로컬 컴퓨터로 '파일' 다운로드 |
| quit | 로그 아웃 |

## 처리 명령

명령설명

| bg | 프로세스를 백그라운드로 보내려면 |
| --- | --- |
| fg | 중지된 프로세스를 포그라운드에서 실행하려면 |
| top | 모든 활성 프로세스에 대한 세부 정보 |
| ps | 사용자에 대해 실행 중인 프로세스의 상태 제공 |
| ps PID | 특정 프로세스의 상태를 제공합니다. |
| pidof | 프로세스의 프로세스 ID(PID)를 제공합니다. |
| kill PID | 프로세스 종료 |
| nice | 주어진 우선 순위로 프로세스를 시작합니다. |
| renice | 이미 실행 중인 프로세스의 우선 순위 변경 |
| df | 시스템에 여유 하드 디스크 공간을 제공합니다. |
| free | 시스템에 여유 RAM 제공 |

## VI 편집 명령

명령설명

| i | 커서 위치에 삽입(삽입 모드로 전환) |
| --- | --- |
| a | 커서 뒤에 쓰기(삽입 모드로 전환) |
| A | 줄 끝에 쓰기(삽입 모드로 전환) |
| ESC | 삽입 모드 종료 |
| u | 마지막 변경 취소 |
| U | 전체 라인에 대한 모든 변경 사항 실행 취소 |
| o | 새 줄 열기(삽입 모드로 전환) |
| dd | 라인 삭제 |
| 3dd | 3줄 삭제 |
| D | 커서 다음 줄의 내용 삭제 |
| C | 커서 뒤에 있는 줄의 내용을 삭제하고 새 텍스트를 삽입합니다. ESC 키를 눌러 삽입을 종료합니다. |
| dw | 단어 삭제 |
| 4dw | 4단어 삭제 |
| cw | 단어 변경 |
| x | 커서에서 문자 삭제 |
| r | 문자 바꾸기 |
| R | 커서부터 문자 덮어쓰기 |
| s | 커서 아래에 한 문자를 대체하여 계속 삽입 |
| S | 전체 줄을 대체하고 줄의 시작 부분에 삽입 시작 |
| ~ | 개별 문자의 대소문자 변경 |