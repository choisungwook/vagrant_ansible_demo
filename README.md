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
![실행결과](./imgs/result.png)
<br> 실행결과: ansible-server, ansible-client1 VM 생성

# 4. 설정 수정
## 4.1 클라이언트 수 추가
* vagranfile파일: N변수 수정
* install_ansible/add_hosts.yaml파일: client그룹에 IP추가
## 4.2 IP 수정
* ansible서버 IP: vagrantfile의 IP_MASTER변수 수정
* ansible클라이언트 IP: vagrantfile의 IP_CLIENT변수 수정

# 5. 참고자료
* [1] 블로그-ansible구축: https://daddyprogrammer.org/post/7369/ansible-vagrant/
* [2] 공식문서-playbooks Intro: https://docs.ansible.com/ansible/latest/user_guide/playbooks_intro.html
* [3] 공식문서-playbooks example: https://github.com/ansible/ansible-examples
* [4] 블로그: gather_facts: https://ossian.tistory.com/98
* [5] 번역: https://github.com/mcchae/ansible_doc_ko/blob/master/Asible%20%EC%86%8C%EA%B0%9C.md