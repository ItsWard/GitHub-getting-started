# GitHub-getting-started
📝[GitHub](https://github.com/)를 시작해보자.

> 처음 개발을 시작하려보니 깃(Git), 깃허브(GitHub), 커밋(Commit).. 등등 이 중요하답니다.<br>
> 열심히 자료를 찾아봤지만 정확하게 뭐가뭔지 모르겠고 너무어렵더라구요.<br>
> **그래서 제가** 이해된 내용들을 개념 ~ 설치 ~ 사용방법까지 하나씩 추가해보도록 하겠습니다.<br>
> Reference를 기반으로 작성할 예정입니다.


## 0. 목차

>목차와 내용은 계속 수정되고, 업데이트 될 예정입니다.

1. [Git, GitHub란?](#1-git-github란)
2. [Git 설치 및 설정](#2-git-설치-및-설정)
3. [GitHub 사용 방법](#3-github-사용-방법)

  
번외 1. [GitHub 게시글 제작 방법](#번외1-github-게시글-제작-방법)<br>
번외 2. [Git, GitHub 용어 정리](#번외2-git-github-용어-정리)<br>
번외 3. [기타](#번외3-기타-사이트-모음)

## 1. Git, GitHub란?

### Git, GitHub는 무엇이길래 개발자들이 많이 사용할까요?<br>
 #### 키워드로보는 Git
 ```C
 #버전관리 #어디서나개발 #협업 #개인포트폴리오 #오픈소스
 ```

어떤 프로젝트던 **버전관리**는 중요하겠지만 소프트웨어에서는 **버전관리가 중요합니다.**
이전 버전의 기능을 가져올 수도 있고, 실수로 삭제되거나 여러 개발자가 하나의 프로그램을 제작 할 때
소스코드가 섞이는경우 **복원해야 할 수도 있죠.**

깃허브는 이러한 개발자들이 그동한 개발해 왔던 내용들을 버전관리 뿐만이 아니라 **개발 프로젝트를 위한 관리 서비스와 저장소**를 지원합니다. 
인터넷이 연결되어있다면 **어디서나 해당 프로그램을 가져와 개발 할 수 있고, 인터넷이 없더라도 미리 저장한 프로그램을 이용해 개발할 수 있습니다.** 물론, 나중에 업로드도 가능하고요!<br>

또, 깃허브를 사용해 소스를 수정하고, 개발하는 내용과 기간은 모두 기록되므로 **깃허브 자체가 자신의 포트폴리오**가 될 수 있습니다.
협업 프로그램에서는 여러 개발 소스를 병합하여 **언제 누가 무엇을 수정**하였는지 확인할 수 있고 각자 맡은 분야를 개발하여 합치는 **소스 병합**도 지원합니다.

이외에도 인스타그램, 트위터 등 SNS처럼 **다른 개발자들의 소스를 참조하거나, 오픈 소스를 이용해 함께 개발** 할 수도 있습니다. 

이러한 굉장한 장점을 가지고 있기 때문에 전세계 개발자들이 많이 사용하고 있습니다. 

### Git과 GitHub의 차이점은요?<br>
  위의 내용들은 Git의 장점들을 나열하였고 **GitHub는 Git을 보다 쉽게 사용할 수 있도록 웹에서 사용할 수 있는 도구** 입니다. 
  Git은 cmd(콘솔창)에서 직접 텍스트형식으로 입력해야하지만, 우리가 지금 보고있는 GitHub는 웹페이지에서 관리 할 수 있습니다.
  
  🎥 **["Git이 영상을 찍는 앱이라면, GitHub는 유튜브 라는 플랫폼이다 라고 생각하면 편하다."](https://www.youtube.com/watch?v=Bd35Ze7-dIw)**
  
만약 Git에 대해 더 깊게 알아보고 싶다면 [여기](https://git-scm.com/book/ko/v2)를 참조해주세요. 


## 2. Git 설치 및 설정

❗ 해당 자료는 Windows 기반을 기본으로 안내드리고있습니다. Mac OS를 사용하시는 분들께서는 [이곳](https://sin0824.tistory.com/8)을 참조하시면 좋을것같습니다.<br>
 :bangbang: 버전이 달라지는 경우 설치 및 설정 방법이 변할 수 있습니다. 해당 설치 및 설정은**2.36.0(2022.04.18) 버전**을 기준으로 진행하였습니다.

### 2.1 Git 다운로드

 2.1.1 먼저 [여기](https://git-scm.com/download/)에서 Git을 다운로드 해주세요.
  
  ![image](https://user-images.githubusercontent.com/104341003/165985804-88be10e5-e7f8-4cd6-97dc-047c238b7e5e.png)


### 2.2 Git 설치

🔍Next버튼을 눌러주세요. only show new options을 누르면, 다른 옵션들이 나오지 않으니 누르지 말고 진행해주세요.

![image](https://user-images.githubusercontent.com/104341003/165987988-88dba63b-3908-4861-996b-d0c9a9449697.png)

🔍**설치할 구성 요소들을 지정**하고 Next를 눌러줍니다.
화면과 같이 진행하였으며, 아래에 간단한 설명을 추가합니다.
![image](https://user-images.githubusercontent.com/104341003/165988256-59d2adea-83ca-4966-b879-1c235728c548.png)

**Additional icons**
 - On the Desktop : 바탕화면에 바로가기 생성
**Windows Explorer integration**
 - Git Bash Here : 폴더 오른쪽 클릭 메뉴에 Git Bash Here(연결 기능) 추가 ❗필수
 - Git GUI Here : 폴더 오른쪽 클릭 메뉴에 Git GUI Here(연결 기능) 추가 ❗필수
**Git LFS (Large File Support)** : 대용량 파일 지원 ❗필수
**Associate .git* configuration files with the defalut text editor** : 기본 텍스트 에디터에 git 구성(.git 확장자) 연결 ❗필수
**Associate .sh files to be run with Bash** : Bash에 .sh 확장자 파일 연결 ❗필수
**Check daily for git for Windows updates** 윈도우에서 매일 새로운 업데이트 확인
**(NEW!) Add a Git Bash Profile to Windows Terminal** 윈도우 기본 터미널(cmd)에 Git Bash 프로파일 추가 (선택)


🔍**사용할 편집기를 선택합니다.** visual studio code를 저는 가장 많이 사용했기 때문에, vs code를 선택하였고, 다른 편집기를 사용하셔도 괜찮습니다.

![image](https://user-images.githubusercontent.com/104341003/165989593-c2fa3346-693a-4ed0-a62d-4dfef3ae2e27.png)


🔍**Repository(분기) 설정입니다.** 대부분, master를 기본으로 사용하기 때문에 **Let Git decide** 를 선택하였습니다.

![image](https://user-images.githubusercontent.com/104341003/165989861-c5a7ac71-63a6-4d35-b109-52bd6ef6415e.png)


🔍**Git 커맨드를 사용하기위한 설정입니다.** 화면과 같이 **Git from the command line and also from 3rd-party software**를 선택하였습니다. 

**Use Git from Git Bash only** : Git Bash에서만 Git 명령어를 수행할 수 있습니다.
**Git from the command line and also from 3rd-party software** : Git을 환경변수(PATH)에 추가하여 윈도우 기본 명령 프롬프트(CMD) 등에서도 Git 명령어를 수행할 수 있습니다.
**Use Git and optional Unix tools from the Command Prompt** : Git과 Unix 도구 모두 환경변수(PATH)에 추가합니다. 
 ❗ 이 경우 몇 가지 Windows 기본 도구가 새롭게 재정의 됩니다. 이러한 위험을 충분히 숙지하고 있는 경우에만 이 옵션을 사용하기를 권장합니다.

![image](https://user-images.githubusercontent.com/104341003/165990195-d4cc4518-f67c-477e-a2ef-7b1931e5a805.png)


🔍**SSH연결 설정입니다.** 
저는 외부SSH가 없고, Git에서 기본으로 제공되는 OpenSSH를 사용하기위해 화면과 같이 선택하였습니다. 

![image](https://user-images.githubusercontent.com/104341003/165990259-7ef88f11-db8a-4acb-a57c-e6aae4581be4.png)

🔍**HTTP 설정입니다. 역시 기본 설정을 사용하였습니다. **

![image](https://user-images.githubusercontent.com/104341003/165990463-32e8f91e-1f52-4b43-98a8-b372a07f3c8e.png)

윈도우 / 유닉스의 줄바꿈 표기가 달라, 개발환경이 다른곳에서 진행할 경우 문제가될 수 있습니다. 
윈도우에서만 진행할 경우 **Checkout Windows-style, commit Unix-style line endings**를 기본적으로 사용하셔도 괜찮습니다. 

![image](https://user-images.githubusercontent.com/104341003/165990798-451a8217-872a-4f08-94a3-259eb3456679.png)

🔍**Git Bash의 터미널 프로그램 설정입니다.**

**Use MinTTY (the default terminal of MSYS2)** : Git에서 제공하는 기본 터미널 에뮬레이터(MinTTY)를 사용합니다.
**Use Windows' default console window** : 윈도우 기본 터미널(cmd)을 사용합니다.

![image](https://user-images.githubusercontent.com/104341003/165990904-99ce251b-5ca3-4eb8-9bbe-72a2f5d3cb1a.png)

🔍**추후 사용할 pull(기존에 작업했던 내용은 유지하면서 최신 코드로 업데이트) 기능에 대한 설정입니다. **

![image](https://user-images.githubusercontent.com/104341003/165991251-e57fa711-eec9-4f04-9bb3-11d874ad0137.png)

🔍**자격 증명 도움입니다.** 

![image](https://user-images.githubusercontent.com/104341003/165991382-54b94761-12f2-42ad-8e29-7610d5a75a8f.png)

🔍**기타 옵션입니다.**

**Enable file system caching** 파일 시스탬 캐싱을 활성화해 메모리 성능향상을 제공합니다

![image](https://user-images.githubusercontent.com/104341003/165991443-92f4a47a-d303-4f57-91a9-4f7e90221983.png)

🔍**실험적 기능입니다.**
버그가 있다는 얘기가 있어 선택하지 않았습니다. 

![image](https://user-images.githubusercontent.com/104341003/165991604-a74897ae-f193-4521-82a2-cbfa1b1c5656.png)

🔍**설치를 시작해주세요.**

![image](https://user-images.githubusercontent.com/104341003/165992180-762ed6ab-5cb4-43c6-aa7b-0ce4df3a08d7.png)

🔍**설치가 완료되었습니다 Finish를 눌러 종료해주세요.**

![image](https://user-images.githubusercontent.com/104341003/165992528-946a8b9b-b96e-4c7b-9ad8-0badc3e2cc27.png)




## 3. GitHub 사용 방법

## 번외1. GitHub 게시글 제작 방법

## 번외2. Git, GitHub 용어 정리

## 번외3. 기타 사이트 모음
[Git Tip모음](https://github.com/Integerous/git-tips) - Integerous님 GitHub <br>
[GitHub Wiki TOC generator](https://ecotrust-canada.github.io/markdown-toc/)<br>
[GitHub 이모티콘 모음](https://gist.github.com/rxaviers/7360908)<br>

## Reference

### 전체
🎥[Git으로 시작하는 협업 및 오픈소스 프로젝트](https://edu.goorm.io/lecture/11528/git%25EC%259C%25BC%25EB%25A1%259C-%25EC%258B%259C%25EC%259E%2591%25ED%2595%2598%25EB%258A%2594-%25ED%2598%2591%25EC%2597%2585-%25EB%25B0%258F-%25EC%2598%25A4%25ED%2594%2588%25EC%2586%258C%25EC%258A%25A4-%25ED%2594%2584%25EB%25A1%259C%25EC%25A0%259D%25ED%258A%25B8) - 동빈나님 <br>
[어떻게 깃을 사용하는지 빠르게 알아봅시다.](https://www.pigno.se/barn/tutorial-git/docs/#/?id=fearful-%ec%86%8c%ec%8a%a4-%eb%b3%91%ed%95%a9)<br>
[깃허브(GitHub)란?](https://tlsdnjs12.tistory.com/7) - 서스포PAR_개발블로그<br>



### 번외1. GitHub 게시글 제작방법

