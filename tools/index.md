---
title: Tools
layout: page
comments: no

---

## 여기서 고전적이고 사용하기 쉬운 셸 팁을 수집하고 검토 및 공유하도록 기록합니다.

## Enjoy Shell！~

	rm -rf !(\*.html)   
\*.html을 제외한 모든 파일 삭제

	ping -c3 www.zasfe.com && links www.zasfe.com	
성공적인 실행

	apt-get update || links zasfe.com		
실행 실패

	python -m SimpleHTTPServer
파이썬을 사용하여 포트 8000의 브라우저를 통해 액세스 할 수있는 현재 디렉토리 구조를 표시하는 간단한 http 서버를 생성

	mtr google.com
ping 및 traceroute 명령 병합

	ls -l > /dev/pts/4
명령 결과를 pts / 4 터미널에 출력하십시오.

	_command
공간 기호로 실행 된 명령은 history(기록)에 기록되지 않습니다.

	stat stricks.md
파일 또는 파일 시스템에 대한 상태 정보를 봅니다

	mount | column -t
마운트 된 모든 파일 시스템을 출력합니다.

	ctrl+l
터미널을 정리하십시오.clear

	${variable:0:5}
첫 5 글자 가로 채기

	mkdir -p /home/user/{test,test1,test2}
여러 디렉토리 만들기

	dd if=/dev/zero of=/tmp/output.img bs=8k count=256k; rm -rf /tmp/output.img
하드 디스크 쓰기 속도 테스트.

	hdparm -Tt /dev/sda
하드 디스크 읽기 속도 테스트

	xmllint --noout file.xml
xml 형식 확인

	cp some_file_name{,.bkp}
빠른 백업 파일

	watch -d -n 1 ps aux
ps aux의 출력을 모니터링하고 초당 1 회 출력하고 변경된 영역을 다른 색상으로 표시합니다.

	mount -o remount,rw /
마운트 매개 변수를 수정하여 다시 마운트 합니다.

	mount -t tmpfs tmpfs /tmpram -o size=512m
임시 RAM 파일 시스템 만들기

	nmap -p 8081 172.20.0.0/16
네트워크에서 열린 포트 검사

	ls | shuf -n1
무작위로 파일 이름 출력 선택

	ssh user@server bash < /path/to/local/script.sh
스크립트를 원격 서버에 업로드하지 않도록 스크립트를 실행하려면 원격 서버에 대한 Ssh

	ssh user@host cat /path/to/remotefile | diff /path/to/localfile -
원격 파일과 로컬 파일의 차이점 비교

	vim scp://username@host//path/to/somefile
원격 파일로 보냄

	curl ifconfig.me
인트라넷에서 공용 네트워크 IP보기

	echo ${#a}
가변 문자 수를 가져라.

	tmp_file_name=$(mktemp TMP.XXXXXX)
임의의 파일 이름으로 임시 파일을 생성하십시오.

ctrl + n을 사용하여 변수 이름을 완성하십시오.

---

