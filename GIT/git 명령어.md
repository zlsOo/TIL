## GIT 명령어
  
##### GIT 설치법
```
1. 터미널(ctrl+alt+t)
2. sudo apt install git 입력 (=> 설치완료)
3. git --version 입력 (=> 설치 확인 및 버전 확인)
```

##### 새로운 저장소 생성
` $ git init `

```
.git하위 디렉토리 생성 (폴더를 만든 후 그 안에서 명령 실행-> 새로운 git 저장소 생성)
```
##### 저장소 복제/다운로드(clone)
`1.$ git clone <https:.. URL>`
`2.$ git clone /로컬/저장소/경로`
`3.$ git clone 사용자명@호스트:/원격/저장소/경로`

```
1.기존 소스 코드 다운로드/복제
2.로컬 저장소 복제
3.원격 서버 저장소 복제
```
##### 가지(branch)치기 작업
`1.$ git branch`
`2.$ git branch <브랜치이름>`
`3.$ git checkout -b <브랜치이름>`
`4.$ git checkout master`
`5.$ git branch -d <브랜치이름>`
`6.$ git push origin <브랜치이름>`
`7.$ git push -u < remote > <브랜치이름>`
`8.$ git pull < remote > <브랜치이름>`
```
1.브랜치 목록
2.새 브랜치 생성 (local로 만듦)
3.브랜치 생성 & 이동
4.master branch로 되돌아 옴
5.브랜치 삭제
6.만든 브랜치를 원격 서버에 전송
7.새 브랜치를 원격 저장소로 push
8.원격에 저장된 git 프로젝트의 현재 상태를 다운받고 + 현재 위치한 브랜치로 병합
```
##### <변경 사항 발행(push)>
`1.$ git push origin master`
`2.$ git push < remote > <브랜치이름>`
`3.$ git push -u < remote > <브랜치이름>`
`4.$ git remote add origin <등록된 원격 서버 주소>`
`5.$ git remote remove <등록된 클라우드 주소>`
```
1.변경사항 원격 서버에 업로드
2.커밋을 원격 서버에 업로드
3.커밋을 원격 서버에 업로드
4.클라우드 주소 등록 및 발행
(git에게 새로운 원격 서버 주소 알림)
5.클라우드 주소 삭제
```
##### <갱신 및 병합(merge)>
`1.$ git pull`
`2.$ git merge <다른 브랜치이름>	`
`3.$ git add <파일명>`
`4.$ git diff <브랜치이름><다른 브랜치이름>`
```
1.원격 저장소의 변경 내용이 현재 디렉토리에 가져와지고(fetch) 병합(merge)됨
2.현재 브랜치.에 다른 브랜치의 수정사항 병합
3.각 파일을 병합할 수 있음
4.변경 내용 merge 전에 바뀐 내용을 비교할 수 있음
```
##### <태그tag 작업>
`$ git log`
```
현재 위치한 브랜치 커밋 내용 확인 및 식별자 부여됨
```
##### <로컬 변경사항 return 작업>
`1.$ git checkout -- <파일명>`
`2.$ git fetch origin`
```
1.로컬의 변경 사항을 변경 전으로 되돌림
2.원격에 저장된 git프로젝트의 현 상태를 다운로드
```

## CLI (Command Line Interface) 명령어

* 명령어 인터페이스는 (마우스나 각종 UI 컴포넌트 대신) 터미널을 통해 사용자와 컴퓨터가 상호 작용하는 방식

##### <관리자 권한으로 실행>
`	$ sudo`
```
의미: super user do
1. 관리자만 읽을 수 있는 파일 읽기
2. 새로운 프로그램 설치 (Ubuntu Linux)
3. Notes : 새로운 프로그램 설치시 Package Manager를 이용하는 것이 보편적
```
##### <기본적인 unix/linux 명령어>
`$ ls`
```
의미: list
파일보기
```

`$ al`
```
의미: all
파일의 세부내용 확인
< $ ls -al의 상세 내용 (권한) >
1. 접근권한 (읽기/쓰기/실행 가능)여부
2. 링크된 파일 갯수
3. 소유자
4. 소유 그룹
5. 파일 크기
6. 만든 날짜
7. 만든 시간
8. 파일/디렉토리 이름
```
`$ cd `
```
의미: change directory
디렉토리로 이동
```
`$pwd`
```
의미: print working directory
full 디렉토리 path 확인 /
(디렉토리 위치 변경)
```
##### 디렉토리로 이동
`1.$ cd ~`
`2.$ cd /`
`3.$ cd .`
`4.$ cd ..`
`5.$ pwd`
`6.$ clear`
```
1.홈 디렉토리 (현재 사용자 개인 파일 디렉토리)
2.루트 디렉토리 (시스템 최상위 디렉토리 확인) /
(매우 중요한 디렉토리를 의미하며 관리자 권한 요구함)
3.현재 디렉토리
4.부모 디렉토리
5.현재 full 디렉토리 확인
6.터미널의 입력 내용들을 지워줌
```

##### 자주쓰는 명령어
`$ touch [file_name]`
```
빈 파일 생성 / (not 디렉토리 / literally 파일을 생성)
```
`$ mkdir [dir_name]`
```
의미:make directory
디렉토리 생성
```
`$ cat [file_name]`
```
의미:concatenate
텍스트 형태의 파일 확인
```
`$ mv [file_name or dic_name][target_dir_name]`
```
의미:move
파일 또는 디렉토리 옮기기
```
`$ mv [file_name or dir_name][new_file_name]`
```
파일 및 디렉토리 이름 바꾸기
```
`$ cp [file][target_dir_name]`
```
의미:copy
복사
```
`$ cp -r [folder_name]`
```
복사
```
#### 삭제 (휴지통을 거치지 않고 즉시 삭제)

`$ rm [file_name]`
```
의미:remove
파일 삭제
```
`$ rm -r [dir_name]`
```
폴더 삭제
```
#### 파일 소유권 변경
`$ chown [owner_file]:[group_file]`
```
의미:change owner
파일 소유권 변경
```
`$ mkdir`
```
디렉토리 생성
```
`$ rm`
```
삭제
```
#### GUI프로그램의 실행을 더 간편하게

`1.$ explorer .`
`2.$ open .`
`3.$ code .`
```
1.현재 폴더를 windows파일 관리자에서 보기
2.현재 폴더를 macOS finder에서 보기
3.현재 폴더를 VS Code 에디터로 열기
```

#### 파일 이름에 따른 팁
`1.공백이 있는 경우`
`2.파일 자동완성 기능`
```
1.공백부분에 tab 키를 누르기 or / (역슬래시)를 입력
2.첫글자 등을 쓰고 tab 키 누르기
```

#### branch에 기존 작업코드 복사하고 push하기
```
branch 생성 후 이동:git checkout -b expressPrac
확인:git status
push 하기:git push origin expressPrac
```