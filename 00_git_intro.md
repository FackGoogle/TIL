### GIT 초기 설정 

커밋의 작성자 설정 

```bash
$ git config --global user.email "메일 주소"
$ git config --global user.name "유저 네임"
```

- 커밋을 작성해야하기때문 

<br>

커밋 편집기 변경

```bash
$ git config --global core.editor "code --wait"

```

- vs코드가 설치 되어있아야 함 

> 기본 텍스트 편집기를 vim을 vscode로 대체 하는것

---

### Git basic 

### 로컬 저장소 설정 



```bash
git init
Initialized empty Git repository in C:/Users/김두진/Desktop/TIL/.git/(master)
```

- 폴더에 git 저장소를 초기화하면 
  - git 숨김파일 폴더가 생기고 
  - bash에는 (master)라고 표기 된다 .

> 주의사항 
>
> - git저장소 내에 또다른 git 저장소를 만들면 안됨
> - git init 명령어 입력할때 (master)가있으면 절대 사용하지 말것 

<br>

### add

> staging area/INDEX

```bash
$ git add 파일명 
$ git add .#현재 디렉토리(하위디렉토리) 
$ git add a.txt #특정파일 
$ git add my_folder/#특정 폴더
```

- working directory 산태의 파일을 staging area 상태로 변경
- 커밋을 위한 파일 및 폴더들을 추가하는 명령어 

```bash
$git status
no branch master
```

>모든 정보는 git status에 있다 .





<br>

### commit 

```bash
$ git commit - m "first commit"
```

- 커밋을 통해 하나의 버전으로 기로됨 
- 커밋 메세지는 현재 변경사항들을 잘나타 낼수 있도록 작성하는것을 권장 
- 커밋은 고유한 아이디인 해시 값을 가짐 
  - SHA-1 알고리즘에 의해 생성
- 커밋 목록은 git log 를 톨해 확인 할수 있음 

```bash
git log --oneline #커밋 목록 한줄로 보기
```

