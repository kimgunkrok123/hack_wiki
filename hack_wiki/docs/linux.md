# linux commands

this commands for archlinux,
not for other linux

### about files and dirt

- **CD**
다른 디렉토리로 이동할때 사용함.
```shell
cd <path>
```
예시
```shell
cd ./kim/workspace
```

--- 

- **ls** 
현재 디렉토리안의 플더와 파일들을 출력함
```shell
ls
#아래와 같은 결과가 나온다
Desktop  Documents  Downloads  Games  Music  Pictures  Public  Templates  Unity  Videos  yay
```

---

- **mkdir**
```shell
mkdir <name>
```

---

- **rm**
디렉토리나 파일을 삭제한다
```shell
rm <path>

#아래와같이 사용할수있다
rm ./kim/workspace
rm ./kim/python_test.py
```

---

- **cp** 
파일이나 디렉토리를 복사하여 다른 디렉토리에 저장한다
```shell
#첫번째 경로에는 복사할 디렉토리나 파일을 입력하고 두번째 경로에는 복사될 디렉토리를 입력하면 된다
cp <path> <path>

cp ./kim/workspace ./kim/zsh
```

---

- **pwd**
현재 자신이 있는 디렉토리의 경로를 출력한다
```shell
pwd
/home/kim
```
---
### about system 

- **cat**
파일의 내용을 출력한다
```shell
cat <path>
```
---
- **sudo**
관리자권한(root)으로 뒤에 오는 명령을 실행한다


```shell
sudo <command>
#아래와같이 쓸수있대
sudo cd /home/usr/share/icons
```
해석하면 원래 편집권한이 없는 플더에 접근하는 것이다

---

- **top**
현재 실행중인 상위 프로세서를 출력한다
```shell
top
```
```shell
Tasks: 379 total, 1 running, 374 sleep, 2 d-sleep, 0 stopped, 2 zombie
%Cpu(s):  0.8 us,  0.8 sy,  0.0 ni, 98.4 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st 
MiB Mem :  15916.5 total,    427.9 free,   6957.3 used,   9227.0 buff/cache     
MiB Swap:      0.0 total,      0.0 free,      0.0 used.   8959.1 avail Mem 

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND                                
 143479 kim       20   0 1394.2g 789440 168224 S  28.0   4.8  67:35.60 chrome                                 
 168339 kim       20   0   12504   9492   7248 R   9.3   0.1   0:00.01 top                                    
      1 root      20   0   23060  12380   7892 S   0.0   0.1   0:24.03 systemd                                
```
---
- **who**
컴퓨터에 접속한 유저들을 출력한다
```shell
who
```
```shell
kim      tty2         2025-10-26 07:09 (:0)
kim      pts/0        2025-10-26 07:09 (:0)
kim      pts/1        2025-10-26 20:45 (:0)
```
---
- **w**
현재 활동하는 유저와 유저에 정보를 출력한다
```shell
w
```
```shell
20:45:27 up 13:36,  1 user,  load average: 2.42, 2.61, 2.88
USER     TTY       LOGIN@   IDLE   JCPU   PCPU  
kim      tty2      07:09   11:17m  9:23   0.02s 
```
---
- **poweroff**
전원끄는거
```shell
poweroff
```
----
- **reboot**
재부팅하는거
```shell
reboot
```
---
- **pacman**
프로그램 설치하는 명령어
```shell
pacman <operation> [...]
```
| operation | discraption | use
|:--|:--|:--
| -S | install program | pacman -S \<package> 
| -Ss | found program| pacman -Ss \<package>
| -Syu | updata repo | pacman -Syu \<package>
| -Rns | remove program | pacman -Rns \<package>   

---