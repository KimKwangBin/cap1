# 메이플 스토리 길드원 관리

메이플 스토리 게임에서 길드 관리를 편하게 도와주는 웹사이트

           

## 1주차 - 어떤것을 만들까?
게임내 길드원의 정보를 처음 접속했을 때 저장 후 사용자가 원하면 처음 저장했던 데이터와 비교해 신규로 가입한 길드원이나 탈퇴한 인원이 있는지 변경점을 확인 합니다.                   
                              
## 2주차 - 개발 환경 세팅
VMWare 와 Ubuntu, Docker, nginx 를 설치 후 실행을 하며 어떤 오류가 있었고 어떻게 해결했는지      

설치하는 방법

VMWare (https://catnip-archive.tistory.com/entry/VMware-VMware-%EB%AC%B4%EB%A3%8C%EB%B2%84%EC%A0%84-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0Player-Window)             
Ubuntu (https://catnip-archive.tistory.com/entry/VMware-VMware%EC%97%90-%EA%B0%80%EC%83%81%EB%A8%B8%EC%8B%A0-%EC%B6%94%EA%B0%80%ED%95%98%EA%B8%B0feat-Ubuntu-1804-LTS)                      
Docker (https://blog.dalso.org/linux/ubuntu-20-04-lts/13118)                                        
nginx (https://whatisthenext.tistory.com/123)                                      

os를 설치하기 위해 Play virtual machine 눌렀을 때 나는 오류
![image](https://user-images.githubusercontent.com/101271598/159760086-2dfebcb5-8459-4f54-896f-cb8bb7a5456d.png)
                               
![image](https://user-images.githubusercontent.com/101271598/159753537-ba73220c-8034-48b2-a843-b8123538309d.png)
                                          
바이오스 세팅에서 가상화가 켜져있지 않을때 나오는 오류                        
                                              
바이오스에 들어가서 svm mode라는 설정이 disable 로 나와있는 것을 enable 로 변경해서 해결                   
https://jhnyang.tistory.com/236


명령을 실행 했을 때 Permission denied 라고 나오면서 다음 단계로 진행되지 않을 때             
                                       
관리자 권한이 없어서 오류가 나는 경우                             
리눅스에서 특정 명령어를 사용할 때 루트 권한이 필요한데 이를 일반 사용자가 사용하기 위해서 명령을 사용할때 명령 앞쪽에 sudo 를 붙여서 해결



## 3주차 - 세팅한 환경에 대한 공부
### Linux와 Windows의 차이점
-무료로 사용가능한 공개 OS             
-자유로운 오픈소스 운영체제                               
-Windows보다 보안성이 높음 (관리자 권한으로 로그인 하지 않으면 보호모드에서 작동, 오픈소스 라서 보안에 문제가 생길시 빠른 대처가 가능)                 
-무료 오픈소스 프로그램이 다양함 (직접 소스를 수정 및 제작하여 배포 가능)                     
                         

### Linux를 사용하기 위한 준비 
VMWare  - 가상 머신 소프트 웨어                     
Ubuntu - 운영체제                          
Docker - Linux 컨테이너를 만들고 사용할 수 있도록 하는 컨테이너화 기술                             
nginx - 동시접속 처리에 특화된 웹 서버 프로그램          
                             

                           
## 4주차 - 간단한 페이지 구상
-로그인       
-게시판                         
-길드 검색              
-길드 멤버 저장        
-길드 멤버 변경점 비교 확인 (캐릭터의 닉네임)        
-변경점 확인 후 새로 저장         
                         
## 5주차 - 서버 구축 및 로그인 확인

## 6주차 - 기본 웹페이지 만들기
                    
## 7주차 - 길드원 정보 가져오기, 로그인한 계정에 저장
                          
## 8주차 - 앞서 저장한 길드원 정보와 현재 길드원 비교
                     
## 9주차 - 수정
