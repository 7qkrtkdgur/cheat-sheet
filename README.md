## 환경 설정
- $ git config --global user.name "[name]" - 자신이 생성한 커밋(commit)에 들어갈 이름을 설정.
- $ git config --global user.email "[email address]" - 자신이 생성한 커밋에 들어갈 이메일 주소를 설정합니다

## 저장소 생성하기
- $ git init [project-name] - 새로운 로컬 저장소를 생성하고 이름을 정합니다.
- $ git clone [url] - 기존 프로젝트의 모든 커밋 가져와 저장소 생성

## 변경점을 저장하기
- $ git status – 커밋할 수 있는 새로운 파일과 수정된 파일 목록 보여줌.
- $ git diff – 수정하였으나 아직 stage하지 않은 파일의 변경점 보여줌.
- $ git add [file] - 커밋을 준비하기 위해 파일 stage합니다.
- $ git diff —staged – stage하였으나 아직 커밋하지 않은 파일과 최근 커밋한 파일 비교.
- $ git reset [file] - 파일의 내용은 유지한 채로 stage한 내역만 제거.
- $ git commit –m“[descriptive message]” - stage한 내용을 커밋으로 영구 저장.

## 변경점을 묶어 관리하기
- $ git branch – 현재 저장소의 모든 로컬 브랜치를 보여줍니다.
- $ git branch [branch name] - 새로운 브랜치 생성.
- $ git checkout [branch name] - 특정 브랜치로 전환하고 워킹 디렉토리 업데이트.
- $ git merge [branch name] - 현재 브랜치에 특정 브랜치의 히스토리를 병합.
- $ git branch –d [branch name] 브랜치를 삭제.

## 파일 이름 바꾸기
- $ git rm [file] - 워킹 디렉토리에 있는 파일을 제거하고 삭제한 내역을 stage합니다.
- $ git rm —cached [file] - 현재 파일은 그대로 두고 버전 관리 체계에서만 제거.

## 변경점 일부분을 저장하기
- $ git stash – 버전 관리 중인 모든 파일의 변경점을 임시로 저장.
- $ git stash list – 임시 저장된 모든 변경점의 목록 보여줌.
- $ git stash drop – 가장 최근에 임시 저장한 내용을 지웁니다.

## 변경 기록 검토
- $ git log – 현재 브랜치의 변경 기록을 보여줌.
- $ git log —follow [file] - 특정 파일의 변경 기록을 보여줌.

## 커밋 되돌리기
- $ git reset [commit] - [commit] 이후 모든 커밋 내용 되돌림.
- $ git reset —hard [commit] - 모든 변경점과 기록 버리고 특정 커밋으로 돌아감.

## 변경점을 동기화하기
- $ git fetch [remote] - 원격 저장소로부터 모든 기록을 받아옵니다
- $ git merge [remote]/[branch] - 원격 브랜치를 현재 사용 중인 로컬 브랜치와 병합.
- $ git push [remote] [branch] - 모든 로컬 브랜치의 변경점을 Github에 업로드 함.
- $ git pull – 북마크된 원격 브랜치의 기록을 다운로드하여 변경점 병합.
