
------------------------------------------------
## 필기 

git -> 커피 / github -> 커피샵 
git : 내 컴퓨터에 있는 모든 파일의 변화를 기록 -> github라는 공간에 올려줌
ㄴ 장점 : 
1. 같은 파일에 대한 각기 다른 버전 보관
-> 수정 타임라인 각각의 파일을  ('버전관리') 
2. 공통적인 변경 사항을 각기다른 파일들에 한번에 적용 가능 
3. 하나의 파일을 여러 에디터가 편집 가능 (변경사항 충돌안하고) 
  : '나의 파일과 깃 히스토리를 에디터와 공유하고 있음' 
 -> 어떻게 : 깃허브! -> 클라우드 
-> 4. 여러 대기업의 코드를 오픈소스로 내려받아 볼 수 있음
-> 5. 용량이 큰 소스파일 저장 용이 
프로젝트별로 관리하는게 better


functeion(event) 에서 event의미? 
ex02 _ jquery/ 왜 ready()로 묶어주지 ?
네임이랑 id 차이점?? 
p가 블럭이었나?  ㅇㅇ 
active 는 단순히 클릭한 상태를 의미하는게 아니었나?? 활성화 되었다는 정확한 의미와 상태 
--
days04' ex06??? 
// let txt3= document.querySelector("input[type=text]:last-of-type"); 
let txt3= document.querySelector("input[type=text]:nth-of-type(2)"); 

vs ex06_02 (jquery) -> 얘는 됨!!!!!!!!1

＜ｇｉｔ　＆　ｇｉｔｈｕｂ＞　
：　일단　기본강의로　깃　，　깃허브　시작하기　－＞　이후에　책으로　조금씩　심화개념　채우기　
＋　ｇｉｔｈｕｂ　ｐａｇｅｓ　도　마찬가지　－－＞　일단　강의로　빠르게　시작후　심화개념　채우기　


<git & github 강의> 
팀프로젝트 -> 중요: 버전관리 & 클라우드 저장소
버전관리1등 : git + 클라우드 1등 : github  

ｇｉｔ　：　게임　세이브　－＞　불러오기　포토샵　ｈｉｓｔｏｒｙ　

우리　테니스　계수기　프로그램　짰던걸　생각．．．그　프로젝트　하나하려고　계속　파일　돌려갖고　이름도　다같이　모여서　상의하고　각자　고치고．．．또　그때그때　따로　보내줘야하고．．．이럴필요　없이　그냥　수정본　클라우드에　올려놓으면　각자　다운

ｇｉｔ　사용하는　두가지　방법　
CLI (command line interface - 개발자 하면 생각나는 까만 화면에　그거　（명령을　직접　입력）　
ＧＵＩ　：　게임하듯이，　포토샵처럼　버튼으로　하는거　（ｇｒａｐｈｉｃ）

－＞　클라우드에　업로드　：　ｇｉｔｈｕｂ


＜ｇｉｔｈｕｂ에　업로드　하는　과정＞　
１．　내　컴퓨터　프로젝트　폴더에　여기서 git 을　써서　올릴거다！　라고　명령　
（git 은　프로젝트　단위로　통째로　복사해서　업로드,즉　버전으로　취급　하기　때문에　어떤　파일
，　폴더들을　하나의　프로젝트로　처리할건지　지정해줘야함）
-> git init
２．즐겁게　코딩
３．내가　변경한　파일　중　올리기　원하는　것만　선택
-> git add 
４．선택한　파일들을　한덩어리로　만들고　설명　적어주기　ｅｘ）　메인　페이지　만들기
-> git commit-m "첫페이지 제작" 
５．　ｇｉｔｈｕｂ　사이트에서　프로젝트저장소　만들기 (블로그 만들기랑 동일)
６．내　컴퓨터　프로젝트　폴더에　ｇｉｔｈｕｂ　저장소　주소　알려주기 
-> git remote add 
(내가 미리 git으로 저장할거라고 알려준 프로젝트 폴더들 있지? 그거 여기다 저장할거야)  
７．　내　컴퓨터에　만들었던　덩어리　ｇｉｔｈｕｂ에　올리기　
-> git push 


*오픈소스 : 소스코드를 인터넷등으로 무료로 공유해주는 것 

설치 
git : 다운로드 -> 쭉쭉쭉 윈도우 사용자는 gitbash 설치할건? 하는거에 꼭 체크 -> 디폴트 쭉쭉쭉
github : 계정 생성 및 가입 



1. git init 
: "이 폴더에서 git으로 버전관리를 하고 싶어" 
ㄴ 원하는 폴더에서 git 초기화(새로 저장소 만들기)를 해줘야함 (그 코딩 : git init) 
-> 이거 해주면 그 지정해준 폴더에 .git이라는 투명 폴더 생김
   : 이게 로컬 저장소!! (내가 만든 버전 정보, 원격 저장소 주소 등이 저장) 
 (로컬 저장소 : 내 컴퓨터 안의 git 적용파일 저장하는 공간) 
+) 원격 저장소에서 내 컴퓨터로 코드를 받아오면 로컬 저장소가 자동으로 생긴다 
(원격 저장소 : 내 컴퓨터 밖 클라우드의 git적용파일 저장하는 공간)
※ 한 폴더에 하나의 로컬 저장소만 유지해야한다 ! ex) 바탕화면에 git init 여러개 ~~ 원격에서 받아와도 그대로~~ (충돌) 

※ (이미 파일이 있어도 초기화된 저장소에 자동으로 들어가진 않음) 

1) 저장소로 사용할 폴더 생성  Boxiting-cat 
2) git bash (mac' terminal) 키기 -> 내가 만든 폴더로 이동하기 
- cd : change directory 
- C:\Users\HOME\OneDrive - 한국외국어대학교\바탕 화면\Programming\Git\Boxiting-cat
-> 여기로 디렉토리 이동 안됨 ㅠㅠ (나중에 해결) '리눅스 명령어' 구글에 쳐서 연습 
-> 일단 c:에 위치 이동 후 바로 들어가줌 
$ cd c:
$ cd Boxiting-cat

3) git init으로 로컬 저장소 생성 
$ git init
Initialized empty Git repository in C:/Boxiting-cat/.git/
$ ls         // 모든 폴더 확인 -> 아무것도 안나옴 
$ ls -a     // 숨겨진 폴더까지 확인  -> 마지막에 .git 파일 있는지 확인 
total 20
drwxr-xr-x 1 HOME 197121 0 May  5 18:51 ./
drwxr-xr-x 1 HOME 197121 0 May  5 18:48 ../
drwxr-xr-x 1 HOME 197121 0 May  5 18:51 .git/


2. 버전 만들기 
덩어리  : commit <-> 하나의 버전 
-> git은 파일단위가 아닌 프로젝트 단위로 관리하기 때문에 그 시점에서 여러 파일들을 '뭉쳐서' 하나의 버전(commit)으로 관리 (그때그때 수정된 파일도 있고, 수정안된 파일도 있음) 

user.name / user.email 설정  -> 이 commit을 작성한 사람은 신희민이고 얘 이메일은 이거다~라고 커밋 올리면 확인 가능함 
1) 내가　변경한　파일　중　올리기　원하는　것만　선택-> git add 

VS Code 에서 git 적용폴더 (Boxiting-cat)에 index.html, README.md 파일 생성 
-> 덩어리로 'README.md' 만들어서 저장할거임 

git ad README.md  // 성공시 아무것도 안뜸 

2) 선택한　파일들을　한덩어리로　만들고　설명　적어주기 
ex) 메인페이지 만들기 -> git commit-m "첫페이지 제작" 
git commit -m "프로젝트 설명파일 추가"
*m: message 

$ git commit -m "프로젝트 설명파일 추가"
// 성공시 
[master (root-commit) aad9618] 프로젝트 설명파일 추가
 1 file changed, 0 insertions(+), 0 deletions(-)
// 하나의 파일이 바꼈고, 추가한 코드 : 0개, 삭제한 코드 : 0개
 create mode 100644 README.md

*생성한 커밋 확인 : $git log
commit aad9618ff48b9e5ab2f391fe00a2df5f7b8d15b9 (HEAD -> master)
Author: HeeMin Shin <sinhimin11@naver.com>
Date:   Fri May 5 19:06:42 2023 +0900

    프로젝트 설명파일 추가

커밋 : 무지성 ctrl+s랑 다름 ! '의미있는' 변동사항을 묶어서 만든다 
ex) 버튼 클릭 버그 고치는데 5가지 파일 수정 -> 이 5개를 묶어서 하나의 커밋으로 만듬 
-> 그래야 다른 사람이 수정의 목적 '버튼 클릭 버그 고치기'를 위해 수정한 파일이 얘네들이구나~ 를 알 수 있음 (메세지가 중요한 이유!***) 

커밋은 기차처럼 쌓임
버전관리 <-> 커밋을 만들고 그 커밋을 잘 쌓는것 

3. 내가 만든 버전(commit) 깃허브에 올리기 
로컬 저장소 vs 원격 저장소 
로컬 저장소 : 내 컴퓨터 안에선 버전관리가 완벽히 되고 있음 
원격 저장소 : 다른 사람들과 협업을 하기 위해 내 저장소를 드라이브에 올리는 것! -> push! 

1) gitHub 사이트에서 프로젝트 저장소 만들기  (블로그 만들기랑 동일)
'Create repository' 
↓
Vida0822 / Boxiting
Public
내 계정 / 저장소이름 
상태 

2) 내　컴퓨터　프로젝트　폴더에 github 저장소　주소　알려주기 
-> git remote add 
(내가 미리 git으로 저장할거라고 알려준 프로젝트 폴더들 있지? 그거 여기다 저장할거야)  
git remote add origin https://github.com/Vida0822/Boxiting
-> 아무 에러메시지 안뜨면 성공

3) 만든 커밋 푸시하기 : git push 
(　컴퓨터에　만들었던　덩어리 github에　올리기)
$git push origin master 

HOME@DESKTOP-N9ILIN5 MINGW64 /c/Boxiting-cat (master) // 너의 커밋을 잘 올렸따 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 248 bytes | 248.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Vida0822/Boxiting  // 여기에 
 * [new branch]      master -> master

4) gitHub 사이트에서 올라간 커밋 확인 
 -> 내 홈페이지 새로고침 하면 잘 되어있는거 확인 가능



< 다른사람이 만든 저장소 받아오기 : clone >
다른 사람이 push한 원격 저장소를 그대로 복사해서 받아옴

-> 이때 고양이가 고양3이라는 파일 추가(데이터 변경)해 push ! 문어는 고양1,2 만 있는 상황 
-> 그 업데이트된 데이터는 풀(pull) 명령어로 받아옴
!이때 원격저장소의 주인이 아닌 문어도 고양이의 원격저장소에 push를 할 수 있지만 이러려면 고양이가 문어한테 푸시권한을 줘야함)

1) 원격저장소를 받아올 폴더 준비 : Boxiting-oct
cd로 Boxiting-oct로 이동해 ls -al 확인

2) 원격 저장소 폴더에 받아오기 : $ git clone
HOME@DESKTOP-N9ILIN5 MINGW64 /c/Boxiting-oct
$ git clone https://github.com/Vida0822/Boxiting .
// ※ 여기 띄어쓰기 하고 . 찍어줘야함!! 그래야 '현재 디렉토리에' 라는 의미를 가짐
Cloning into '.'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

$ ls -al
total 20
drwxr-xr-x 1 HOME 197121 0 May  5 19:43 ./
drwxr-xr-x 1 HOME 197121 0 May  5 19:35 ../
drwxr-xr-x 1 HOME 197121 0 May  5 19:43 .git/
-rw-r--r-- 1 HOME 197121 0 May  5 19:43 README.md


3) 다른 계정에서 변경사항 원격저장소에 push
*Collaborater 추가 : Access - Collaborators -> Add a Collaborater 에 권한 줄 이름 입력
gitHub 홈페이지에서 Settings -> 
HOME@DESKTOP-N9ILIN5 MINGW64 /c/Boxiting-oct (master)
$ git add app.js

HOME@DESKTOP-N9ILIN5 MINGW64 /c/Boxiting-oct (master)
$ git commit -m "문어의 커밋"
[master 3b6f071] 문어의 커밋
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 app.js

HOME@DESKTOP-N9ILIN5 MINGW64 /c/Boxiting-oct (master)
$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 272 bytes | 272.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Vida0822/Boxiting
   aad9618..3b6f071  master -> master
 


4) cat 이 문어의 변경 사항 가져오기 : pull 
HOME@DESKTOP-N9ILIN5 MINGW64 /c/Boxiting-cat (master)
$ git pull origin master

remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 0), reused 2 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), 252 bytes | 21.00 KiB/s, done.
From https://github.com/Vida0822/Boxiting
 * branch            master     -> FETCH_HEAD
   aad9618..3b6f071  master     -> origin/master
Updating aad9618..3b6f071
Fast-forward
 app.js | 0
 1 file changed, 0 insertions(+), 0 deletions(-) // 변경사항 : 파일이 하나 생성됨 
 create mode 100644 app.js // 새로 추가된 파일인 app.js 를 가져옴
(궁금! 이때 변경사항만 ㅏ져오는건지 저장소는 있으니까 저장소 말고 데이터 전체를 가져오기 위한 코딩인지) 

*GUI, CLI 둘다 쓸 수 있어야함 (개념 잡을 땐 GUI 가 직관적으로 보기가 쉬움)
-> 일단 GUI로 초반 익숙해지기 + 나중에 더 복잡한 작업할 땐 CLI 


<소스트리 GUI로 깃 다지기> 

1. 커밋 객체에는 대체 머가 저장? 
2. 두사람이 병렬로 커밋을 만들어도 ㄱㅊ,,? 같은곳을 수정한다면?
3. 두사람이 만든 버전 어케 합쳐?
4. 남이 만든 오픈소스에 기여 가능? 


1. GIT GUI인 소스트리로 로컬 저장소 추가 
*GUI : 버튼 클릭으로 Git 명령을 실행할 수 있는 도구 (소스트리 설치) 
-> git 개념을(동작을) 그래프로 가시적으로 볼 수 있어 편리 

1) 소스트리 설치 
https://www.sourcetreeapp.com/

2) 이미 있는 로컬 저장소 추가 


2. 애드 (Add)와 Commint이 이무엇인지 제대로 ! 

git 원리를 알아야 명령이 꼬이지 않게 현명하게 git 사용 가능 
-> 애드 (Add)와 Commint이 이무엇인지 제대로 ! 

변경사항의 모음 x -> 하나의 최종 모드 모음 (기존에 있던 애들도 한번에 사진 찍힘 - 무대에 있으니까) 

이전 SVN : 이전 커밋과의 변경사항만 저장 -> 용량 자체는 git 보다 작을 순 있어도 실제 현재 버전을 보려면 처음의 커밋부터 다 계산을 해야 현재 버전 도출가능 (느림)
vs 
git : 이전 커밋만 보면 됨 (속도 빠름) + 기존 커밋과 비교해 변경된 파일이 아니면 그 파일 자체를 다시 저장하는게 아닌 '변경되지 않았다'고만 저장 

*origin/master : 원격저장소에 있다 ('pusing to origin' ) 
*master : 내 로컬 저장소에 있다 


<나누기 : 브랜치> 
: 평행세계 나누기 

*지금까지는 순차적으로 받아오고 추가 but 동시에 한 커밋된 상태에서 수정한다면? 수정사항이 겹칠 수 밖에 없음  (한줄에서 작업하면 커밋) 
> 여러 줄로 쌓으면 됨 : '브랜치' 
> 실제로 충돌이 발생할 수 있는 부분을 '합칠떄' 명시적으로 해결해줌 
ex) '수많은 브랜치중 단 하나만이 버그없는 미래야...'

git push origin master 
master : 기본 브랜치
-> master 브랜치에 커밋을 푸시해라 
head  : 많은 브랜치들 중 내가 지금 작업하는 로컬 브랜치를 가리킴 (포인터) 

*브랜치 만드는 명령어 

－ git branch cat : cat 브랜치를 만들어라
고양4상태(master 브랜치) 가 head일 때 cat 브랜치 추가 -> 브랜치가 생성됨 

- git checkout cat : 헤드를 옮기는 명령어 (master 브랜치에서 cat 브랜치로)
- 여기서 다시 master브랜치로 돌아가 git branch oct 
-> cat , oct 라는 브랜치가 나누어짐 

보통 브랜치는 새로운 기능을 추가할 때 만듬 ex) 메인페이지 
master에서 브랜치 만드려면 두번째에 마스터 태그 붙어있는 애에서 브랜치 생성 

병렬로, 서로 상관하지 않고, 나만의 브랜치 생성 

<합치기 : 머지(merge)> 
feat 브랜치에서 작업이 끝나 master에서 합치고 싶음 

master 브랜치의 최신 커밋에(base) oct 브랜치의 최신 커밋(compare)을 합치려고 한다 
1. base가 될 master 브랜치로 이동 : 나한테 다시 땡겨와! 들어와 
2. git merge oct 
3. 합쳐진 결과는 문어 a 커밋 (원래 문어 a가 고양4에서 만든거니까) 

feat/mainpage랑 병합하니까 feat/mainpage에 master가 이동 

*컨플릭트 : 합치다가 충돌 

- Fast-forward : 빨리감기됨 (두개를 합쳤더니 하나로 빨리감기 된것처럼 보임)
- Merge commit : 새로운 그림 but 정상적으로 합쳐짐 (새로운 커밋이 생김) 
- Conflict : 두 커밋에서 모자 씀


<나누기 2 : 저장소 통째로 복사 : fork> 
원격저장소를 복제해 내 원격저장소로  
오픈소스에 기여하기 위해선 커밋 전 반드시 컬레버레이터 등록해야해 ? 
ㄴㄴ 굳이 드라이브에 반영하려고 하지 ㅏㄹ고 ㅡ냥 저장소 자체를 가져와 내 깃허브드라이브에 저장하고 거기에 내껄 자유롭게 커밋, 푸시 하면서 맘대로 만지고 다 완성하면 머지해달라고 요청 

브랜치 vs 포크 

원본 저장소의 변경이력을 ㅗ기 위해선 upstream이란 이름으로 원격저장소 경로에 추가(2개가 되는 것) 
-> 원본 저장소에선 가져오기 밖에 안되겠지? 


<내 코드를 머지해줘 : ｆｕｌｌ　request> 

포그한 저장소에서 기능 개발을 마친 너구리 -> 고양 문어 원본저장소에 머짛달라고 하고 싶음 
근데 권한 없자나...

＞　풀　리퀘스트　：　이　커밋이랑　저　커밋을　합치는걸　허락해줘　




[실무사례] 

1. 어맨드 (amend) 

*어맨드 : 깜빡하고 수정못한 파일이 있을 때 방금만든 커밋에 살짝 수정 
방금 커밋으로 모든 수정사항을 하고 싶은데 수정사항 하나때문에 커밋을 아예새로 만들어야하는 상황
=> 방금 만든 커밋에 수정사항 반영하는명령어가 amend

※ 이력 변경하는 명령어는 다른사람과 협업하는 경우 꼬일 수 있음... 왠만하면 혼자 쓰는 브랜치에서 작업 ! 


2. stash 
: 다른 브랜치로 이동해야하는데 현재 작업중인 브랜치의 파일들을 날려야하나? 
(그냥 브랜치 이동하면 Please commit your changes or stash them before you switch branches. 이런 에러뜨면서 못넘어감! )
-> 수정사항을 지우거나 커밋하고 가야함 .... 그냥 나만 가고싶은데!!) 
-> 변경사항을 잠시 킵해두고 커밋은 안만들래요~ : stash (변경사항을 서랍에 넣어주기) 

-> pop : 다시 꺼내오기 (스태시 우클릭) 


3. reset 
: 여러 버전을 올려놓고 옛날 버전으로 되돌리고 싶을때 
(history를 아예 초기화) 

1) hard : 지금까지 작업하던거 다 날리고 이전 버전으로
그냥 push하려하면 안됨 -> 강력push 체크하고 ! (도구에서 허용권한주고) 
2) mixed(default) : 버전을  reset하지만 이전의 내 변경사항은 따로 저장 
-> 리셋시점 이후의 커밋사항들이 'uncomitted changes' 상태로 바껴서 저장되어있음!! 
3) soft : 모든 로컬 변경사항을 유지 


4. revert 
: 내 커밋을 되돌리고 싶을 때 사용 (history를 새로 쌓으면서) 

master에 잘못된 커밋을 올려버렸다. reset하고 force push 하면 다른 사람들한테 영향을 주니 revert해야함 
-> 수정사항이 반영된 커밋을 되돌려줘서 새로은 커밋으로 새로 쌓으면서 이전의 커밋 삭제


5. cherry-pick 
: 여러가지 커밋들중 원하는 것만 데서 지금 브랜치에 붙이는 것 
제가 고친 코드가 있는 커밋을 latest에 똑 떼서 붙일게요~ 
-> 원하는 커밋을 맘대로 똑 떼와서 쌓을 수 있음 
