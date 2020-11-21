# 1. 프로젝트 개요
vagrant로 ansible server, client 구축

# 2. 준비
* virtualbox 설치
* vagrant 설치
  
# 3. 사용방법
* 네트워크는 NAT, INTERNET 총 2개로 구성
```sh
vagrant up
```

# 4. 설정 수정
## 4.1 클라이언트 수 추가
* vagranfile파일: N변수 수정
* install_ansible/add_hosts.yaml파일: client그룹에 IP추가
## 4.2 IP 수정
* ansible서버 IP: vagrantfile의 IP_MASTER변수 수정
* ansible클라이언트 IP: vagrantfile의 IP_CLIENT변수 수정