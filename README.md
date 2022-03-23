# 메이플 스토리 길드원 인원의 변경점 확인할수있는 페이지

메이플 스토리 게임에서 길드 관리를 편하게 도와주는 웹사이트

                    
## 구축 환경           
VMWare                   
Ubuntu                    
Docker              
nginx                


## 사용 언어
JavaScript    
html       
css       

                          
## 주요 기능
게임내 길드원의 정보를 처음 접속했을 때 저장 후 사용자가 원하면 처음 저장했던 데이터와 비교해 신규로 가입한 길드원이나 탈퇴한 인원이 있는지 변경점을 확인 합니다.

                          
## -
-로그인       
-길드 검색              
-길드 멤버 저장        
-이후 인원의 변경점 비교 확인 (캐릭터의 닉네임)        
-변경점 확인 후 새로 저장         


## 1


## 2week
VMWare 와 Ubuntu, Docker, nginx 를 설치 후 실행을 하며 어떤 오류가 있었고 어떻게 해결했는지      

VMWare, Ubuntu 설치

VMWare (https://catnip-archive.tistory.com/entry/VMware-VMware-%EB%AC%B4%EB%A3%8C%EB%B2%84%EC%A0%84-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0Player-Window)
Ubuntu (https://catnip-archive.tistory.com/entry/VMware-VMware%EC%97%90-%EA%B0%80%EC%83%81%EB%A8%B8%EC%8B%A0-%EC%B6%94%EA%B0%80%ED%95%98%EA%B8%B0feat-Ubuntu-1804-LTS)


os를 설치하기 위해 Play virtual machine 눌렀을 때 오류가 
![image](https://user-images.githubusercontent.com/101271598/159760086-2dfebcb5-8459-4f54-896f-cb8bb7a5456d.png)

![image](https://user-images.githubusercontent.com/101271598/159753537-ba73220c-8034-48b2-a843-b8123538309d.png)

바이오스 세팅에서 가상화가 켜져있지 않을때 나오는 오류                        

바이오스에 들어가서 svm mode라는 설정이 disable 로 나와있는 것을 enable 로 변경해서 해결                   
https://jhnyang.tistory.com/236


관리자 권한이 없어서 오류가 나는 경우 (명령을 실행 했을 때 Permission denied 라고 나올 경우)             
리눅스에서 특정 명령어를 사용할 때 루트 권한이 필요한데 이를 일반 사용자가 사용하기 위해서 명령을 사용할때 명령 앞쪽에 sudo 를 붙여서 사용한다



## 3
## 4
## 5
## 6
## 7
## 8
## 9

