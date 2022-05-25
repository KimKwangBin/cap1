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
    
    
## 4주차 - Redis 및 Mysql 설치 확인 
redis (https://ozofweird.tistory.com/entry/Spring-Boot-Redis-Cache-MySQL-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EA%B0%84%EB%8B%A8%ED%95%9C-API-%EC%A0%9C%EC%9E%91)            
mysql (https://velog.io/@seungsang00/Ubuntu-%EC%9A%B0%EB%B6%84%ED%88%AC%EC%97%90-MySQL-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0)                     
               
               
## 5주차 - 간단한 페이지 구상
처음 화면                   
![image](https://user-images.githubusercontent.com/101271598/163008128-9c1cd91d-4aa1-43fa-927c-d88c79a31382.png)                   
길드 검색 화면                         
![image](https://user-images.githubusercontent.com/101271598/163008173-1e0f8f06-72d6-43fc-b38a-f2cb83053f92.png)                     
저장한 데이터 불러오기                         
![image](https://user-images.githubusercontent.com/101271598/163008332-9fe64fcb-b43a-4ec5-ba74-f38449e68d72.png)                              
데이터 비교                                
![image](https://user-images.githubusercontent.com/101271598/163008396-ccd97acf-5c15-44bb-a184-a1d0fadcf93c.png)                         
게시판                       
![image](https://user-images.githubusercontent.com/101271598/163008448-7edd678b-1837-4a8e-8697-deff98032d25.png)                           


## 6주차 - 기본 웹페이지 만들기
메인 페이지                                             
![image](https://user-images.githubusercontent.com/101271598/170381734-32230c09-16d1-4370-99c8-fa3102218146.png)
                                                       


## 7~8주차 - 회원가입, 로그인 만들기                               
로그인 페이지                                
로그인 페이지는 들어가자 마자 ID 입력란에 바로 커서가 올라가게 설정
![image](https://user-images.githubusercontent.com/101271598/170381778-fc186129-24c4-453b-86c8-d739bc91a891.png)
아이디를 입력하지 않을경우 경고문이 나오면서 버튼클릭을 막음
![image](https://user-images.githubusercontent.com/101271598/170381837-f3e3b617-45b9-4b6c-a60c-f44009e45351.png)
비밀번호도 아이디와 같게 설정
![image](https://user-images.githubusercontent.com/101271598/170381880-815dcebb-1777-47f0-b6e7-b9a49aa1bd5f.png)
                  
                  
회원가입 페이지                                            
![image](https://user-images.githubusercontent.com/101271598/170385389-ae60f0c0-8418-4c24-9426-05bde152bbd5.png)                           
                                                     
                                                     
                                                     
데이터베이스에 로그인하여 정보를 저장할때 사용할 코드                                                               
![Inked170382527-2235a613-d74e-47dc-a22a-5dc57e961ece_LI](https://user-images.githubusercontent.com/101271598/170383949-6d6d2cc0-b835-427a-9683-92ab05924052.jpg)
                             

DAO와 DTO를 이용해 회원가입페이지에서 입력한 정보를 데이터베이스에 저장하는 코드                            
![image](https://user-images.githubusercontent.com/101271598/170384573-ec4def5d-531e-469f-be6d-9b1b6e879438.png)                               



## 9~10주차 - 데이터베이스 구축
데이터베이스 테이블을 만듬                                            
![image](https://user-images.githubusercontent.com/101271598/170383293-a2bca7db-5214-401e-90ea-46a3ed4fff81.png)

먼저 데이터를 입력후 저장되는지 확인                                       
![image](https://user-images.githubusercontent.com/101271598/170383314-fe3a5b11-e55c-4c8c-ae13-260f321e6bd2.png)



                    
## 11~ 주차 - 데이터 가져오기, 로그인한 계정에 데이터 저장하기
사이트에서 검색을 하면 서버 마다 같은이름의 길드가 존재할 가능성이 있음
정보갱신을 직접 해줘야함

캐릭터 정보외 다른것도 있음
![image](https://user-images.githubusercontent.com/101271598/170385633-410a2472-7718-439d-9768-e17c86978f37.png)

         
## 주차 - 앞서 저장한 데이터와 새로운 데이터 비교
어떤 방법으로 비교할것인가
         
         
## 주차 - 게시판 추가

