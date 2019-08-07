## Apache2 설치(Ubuntu 18.04)

ubuntu 기본 소프트웨어 저장소에 사용할 수 있는 apache가 있다.

1. root 로그인

2. 패키지 관리 툴인 apt-get을 이용하여 apache2를 설치한다. (apache2 설치와 함께 의존하는 프로그램도 함께 설치된다.)

 > apt-get update

 > apt-get install apache2

3. 설치 후 Apache 상태 확인

 > systemctl status apache2

4. Apache 접속

 > hostname -I  명령어를 통해 IP를 알아낸 후 웹 브라우저를 이용하여 http://{IP} 로 접속해보자.
 
 ## Apache2 설정
 
 /etc/apache2/

아파치 설정 디렉토리



/etc/apache2/apache2.conf

아파치 기본 설정 파일



/etc/apache2/ports.conf

아파치 포트 설정 파일



/etc/apache2/sites-available/

virtual host 관리 디렉토리 (아파치에서는 해당 디렉토리를 직접 참조하지는 않는다.)



/etc/apache2/sites-enabled/

virtual host를 이용하기 위한 설정 디렉토리

000-default.conf -> ../sites-available/000-default.conf 와 같이 심볼릭 링크를 이용하여 sites-available 디렉토리 파일을 참조하는 방식으로 사용되어진다.

ln -s ../sites-available/000-default.conf 000-default.conf 



/etc/apache2/mods-available/, /etc/apache2/mods-enabled/

모듈 설정 디렉토리
