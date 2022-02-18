# 깃 허브 명령어 정리

### Branch Remote Local 기본 과정

---

- git init (현재 디렉토리에 git 적용)
- git add README.md (readme 추가)
- git commit -m "" (하나의 버전을 히스토리에 저장)
- git status (현재 local 적용상태 확인)
- git push (local을 remote로 저장)
- git pull (remote를 local로 저장)

### Branch 명령어 ( Local Repository )

---

- git branch (로컬 브랜치 목록 조회)
- git branch -r (원격 브랜치 목록 조회)
- git branch -a (모든 브랜치 목록 조회)

- git branch {브랜치명} ( local 브랜치 생성)
- git checkout -b {브랜치명} (명령어를 통해 신규 브랜치 생성과 동시에 체크아웃)
- git checkout {브랜치명} (브랜치 변경)
- git branch -d {브랜치명} ( 브랜치 삭제 )

### 원격 저장소( remote repository )

---

- git push origin -u <new_name_branch> (Remote Branch(원격 브랜치) 이름 변경 방법)
- git remote -v (현재 연결되어 있는 원격 레파지토리를 확인)
- git remote add <name> <url> (원격저장소와 연결하고 싶으실 경우엔)

- git clone [저장소 주소] ( 저장소 복제 )
- git fetch (remote를 local로 저장, 직접 비교대조 후에 수동 merge)
- git pull (remote를 local로 저장, 자동 merge)
