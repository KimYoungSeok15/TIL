### 마크다운이란?

* 제목
  '#','##'등으로 크기 조절


* 리스트
*  순서 X -> *or-


* 코드블록
  *문장 한 가운데에서 'print('pppp')
  *'''
  문장 한 가운데에서 'print('pppp')
   '''
* URL & image
  * string
  * [제목] (URL)
* 테이블
  |제목|제목2|제목3|

>인용
GIT의 기초
| 분산 버전 관리 프로그램
| | 하나의 중앙집중식 관리가 아닌 서버 그리고 개발자 개인의 PC에도 버전이 동시에 관리가 되어서, 리소르를 분산으로 관리하는 것.
1. 백업
2. 복구
3. 협업

Git 문법
1. 깃 시작하기
  1.초기화 : 'git init' : git local repository 초기화
    1. 로컬 레포지토리 생성 후 버전으로 관리할 파일을 git add로 단 한번이라도 staging area에 옮겨줘야한다.
       Why? git init해도, git는 어떤 파일을 관리해야하는지 모른다.
    2. 파일의 상태
       1.최초 생성 시 : untracked
       2 git add 후 : staged
       3. git commit : tracked
       4. 
    1. .git 이 있는 repository를 만든다. touch a.txt를 하고 git status를 하면 상태값이 나온다.
  2.'git add' : staging area로 버전관리 할 파일 옮기기
    1. git add . : 현재 위치한 w.d(workking directory)에 생긴 모든 변화 사항을 stage
    2. git add {file name}: file 을 지정해서 stage
  3. git commit -m '커밋메시지' 
    1. 커밋 메세지는 해당 버전이 어떤 목적에서 생성됐는지.
      1. 길이의 제한 O
**여기까지가 local repository의 일들.**
----------------------------------------------------------------------------------
## Remote Repository(원격 레포지토리 / 깃허브)
* 레포지토리 연결하기 : 'git remote add origin remote_repo Url'
* git push origin master : local -> remote로 (upload)
  * 인증 : remote repository에 push를 할 권한이 있는지 확인
* add -> commit -> push
