# GitHub-getting-started

📝[GitHub](https://github.com/)를 시작해보자.

> 처음 개발을 시작하려보니 깃(Git), 깃허브(GitHub), 커밋(Commit).. 등등 이 중요하답니다.<br>
> 열심히 자료를 찾아봤지만 정확하게 뭐가뭔지 모르겠고 너무어렵더라구요.<br> > **그래서 제가** 이해된 내용들을 개념 ~ 설치 ~ 사용방법까지 하나씩 추가해보도록 하겠습니다.<br>
> Reference를 기반으로 작성할 예정입니다.

## 0. 목차

> 목차와 내용은 계속 수정되고, 업데이트 될 예정입니다.

1. [Git, GitHub란?](#1-git-github란)
2. [Git 설치 및 설정](#2-git-설치-및-설정)
3. [GitHub 사용 방법](#3-github-사용-방법)

번외 1. [GitHub 게시글 제작 방법](#번외1-github-게시글-제작-방법)<br>
번외 2. [Git, GitHub 용어 정리](#번외2-git-github-용어-정리)<br>
번외 3. [기타](#번외3-기타-사이트-모음)

[Truble Shooting](#truble-shooting) -설치 / 설정 / 실행 이슈사항 해결방법

<br>
<br>

## 1. Git, GitHub란?

### Git, GitHub는 무엇이길래 개발자들이 많이 사용할까요?<br>

#### 키워드로보는 Git

```C
#버전관리 #어디서나개발 #협업 #개인포트폴리오 #오픈소스
```

어떤 프로젝트던 **버전관리**는 중요하겠지만 소프트웨어에서는 **버전관리가 중요합니다.**
버전관리란, 시간에 따라 파일의 변화를 기록하여 특정 시점의 버전을 다시 꺼내올 수 있도록 하는 시스템입니다.
이전 버전의 기능을 가져올 수도 있고, 실수로 삭제되거나 여러 개발자가 하나의 프로그램을 제작 할 때
소스코드가 섞이는경우 **복원해야 할 수도 있죠.**

이러한 것들이 모두 가능하게 하는것이 **Git**이라는 프로그램입니다.

깃허브는 이러한 개발자들이 그동한 개발해 왔던 내용들을 버전관리 뿐만이 아니라 **개발 프로젝트를 위한 관리 서비스와 저장소**를 지원합니다.
인터넷이 연결되어있다면 **어디서나 해당 프로그램을 가져와 개발 할 수 있고, 인터넷이 없더라도 미리 저장한 프로그램을 이용해 개발할 수 있습니다.** 물론, 나중에 GitHub로 업로드(추후엔 Push라고 합니다!)도 가능하고요!<br>

또, 깃허브를 사용해 소스를 수정하고, 개발하는 내용과 기간은 모두 기록되므로 **깃허브 자체가 자신의 포트폴리오**가 될 수 있습니다.
협업 프로그램에서는 여러 개발 소스를 병합하여 **언제 누가 무엇을 수정**하였는지 확인할 수 있고 각자 맡은 분야를 개발하여 합치는 **소스 병합**도 지원합니다.

이외에도 인스타그램, 트위터 등 SNS처럼 **다른 개발자들의 소스를 참조하거나, 오픈 소스를 이용해 함께 개발** 할 수도 있습니다.

이러한 굉장한 장점을 가지고 있기 때문에 전세계 개발자들이 많이 사용하고 있습니다.

### Git과 GitHub의 차이점은요?<br>

**GitHub는 Git을 보다 쉽게 사용할 수 있도록 웹에서 사용할 수 있는 도구** 입니다. <br><br>
**Git** : CLI(Command Line Interface)환경의 버전관리 시스템 <br>
**GitHub** : GUI(Grapic User Interface)의 웹페이지 환경에서 Git으로 관리하는 프로젝트를 올려두는 사이트 + 원격으로 저장,관리 및 협업을 위해 여러 시스템들을 제공해주는 사이트 <br>
🎥 **["Git이 영상을 찍는 앱이라면, GitHub는 유튜브 라는 플랫폼이다 라고 생각하면 편하다."](https://www.youtube.com/watch?v=Bd35Ze7-dIw)**

만약 Git에 대해 더 깊게 알아보고 싶다면 [여기](https://git-scm.com/book/ko/v2)를 참조해주세요.

<br>
<br>

## 2. Git 설치 및 설정

❗ 해당 자료는 Windows 기반을 기본으로 안내드리고있습니다. Mac OS를 사용하시는 분들께서는 [이곳](https://sin0824.tistory.com/8)을 참조하시면 좋을것같습니다.<br>
:bangbang: 버전이 달라지는 경우 설치 및 설정 방법이 변할 수 있습니다. 해당 설치 및 설정은**2.36.0(2022.04.18) 버전**을 기준으로 진행하였습니다.

### 2.1 Git 다운로드

2.1.1 먼저 [여기](https://git-scm.com/download/)에서 Git을 다운로드 해주세요.

![image](https://user-images.githubusercontent.com/104341003/165985804-88be10e5-e7f8-4cd6-97dc-047c238b7e5e.png)

<br>

### 2.2 Git 설치

🔍Next버튼을 눌러주세요. only show new options을 누르면, 다른 옵션들이 나오지 않으니 누르지 말고 진행해주세요.

![image](https://user-images.githubusercontent.com/104341003/165987988-88dba63b-3908-4861-996b-d0c9a9449697.png)
<br>
🔍**설치할 구성 요소들을 지정**하고 Next를 눌러줍니다.
화면과 같이 진행하였으며, 아래에 간단한 설명을 추가합니다.

![image](https://user-images.githubusercontent.com/104341003/165988256-59d2adea-83ca-4966-b879-1c235728c548.png)
<br>
<br>
**Additional icons**

- On the Desktop : 바탕화면에 바로가기 생성
  **Windows Explorer integration**<br>
  ❗필수 - Git Bash Here : 폴더 오른쪽 클릭 메뉴에 Git Bash Here(연결 기능) 추가 <br>
  ❗필수 - Git GUI Here : 폴더 오른쪽 클릭 메뉴에 Git GUI Here(연결 기능) 추가<br>
  ❗필수 **Git LFS (Large File Support)** : 대용량 파일 지원 <br>
  ❗필수 **Associate .git configuration files with the defalut text editor** : 기본 텍스트 에디터에 git 구성(.git 확장자) 연결<br>
  ❗필수 **Associate .sh files to be run with Bash** : Bash에 .sh 확장자 파일 연결 <br>
  **Check daily for git for Windows updates** 윈도우에서 매일 새로운 업데이트 확인<br>
  **(NEW!) Add a Git Bash Profile to Windows Terminal** 윈도우 기본 터미널(cmd)에 Git Bash 프로파일 추가 (선택)
<br>
<br>
🔍**사용할 편집기를 선택합니다.**
visual studio code를 저는 가장 많이 사용했기 때문에, vs code를 선택하였고, 다른 편집기를 사용하셔도 괜찮습니다.

![image](https://user-images.githubusercontent.com/104341003/165989593-c2fa3346-693a-4ed0-a62d-4dfef3ae2e27.png)
<br>
<br>
🔍**Repository(저장소) 설정입니다.**
대부분, master를 기본으로 사용하기 때문에 **Let Git decide** 를 선택하였습니다.
>2022.05.03 변경내용 2020년 10월부터 master 용어를 잘 사용하지 않음으로, 아래를 선택한후 main으로 변경해주세요

![image](https://user-images.githubusercontent.com/104341003/165989861-c5a7ac71-63a6-4d35-b109-52bd6ef6415e.png)


<br>
<br>
🔍**Git 커맨드를 사용하기위한 설정입니다.**
화면과 같이 **Git from the command line and also from 3rd-party software**를 선택하였습니다.

**Use Git from Git Bash only** : Git Bash에서만 Git 명령어를 수행할 수 있습니다.
**Git from the command line and also from 3rd-party software** : Git을 환경변수(PATH)에 추가하여 윈도우 기본 명령 프롬프트(CMD) 등에서도 Git 명령어를 수행할 수 있습니다.
**Use Git and optional Unix tools from the Command Prompt** : Git과 Unix 도구 모두 환경변수(PATH)에 추가합니다. <br>
이 경우 몇 가지 Windows 기본 도구가 새롭게 재정의 됩니다. 이러한 위험을 충분히 숙지하고 있는 경우에만 이 옵션을 사용하기를 권장합니다.<br>

![image](https://user-images.githubusercontent.com/104341003/165990195-d4cc4518-f67c-477e-a2ef-7b1931e5a805.png)
<br>
<br>
🔍**SSH연결 설정입니다.**
저는 외부SSH가 없고, Git에서 기본으로 제공되는 OpenSSH를 사용하기위해 화면과 같이 선택하였습니다.

![image](https://user-images.githubusercontent.com/104341003/165990259-7ef88f11-db8a-4acb-a57c-e6aae4581be4.png)
<br>
<br>
🔍**HTTP 설정입니다.**
역시 기본 설정을 사용하였습니다.

![image](https://user-images.githubusercontent.com/104341003/165990463-32e8f91e-1f52-4b43-98a8-b372a07f3c8e.png)

윈도우 / 유닉스의 줄바꿈 표기가 달라, 개발환경이 다른곳에서 진행할 경우 문제가될 수 있습니다.
윈도우에서만 진행할 경우 **Checkout Windows-style, commit Unix-style line endings**를 기본적으로 사용하셔도 괜찮습니다.

![image](https://user-images.githubusercontent.com/104341003/165990798-451a8217-872a-4f08-94a3-259eb3456679.png)
<br>
<br>
🔍**Git Bash의 터미널 프로그램 설정입니다.**

**Use MinTTY (the default terminal of MSYS2)** : Git에서 제공하는 기본 터미널 에뮬레이터(MinTTY)를 사용합니다.
**Use Windows' default console window** : 윈도우 기본 터미널(cmd)을 사용합니다.

![image](https://user-images.githubusercontent.com/104341003/165990904-99ce251b-5ca3-4eb8-9bbe-72a2f5d3cb1a.png)
<br>
<br>
🔍**추후 사용할 pull(기존에 작업했던 내용은 유지하면서 최신 코드로 업데이트) 기능에 대한 설정입니다.**

![image](https://user-images.githubusercontent.com/104341003/165991251-e57fa711-eec9-4f04-9bb3-11d874ad0137.png)
<br>
<br>
🔍**자격 증명 도움입니다.**

![image](https://user-images.githubusercontent.com/104341003/165991382-54b94761-12f2-42ad-8e29-7610d5a75a8f.png)
<br>
<br>
🔍**기타 옵션입니다.**

**Enable file system caching** 파일 시스탬 캐싱을 활성화해 메모리 성능향상을 제공합니다

![image](https://user-images.githubusercontent.com/104341003/165991443-92f4a47a-d303-4f57-91a9-4f7e90221983.png)
<br>
<br>
🔍**실험적 기능입니다.**
버그가 있다는 얘기가 있어 선택하지 않았습니다.

![image](https://user-images.githubusercontent.com/104341003/165991604-a74897ae-f193-4521-82a2-cbfa1b1c5656.png)
<br>
<br>
🔍**설치를 시작해주세요.**

![image](https://user-images.githubusercontent.com/104341003/165994016-ee8c8f68-108c-42bb-bf78-25a2a249aaae.png)
<br>
<br>
🔍**설치가 완료되었습니다 Finish를 눌러 종료해주세요.**

![image](https://user-images.githubusercontent.com/104341003/165994118-4e916000-995b-4bef-9a30-d51c71b9e34e.png)

검색창에서 GitBash를 입력하여 실행해주세요.
<br>
<br>
![image](https://user-images.githubusercontent.com/104341003/166193856-422fb601-8bb9-4089-878e-ae08a17caeea.png)

실행한 Git Bash에서 git version을 확인해 다음 사진과 같이 나오면 정상적으로 설치되었음을 확인할 수 있습니다.
<br>
```C

git --version

```

![image](https://user-images.githubusercontent.com/104341003/166300088-f47b5d61-1e1f-46cb-a42c-6227e17ac9df.png)

<br>
<br>

### 2.3 GitHub 가입

GitHub를 이용하기 위해서는 반드시 계정이 필요합니다. 만약 GitHub에 가입이 되어있다면 [2.4 Git 설정 및 GitHub 연동](#24-git-설정-및-github-연동)으로 이동하셔도 좋습니다.<br>
GitHub는 [여기](https://github.com)에서 가입이 가능합니다.

우측 상단의 Sign up을 클릭하여 가입할 수 있습니다.
<br>
![image](https://user-images.githubusercontent.com/104341003/166183718-4080e315-66f4-42c4-ae4e-fe9354d75604.png)
<br>
<br>
사용할 메일주소, 비밀번호, GitHub에서 사용할 닉네임 입력, 광고/업데이트 관련 메일 수신여부 및 로봇이 아닙니다.를 설정하면 이메일 인증으로 넘어가집니다.

![image](https://user-images.githubusercontent.com/104341003/166184179-6956b84b-bf9c-4027-80f6-f93b6019de09.png)
<br>
<br>
아이디로 사용할 이메일 편지함에서 인증코드를 확인하여 인증을 진행해주세요.
<br>
![image](https://user-images.githubusercontent.com/104341003/166184564-18460205-9fae-417d-bd3e-82b5582ccc21.png)

<br>
<br>

**만약 가입 시 메일이 오지않는다면**

resend the code를 클릭해 다시 메일을 보내거나 혹은<br>
[가입 시 이메일 주소를 잘못 입력하였을 경우](#가입-시-이메일-주소를-잘못-입력하였을-경우)를 참조해주세요.

<br>
<br>

### 2.4 Git 설정 및 GitHub 연동

> **Git 설정 및 Github 연동** 전, 간단하게 git에서 사용하는 용어에 대해 알아보겠습니다.

```C

로컬(Local) : 내 PC (혹은 작업하고 있는 PC)
원격(Remote) : 원격 서버 (Git/GitHub에서 원격은 보통 GitHub를 의미함)
작업공간(WorkSpace) : 소스코드, 폴더들이 들어있는 프로젝트 폴더
저장소(Repository) : 내가 관리할 작업공간을 Git이 제공하는 자료구조 안에 압축시켜 넣은것 (git init 명령어를 실행하면, 해당 파일안에 .git 폴더가 생성되며 이 작업공간의 .git 폴더를 저장소라고 함.)
커밋(Commit) : 프로젝트(파일 및 폴더)의 추가/변경사항을 저장소에 기록하는 것(어떤 프로젝트의 Save파일을 만들어 저장소에 저장하는것 라고 생각하면 편합니다.)

```

### 2.5 Git 설정

git을 사용하기 위해 최초 설정을 진행합니다 .

먼저 사용자 이름과 이메일을 설정합니다.
설정하는 이유는 **git**을 이용해 **커밋(commit)** 할 때 사용자 이름과 이메일이 기록되기 때문에 먼저 설정해둡니다.
한번만 설정하면 나중에는 설정할 필요가 없습니다.

다음 명령어를 Git Bash에서 실행합니다.

```C

git config --global user.name "사용자 이름"
git config --global user.email "사용자 이메일"

```

![image](https://user-images.githubusercontent.com/104341003/166198325-06dcb6d4-0204-4449-bbd8-6f0d4744c253.png)

입력이 제대로 되었는 지 다음 명령어를 입력합니다.

```C

git config --list

```

![image](https://user-images.githubusercontent.com/104341003/166198435-d6142efe-2875-431b-ae07-86784e8bd072.png)

<br>
<br>

### 2.6 Git 맛보기

우선 연습용 **작업공간(WorkSpace)을** 하나 만들어보겠습니다. (연습용이 아닌 실제 프로젝트로 진행하셔도 좋습니다.)

![image](https://user-images.githubusercontent.com/104341003/166199291-0409f45d-e6a6-4739-9095-852858926e27.png)
<br>
<br>
저는 이름을 **TestWorkSpace** 로 지정하였습니다

해당 폴더안에 **테스트폴더** 와 **테스트소스코드.txt** 파일을 만들었습니다.

![image](https://user-images.githubusercontent.com/104341003/166199534-c2b45d99-e33a-4d32-95b6-408f9934a6ac.png)
<br>
<br>
해당 **작업공간(WorkSpace)** 에서 commit을 빠르게 진행하기위해 폴더 내에서 마우스 우클릭 - **Git Bash Here**을 선택합니다.

![image](https://user-images.githubusercontent.com/104341003/166199628-ced50e14-186d-48e0-8c40-fc103e16f76c.png)
<br>
<br>
**Git Bash Here**을 선택하면, 해당 위치를 따로 설정하지 않아도 작업공간으로 위치를 설정합니다.

![image](https://user-images.githubusercontent.com/104341003/166199977-cc85e182-a77c-465d-a3d7-4271979d585f.png)
<br>
<br>
해당 **작업공간(WorkSpace)** 을 **저장소(Repository)** 로 관리하기 위해 `git init`로 저장소를 초기화 합니다.
<br>
```C

git init

```

명령어를 입력하면, Git Bash에는 `Initialized empty Git repository` (비어있는 **저장소(Repository)** 를 생성했다.)라는 문구와 함께 **작업공간(WorkSpace)** 에 .git폴더가 생성됨을 확인 할 수 있습니다.

![image](https://user-images.githubusercontent.com/104341003/166200219-bd052b92-14cc-4e7b-857d-b2d6d0c36ea7.png)
<br>

.git 폴더가 보이지 않는경우 **폴더 위 보기 - 표시/숨기기**의 숨긴항목 체크

![image](https://user-images.githubusercontent.com/104341003/166200379-a9ae6d34-6842-4c38-abda-526aaf65b53b.png)
<br>
<br>
그렇다면 저장소도 생성했으니 **커밋(Commit)** 을 해보도록 하겠습니다. **커밋(Commit)** 명령어는 다음과 같습니다.
<br>
```C

git commit -m "어떤 내용을 기록/변경 하는지 메모 남기기"

```

다음과 같이 커밋하겠습니다. `git commit -m "Hello, git"`

![image](https://user-images.githubusercontent.com/104341003/166201925-03a37ec7-f7e6-482e-aad6-8bab85732404.png)
<br>
<br>
다음과 같은 오류메세지 `nothing added to commit but untracked files present (use "git add" to track)`과 함께 커밋에 실패했습니다. <br>
**notthing added to commit** 커밋을 위해 add된 파일이 없습니다. <br>
**untracked files present** Git에 의해 아직 추적되고있지 않아 버전관리 대상이 아니다. 라는 뜻입니다.
**use** `git add` **to track** git add를 이용해 track 하라고 되어있네요. 한마디로,

커밋을 하기 전에는 반드시 **커밋할 파일들을 미리 지정** 해야합니다. <br>
파일을 새로 생성하거나 원래 있던 파일들을 수정한 내용을 .git에 기록하는 것이 커밋입니다.
해당 작업을 하는 부분이 바로 `add` 입니다.

파일들을 add해보겠습니다. 명령어는 `git add 파일이름.파일확장자` 입니다.
<br>
```C
git add 테스트폴더
git add 테스트소스코드.txt
```

![image](https://user-images.githubusercontent.com/104341003/166207424-d009e6da-d271-4a93-b7f7-bdbb3ededabe.png)
<br>
<br>
이렇게 **작업공간(Work Space)** 에서 **로컬 저장소(Local Repository)** 만들기, **커밋(commit)** 까지 진행해보았습니다. <br>

![image](https://user-images.githubusercontent.com/104341003/166229869-a338ba6d-3e03-4bec-aac1-0c9db2fd009b.png)
<br>
<br>
아래 사진은 **브랜치(branch)** 에 대한 내용을 제가 오늘 만들어 낸 커밋파일과 맞춰 제작하였습니다.<br>
최초의 `git init`를 통해 master branch를 생성하고, add 파일 - commit을 통해 하나의 시점을 추가했습니다. <br>

이후 이렇게 버전별로 추가하게 되면 업데이트가 되고, **커밋(Commit)** 할 때 마다 master branch가 계속해서 생성되겠죠! <br>
브랜치(Branch)에 대한 설명은 추후에 추가하도록 하겠습니다. 브랜치에 대해 자세히 알고싶으시다면 [여기](https://git-scm.com/book/ko/v2/Git-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EB%B8%8C%EB%9E%9C%EC%B9%98%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80)를 참조해주세요. 혹은 [여기](https://gmlwjd9405.github.io/2018/05/11/types-of-git-branch.html)를 확인해주시면 좋을 것 같습니다.<br>

![image](https://user-images.githubusercontent.com/104341003/166297029-55c75c04-ad6c-41d5-80ca-b1c90e0bc9f9.png)
<br>

> 2022.05.03 추가 : ```git init```를 진행하면 해당 폴더가 자동으로 ```master``` 로 지정이 되나, 2020 10월 이후로 국제사회에서 master/slave, blacklist/whitelist 등 변경하는 운동이 많아짐에 따라 GitHub에서는 ```master```를 ```main```으로 변경되었습니다. 자세한 내용은 [여기](https://kyeoneee.tistory.com/72)를 참조하세요.<br>
> Local만 사용할 경우 문제가 없지만, GitHub를 연동 하는 경우  우리가 사용하는 Branch도 main으로 변경하여야지만 정상적으로 GitHub에 업로드가 가능합니다.<br>

```C

git branch -M main

```
명령어를 통해 작업공간을 master에서 main으로 변경합니다.

![image](https://user-images.githubusercontent.com/104341003/166297333-a8f065fd-5ef3-4953-9cb6-ddb40ee3581b.png)


<br>
<br>

## 3. GitHub 사용 방법

### 3.1 GitHub 연동 -SSH키 만들기

> 우리는 지금까지 Git을 설치하고, 간단하게 버전관리하는 방법을 알아봤습니다.
> 이번에는 다양한 협업 기능을 제공하는 GitHub를 연동하여 사용하는 방법에 대해 알아보겠습니다.

GitHub를 사용하려면 **SSH 키** 를 먼저 등록해야 합니다.

> SSH 키란? **안전한 셸(Secure SHell)** 로 CLI(Command Line Interface)에서 다른 PC 혹은 서버에 연결하기 위한 인증 방법입니다.
> 사용자, 패스워드 등 다양한 인증방법을 지원하지만, 편리성, 안정성 면에서 추천하는 방법은 **공개키 인증 방식** 입니다.
> 공개키 인증 방식을 사용하려면 공개키와 개인키를 한 쌍을 만들어 공개키를 서버에 미리 등록해두면, 사용자는 개인키를 통해 SSH에 접속하고 공개키에 일치하는 부분이 있으면 인증에 성공하여 서버에 접속되는 방식입니다.

```C

ssh-keygen

```

명령어를 이용해 ssh key를 생성합니다.

먼저 저장할 위치를 물어봅니다. `Generating public/private rsa key pair. Enter file in which to save the key (/c/Users/유저이름/.ssh/id_rsa):`
기본값을 사용하기위해 그냥 Enter키를 눌러 다음으로 넘어갑니다.

다음으로는 SSH 추가 Password를 지정할 것인지 물어봅니다. 추가 패스워드는 나중에 지정할 수 있으므로 우선 Enter를 **두 번** 눌러 키를 생성합니다.합니다.
<br>
![image](https://user-images.githubusercontent.com/104341003/166234591-da503b68-1c47-4f5c-9153-ef29487d2fb4.png)
<br>
<br>
생성된 ssh키는
**개인키(Private Key)** `id_rsa` 와
**공개키(Secret Key)** `id_rsa.pub` 두개를 생성합니다.

**개인키(Private Key)** 는 **절대 외부에 공개되면 안되는 키**입니다.
생성된 키 중 **공개키(Secret Key)**를 복사하여 자신의 GitHub에 등록합니다.

```C

cat ~/.ssh/id_rsa.pub

```

![image](https://user-images.githubusercontent.com/104341003/166235494-e6ad5419-07fc-45d9-8ee2-09b4c834f6c1.png)
<br>
<br>
화면에 출력된 키(ssh-rsa ~~ 컴퓨터 이름)를 마우스로 드래그하여 복사합니다.

복사하는 방법은 다음과 같습니다.

> 1.  마우스 우클릭 - 복사(Copy)<br>
> 2.  키보드 복사 <br> > _(windows CMD 또는 터미널 등) `Ctrl`+`C` <br> > _(git bash) `Ctrl`+`Insert` <br> > \*(MacOS) `Command`+`C` <br>

메모장에 붙여넣기하여 복사가 잘 되었는 지 확인후, github에 공개키를 등록합니다.

<br>

### 3.2 GitHub 연동 - 공개키를 GitHub 계정에 등록하기

[Git Hub](https://github.com/settings/keys)로 이동해 SSH Key를 등록합니다.

![image](https://user-images.githubusercontent.com/104341003/166236847-00e82b20-d692-4391-a358-1ddab4dca501.png)
<br>
Title에는 사용자 임의로 제목을 입력합니다.
Key에는 이전에 복사한 **공개키(Secret Key)** 를 붙혀넣기 한 후 Add SSH key를 눌러 등록합니다.

![image](https://user-images.githubusercontent.com/104341003/166237155-da472ca2-b2db-46e4-8ba7-845bbd91433b.png)
<br>
정상적으로 등록된 경우 아래 사진처럼 추가됩니다.

![image](https://user-images.githubusercontent.com/104341003/166237401-6e4f517f-2021-49c7-a4cc-b9f0e3e5c737.png)


SSH 키가 정상적으로 등록되었는 지 확인하기 위해 원격 저장소(Remote Repository)에서 자신의 로컬 저장소(Local Repository)로 복제가된다면, 정상적으로 연결이 된겁니다.<br>

[원격 저장소 복제(Clone)하기](#34-github-원격-저장소remote-repository-복제clone하기) <br>


원격 저장소 복제(Clone) 혹은 공개키를 GitHub 계정에 등록하기를 실패했을경우, [SSH키를 계정에 등록하였는데도 안되는경우](#ssh키를-계정에-등록하였는데도-안되는경우)를 클릭하여 확인해보세요.

<br>
<br>

### 3.3 GitHub 에서 원격 저장소(Remote Repository) 만들기

Github는 원격에서 Git **저장소(Repository)** 를 호스팅 해주는 서비스입니다. GitHub에서는 GUI환경의 웹에서 **원격 저장소(Remote Repository)** 를 간단하게 생성하고 관리할 수 있습니다.

[GitHub](https://github.com)를 맨처음 로그인 하게되면 다음과 같은 웹페이지가 나옵니다.
<br>
![image](https://user-images.githubusercontent.com/104341003/166258618-0e270227-5351-4afb-8576-8666370f20f7.png)
<br>
<br>
**원격 저장소(Remote Repository)** 를 만들기위해

1. GitHub에 로그인되어있다면 [여기](https://github.com/new)를 클릭하세요.
2. 혹은 GitHub 메인 홈페이지의 New를 누릅니다.
<br>
사용할 **원격 저장소의 이름(Repository name)** 을 입력합니다.

> 개발 언어 혹은 환경마다 통상적으로 사용하는 규칙 혹은 스타일이 있습니다.<br> >[여기](http://developer.gaeasoft.co.kr/development-guide/workflow/gitlab-style-guide/)에 자세하게 나와있으며<br>
> stack overflow [답변](https://stackoverflow.com/questions/11947587/is-there-a-naming-convention-for-git-repositories)을 참조하세요.

![image](https://user-images.githubusercontent.com/104341003/166259083-0324f2ba-ce41-487d-9fd2-94daed2b6783.png)
<br>
<br>

해당 **저장소(Repository)** 의 간단한 설명을 입력합니다.

![image](https://user-images.githubusercontent.com/104341003/166260644-669b505e-4e67-44b5-9af8-e3d16af7f807.png)

공개 여부를 선택합니다.<br>
**Public** : 전체 공개
**Private** : 선택적 공개

![image](https://user-images.githubusercontent.com/104341003/166260830-62f68c93-9849-4c52-ac3b-e11c055f34d7.png)

**저장소(Repository)** 초기화 입니다. 모두 선택 후 Create repository를 눌러 저장소를 새로 제작합니다.

**Add a README file** : 해당 **저장소(Repository)** 에 대한 자세한 설명이나 사용 방법에 대해 서술하는 파일을 만듭니다.<br>
**Add .gitignore** : 지정한 확장자 파일을 무시합니다. (Git 버전 관리에서 제외할 파일 목록을 지정하는 파일 지정)<br>
**Choose a license** : 라이센스를 선택합니다. (자세한 내용은 [여기](https://flyingsquirrel.medium.com/github-license%EC%9D%98-%EC%A2%85%EB%A5%98%EC%99%80-%EB%82%98%EC%97%90%EA%B2%8C-%EB%A7%9E%EB%8A%94-%EB%9D%BC%EC%9D%B4%EC%84%A0%EC%8A%A4-%EC%84%A0%ED%83%9D%ED%95%98%EA%B8%B0-ae29925e8ff4)를 확인하세요)<br>
<br>
![image](https://user-images.githubusercontent.com/104341003/166262010-d077f4b1-fab2-4100-bd49-a8cc98b887d2.png)

<br>
<br>

### 3.4 GitHub 원격 저장소(Remote Repository) 복제(Clone)하기

```clone``` 명령어는 **원격 저장소(Remote Repository)** 에 있는 소스코드나 프로젝트들을 복사하여 **로컬 저장소(Local Repository)** 로 가지고오고 싶을 때(복제), 사용하는 명령어 입니다.

먼저 **복제(Clone)** 하려는 **원격 저장소(Remote Repository)** 에 접속합니다. 

저는 여러분들이 지금 읽고 있는 이 **저장소(Repository)[https://github.com/ItsWard/GitHub-getting-started]** 를 이용해 예제를 들겠습니다.


Git과 GitHub가 어떤 방식으로 연결되었는지(**SSH 인증방식/HTTP 인증방식**)에 따라 해당 하는 인증방식을 선택 후 주소를 복사하여 ```git clone```명령어를 입력합니다.

![image](https://user-images.githubusercontent.com/104341003/166293321-c743ce7f-a7ec-4830-99d2-033fc8fc7efb.png)



> SSH 인증방식의 경우

```C

git clone git@github.com:ItsWard/GitHub-getting-started.

```
<br>


> HTTPS 인증방식의 경우

```C

git clone https://github.com/ItsWard/GitHub-getting-started.git

```
<br>


> git bash 붙혀넣기
>
>  ```Shift``` + ```Insert```

![image](https://user-images.githubusercontent.com/104341003/166239332-78173e1c-42d9-4458-a002-b7dd9f8dcddb.png)
<br>
사용자가 등록한 SSH키와 복사하려는 **저장소(Remote Repository)** 의 이름이 다른경우
`This key is not known by any other names. Are you sure you want to continue connecting (yes/no/[fingerprint])?` 와 같이 나오게되는데, ```yes```를 입력합니다.

![image](https://user-images.githubusercontent.com/104341003/166239664-36bd9d3e-2d77-439f-869c-3f4c55bc470f.png)
<br>
정상적으로 복제가 완료되었다면 ls 명령어를 이용해 확인이 가능합니다.

![image](https://user-images.githubusercontent.com/104341003/166239545-075b7176-0d7a-4dc8-89bb-411075e1b382.png)

혹은 해당 폴더에 들어가면 **저장소(Repository)** 가 복제 되어있는 것을 볼 수 있습니다.

![image](https://user-images.githubusercontent.com/104341003/166239451-debc6e4b-f211-4e48-b0c2-e9c196672d5b.png)
 

### 3.5 GitHub 원격 저장소(Remote Repository)에 push 하기

push 전 알고 넘어가야 할 용어에 대해 소개합니다.<br>

>```origin``` : **원격 저장소(Remote Repository)** 의 단축이름 <br>
> Git에서 해당 **저장소(Repository)** 인 GitHub-getting-started 대신 origin으로 사용가능 <br>
> ex) ```git push origin main``` = ```git push GitHub-getting-started main``` <br>
한번이라도 ```init```하거나 ```clone```하는경우 자동으로 origin에 **원격 저장소(Remote Repository)** 의 이름이 저장된다고 생각하면 됩니다. <br>

우리는 **2.6 Git 맛보기** 에서 **로컬 저장소(Local Repository)** 에 ```commit``` 하는 것 까지 진행했습니다.
```push```는 ```commit```된 **로컬 저장소(Local Repository)** 를 **원격 저장소(Remote Repository)** 에 업데이트해 주는 기능입니다. 

준비사항 : 로컬 저장소, 원격 저장소



>추가 예정입니다.
<br>
<br>

### 3.6 GitHub 원격 저장소(Remote Repository)에서 pull 하기
>추가 예정입니다.
<br>
<br>

### 3.7 GitHub 게시물 가져오기(Fork)
>추가 예정입니다.
```Fork``` 는 **원격 저장소(Remote Repository)** 에 있는 소스코드나 프로젝트들을 복사하여 내 GitHub의 **원격 저장소(Remote Repository)** 로 복제하고 싶을 때, 사용하는 기능입니다.
<br>
<br>

### 3.8 GitHub Pull Request 하기
>추가 예정입니다.
<br>
<br>

## 번외1. GitHub 블로그 게시글 제작 방법
>추가 예정입니다.
<br>
<br>

## 번외2. Git, GitHub 용어 정리
>추가 예정입니다.
<br>
<br>

## 번외3. 기타 사이트 모음

[Git Tip모음](https://github.com/Integerous/git-tips) - Integerous님 GitHub <br>
[GitHub Wiki TOC generator](https://ecotrust-canada.github.io/markdown-toc/)<br>
[GitHub 이모티콘 모음](https://gist.github.com/rxaviers/7360908)<br>
[마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601)<br>
[Git 이름 스타일 가이드](http://developer.gaeasoft.co.kr/development-guide/workflow/gitlab-style-guide/)
[매력적인 깃허브 프로필을 만들어보아요](https://butter-shower.tistory.com/142)

## Truble Shooting

### 가입 시 이메일 주소를 잘못 입력하였을 경우

만약 가입할 때, 이메일 주소를 잘못 입력하였을 경우, 이메일 인증 과정을 진행 할 수 없습니다. 이 경우 Update your email address에 클릭합니다.

![image](https://user-images.githubusercontent.com/104341003/166184590-b6b25d51-ca4b-4c80-aa02-c55830cd0df0.png)

Add email address에 해당 이메일을 다시 입력한 후 Unverified - Resend Verification email을 클릭하여 인증을 다시 진행해주세요.

이후 잘못된 이메일은 우측 상단 쓰레기통 메뉴를 눌러 제거합니다.

![image](https://user-images.githubusercontent.com/104341003/166185078-55fc12a9-e0ea-4adc-ad8c-097fef86bafc.png)

![image](https://user-images.githubusercontent.com/104341003/166185229-7dcabd6a-d164-441e-a2dc-e108f313af78.png)

<br>
<br>

### SSH키를 계정에 등록하였는데도 안되는경우

**(공통)SSH키 재설정**

1. Github - Settings - SSH keys 에 등록한 공개키 삭제합니다.<br>
2. 프롬프트에 cat ~/.ssh/id_rsa.pub 명령어를 입력하여 나타나는 공개키를 다시 복사합니다.<br>
3. Github - Settings - SSH keys 에서 New SSH key 버튼 클릭합니다.<br>
4. Title을 입력하고, 복사한 공개키를 Key에 붙여 넣고 Enter 키를 입력해 한 줄을 추가(개행)<br>
5. Add SSH key 버튼을 클릭하고, 승인하여 공개키를 등록<br>

---

**GitHub CLI 설치(Windows) - HTTPS 인증**
[여기](https://cli.github.com/)에서 github cli를 다운로드합니다.

![image](https://user-images.githubusercontent.com/104341003/166245942-a38a338e-5003-4dbc-8456-3f33e4ce8c07.png)

다음과 같이 설치합니다.

![image](https://user-images.githubusercontent.com/104341003/166246051-536df8e2-1918-4b1b-a432-fe9953bd098c.png)
![image](https://user-images.githubusercontent.com/104341003/166246083-898b636a-ab22-4a40-a123-26767e5a3f23.png)
![image](https://user-images.githubusercontent.com/104341003/166246108-b10e04f1-7607-40d4-919f-18ed8cfa1ee3.png)

`gh --version`명령어를 입력했을 때 다음과 같이 버전이 확인되면 정상적으로 설치된 것입니다.

```C

gh --version

```

![image](https://user-images.githubusercontent.com/104341003/166248613-87de2b50-dc79-4d06-b7c5-a0e43a8b3d72.png)

`winpty gh auth login` 명령어를 입력해 로그인을 시도합니다.

```C

winpty gh auth login

```

## <br>

**macOS 환경**

`brew install gh` 명령어를 이용해 GitHub CLI를 설치합니다.

```C

brew install gh

```

`gh --version`명령어를 입력했을 때 다음과 같이 버전이 확인되면 정상적으로 설치된 것입니다.

```C

gh --version

```

`gh auth login` 명령어를 입력해 로그인을 시도합니다.

```C

gh auth login

```

---

#### Git CLI을 이용한 인증과정 진행

방향키와 Enter를 이용하여 git Bash 혹은 터미널 창에서 선택할 수 있습니다. <br>
`? What account do you want to log into?` -> `GitHub.com`을 선택합니다.

![image](https://user-images.githubusercontent.com/104341003/166248923-a9da253d-b15d-4bc2-a812-480b9e255f98.png)

`SSH`로 인증을 실패하였으므로 `HTTPS`를 선택해 인증을 진행합니다.<br>
? What is your preferred protocol for Git operations? -> `HTTPS`

![image](https://user-images.githubusercontent.com/104341003/166249198-e764d24a-ad31-4a99-a773-709c92f81c49.png)

Git허브 인증으로 Git을 인증할건지를 선택합니다. <br>
`? Authenticate Git with your GitHub credentials?` -> `Y`

![image](https://user-images.githubusercontent.com/104341003/166249958-da1e5c29-6654-4939-a53c-1f110cde1363.png)

GitHub 로그인 방법을 선택합니다. <br>
`? How would you like to authenticate GitHub CLI?`->`Login with a web browser`

![image](https://user-images.githubusercontent.com/104341003/166249996-ddac1fff-df99-4912-86ad-f30f898bdc3b.png)

Enter를 누르지 말고 `! First copy your one-time code`를 미리 메모장에 복사해 둡니다. 이후 Enter를 누르면 GitHub 인증코드 입력 페이지가 나옵니다.

![image](https://user-images.githubusercontent.com/104341003/166250305-67a1c0a3-c812-41b0-ad7f-a39c4b49b2e3.png)

![image](https://user-images.githubusercontent.com/104341003/166250658-1266d4a4-c648-4fd4-844d-c4b517d8e58d.png)

**Authorize GitHub** 를 클릭하여 Git과 GitHub를 연동합니다.

![image](https://user-images.githubusercontent.com/104341003/166250714-5a1c970c-7a12-4447-9e4f-226804a21efa.png)

연동이 완료되었으면 Git과 GitHub에서 연결완료가 되었다고 나옵니다.<br>
![image](https://user-images.githubusercontent.com/104341003/166250984-c6b71527-e5f1-4dfc-8f6d-eaf0bf8723af.png) <br>
![image](https://user-images.githubusercontent.com/104341003/166251196-4bf83f81-9e7d-4341-a341-a88f5ec0adc8.png) <br>




![image](https://user-images.githubusercontent.com/104341003/166263280-352979c4-b6ce-4165-b767-29b93eadbe62.png)

`ls` 명령어로 정상적으로 **복제(clone)** 한 것을 확인할 수 있고

![image](https://user-images.githubusercontent.com/104341003/166263321-c54efb06-41b7-443f-9094-966e37918cd3.png)

<br>

혹은 폴더에서 정상적으로 **복제(clone)** 한 것을 확인할 수 있습니다.

![image](https://user-images.githubusercontent.com/104341003/166263424-aceceec5-bb38-4154-aab0-fa6f541f650d.png)

<br>

### Git 기본 브랜치 master 에서 main으로 변경하기

위에서 언급한 내용이지만, 설치 시 Git Repository 설정을 master로 한 경우 main으로 변경할 수 있는 방법을 공유드립니다.

>  ```git init```를 진행하면 해당 폴더가 자동으로 ```master``` 로 지정이 되나, 2020 10월 이후로 국제사회에서 master/slave, blacklist/whitelist 등 변경하는 운동이 많아짐에 따라 GitHub에서는 ```master```를 ```main```으로 변경되었습니다. 자세한 내용은 [여기](https://kyeoneee.tistory.com/72)를 참조하세요.<br>
> Local만 사용할 경우 문제가 없지만, GitHub를 연동 하는 경우  우리가 사용하는 Branch도 main으로 변경하여야지만 정상적으로 GitHub에 업로드가 가능합니다.<br>

```C

git config --global init.defaultBranch main

```

해당 설정 이후 ```init``` 혹은 ```clone```으로 생성된 브랜치는 ```main```으로 변경됩니다.<br>
다만 이전 ```master```로 되어있는 브랜치는 수동으로 ```main``` 으로 변경 하여야 합니다.<br>

```C

git branch -M main

```




## Reference

### 전체

[코드스테이츠](https://codestates.com/)
🎥[Git으로 시작하는 협업 및 오픈소스 프로젝트](https://edu.goorm.io/lecture/11528/git%25EC%259C%25BC%25EB%25A1%259C-%25EC%258B%259C%25EC%259E%2591%25ED%2595%2598%25EB%258A%2594-%25ED%2598%2591%25EC%2597%2585-%25EB%25B0%258F-%25EC%2598%25A4%25ED%2594%2588%25EC%2586%258C%25EC%258A%25A4-%25ED%2594%2584%25EB%25A1%259C%25EC%25A0%259D%25ED%258A%25B8) - 동빈나님 <br>
[어떻게 깃을 사용하는지 빠르게 알아봅시다.](https://www.pigno.se/barn/tutorial-git/docs/#/?id=fearful-%ec%86%8c%ec%8a%a4-%eb%b3%91%ed%95%a9)<br>
[깃허브(GitHub)란?](https://tlsdnjs12.tistory.com/7) - 서스포PAR\_개발블로그<br>
[GITHUB입문 Git 설치하기](https://taewow.tistory.com/13) - 코딩의행복블로그<br>
[Git허브 브랜치](https://www.youtube.com/watch?v=RYfO6-hPBdw) - 베르의 게임 개발 유튜브<br>
[[Windows 10] Git 최신 버전 설치 및 사용 방법](https://www.lainyzine.com/ko/) - LainyZine: 프로그래머 가이드<br>
[GitHub Git 브랜치의 종류 및 사용법 (5가지)](https://gmlwjd9405.github.io/2018/05/11/types-of-git-branch.html) -HeeJeong Kwon님의 블로그<br>
[누구나 쉽게 이해할 수 있는 Git 입문](https://backlog.com/git-tutorial/kr/stepup/stepup1_3.html)<br>

### 번외1. GitHub 게시글 제작방법
