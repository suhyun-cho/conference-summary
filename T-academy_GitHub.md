
## Git과 Github-Page블로그 만들기
SK T-academy 65차 <br>
date : 2019-12-12


## Github 실습하기
* 버전 저장은 .git 폴더에 저장됨
* 저장이 싫다면 .gitignore파일에 작성
* README.md 작성 팁
    * 프로젝트 내용 (이미지/로고)
    * 설치 방법
    * 코드 예제
    * 개발 환경 설정 방법
    * 기여방법
    * 로그 변경
    * 크레딧
        * 코드수정 및 오타수정에 도와준 사람 작성
    * 라이센스
        * 내가 했다는 것에 대한 증명
    * 연락처

#### [파일 스테이지로 올리기]
* git add [file] 
    * [file]을 스테이지로 올림, 폴더나 전체도 가능
* git status , git diff
    * 어떤 파일을 수정했고, 스테이징 했는지, 어떤 파일이 얼마나 바뀌었는지 확인
* git commit -m "add README.md"
    * 간단한 설명과 함께 commit (version upgrade)
* git log
    * 이전 commit 기록 살펴보기
* git remote add origin [url]
    * origin이라는 이름으로 [url]과 연결
    * 내 공간과 원격 공간을 연결 
* git push origin master
    * 원격 저장소로 올리기 (내가보는 버전과 모두가 보는 버전이 동기화 완료)


---------------
# cmd창에서 git 사용법
### basic

* clear : 초기화
* cd : change directory
* mkdir : make directory
* ls : list (폴더안에 있는 파일들을 보여줌)
* touch [file]: 빈 파일을 만들어줌
* code .
    * vs code 화면 켜짐
* cat README.md
    * 내가 작성한 내용이 cmd창에 보여짐
* ls -al
    * 숨긴폴더 보여줌
    * .git 폴더 건드리면안됨..
* git init
* git status
    * 현재 git 의 상태
* git add README.md
    * 추적이 된다는 의미, 하고나서 다시 git status 하면 빨간색이 초록색으로 변함
    * commit할 준비가되었다는 뜻
* git config --global user.name="suhyuncho"
    * git 설정을 내 모든 컴퓨터에 저장
* git config --global user.email="whtngus4759@gamil.com"
* git log
* git diff 
    * 파일 수정내용을 보여줌
* git add .
    * 현재 내가있는 모든 폴더를 올리겠다.
* git remote -v
    * 연결이 되었는지 확인
    


### high-version
* git clone [url] 
    * 원격 저장소에서 다운로드
* git branch [name]
    * 필요한 기능은 병렬적으로 개발. 완성되기 전까지는 기능별로 따로 관리
* git checkout [name]
    * [name] branch 로이동
* git merge [name]
    * [name] branch를 현재 branch로 합친다
* git rebase master 
    * base를 master로 re-base한다
* git branch -d [name]
    * 완료된 branch를 지운다.
    

### high-high-version
* git fetch
    * 원격 저장소와 동기화
    * 협업을 할 때는 fetch 사용
* git pull
    * 원격 저장소와 동기화하고 merge
    * 혼자 작업할 경우는 그냥 pull
* git reset [option] [branch]
    * branch 이후 기록을 없애자
* git revert [branch] 
    * 수정한 기록도 남기자
* git stash
    * 현재 작업하고 있는 작업물을 따로 저장하기
    

----------------
# github blog

#### [ 참고 사이트 ]
git blog Theme site 
> http://jekyllthemes.org <br>

수업시간에 활용한 Theme 주소<br>
> https://github.com/mmistakes/minimal-mistakes/ <br>
> https://github.com/RyanFitzgerald/devportfolio <br>

GitHub로 취업하기 <br>
> https://sujinlee.me/professional-github/

개발자의 이력서 만들기 <br>
> http://woowabros.github.io/experience/2017/07/17/resume.html

### [ blog Theme과 내 git 주소 연결하는 방법 ]
* mkdir blog_blog
    * 폴더만들기
* git clone https://github.com/RyanFitzgerald/devportfolio.git
    * 인기 Theme 인 minimal mistake 를 clone
* sudo rm -r .git
    * devportfolio 폴더에 들어가서 .git 파일을 제거
* git init
* git remote add origin https://github.com/whtngus4759/github_blog.git
    * 내 깃허브 Repository 연결
* git remote -v
    * 블로그가 제대로 되었는지 확인가능
* git add . 
    * stage에 전부 올리겠다
* git commit -m "blog start"
* git push origin master
-----------
* config 파일 수정
* posts가 글 올리는 부분


```python

```
