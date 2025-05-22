# 프로그래머스 - 웹 프론트 엔드 1일차 과제

**2025.05.22**
로컬에서 프로젝트 생성하여 원격 레포에 올리기

---

## 학습한 내용

- 인터넷의 역사
- 환경 설정
- 깃, 깃허브 프로세스 이해

---

## 복습

- `cmd + shift + p` : 숨겨진 .git 폴더 볼 수 있음
- vscode에서 `cmd + shift + p`: 검색창 나옴
- `cmd + w` : 현재 탭 닫음
- **Git**

  - 소스코드를 효과적으로 관리하기 위한 분산형 버전 관리 시스템
  - 인터넷 연결 없어도 작업과 버전 관리 가능
  - working directory → staging area → (.git)Local repository
  - **cli 명령어**

  ```bash
  git init // 폴더의 버전 초기화
  git branch
  git checkout -b 브랜치명 // 브랜치 생성
  git status //작업 내역 확인
  git add .  //작업 내역 스테이징
  git commit -m "커밋메세지" // 커밋
  git checkout main // 합칠 브랜치로 체크아웃
  git merge 브랜치명 // 나의 브랜치에서 변경된 사항(커밋)을 합침
  git branch -D 브랜치명 //브랜치 삭제
  ```

  - gitignore
    - 깃에 올리고 싶지 않은 파일,폴더를 넣어둠
    - gitignore.io 사이트에서 내가 사용하는 프로그램의 파일,폴더 알 수 있음
  - **HARD vs SOFT**
    - 둘 다 커밋 전으로 돌아감
    - HARD: 이전 커밋 내역 모두 삭제 + 변경된 파일 내역도 삭제
    - SOFT: 이전 커밋 내역 모두 삭제 but 변경된 파일 내역 살림
      ```bash
      git log // 전체 로그 보여줌
      git log --oneline // 로그 한 줄에 보여줌
      git reset --hard 해시값 // 해시값이 있는 커밋으로 이동
      git reset --soft 해시값
      ```

- **GitHub**
  - 깃을 올리는 저장소
  - 인터넷이 연결되야 로컬과 원격 레포 병합 가능
    ```bash
    git push origin main
    ```
