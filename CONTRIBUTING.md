# KPaper 기여
## 환경
1. Unix 기반(Linux, Mac OSX)
    - 윈도우일경우 WSL로 해주세요. Git Bash를 사용할시 오류가 발생합니다. (WSL 부분 참고)
2. 개발 도구 - VIM, IntelliJ IDEA
    - 다른것도 뭐 상관없어요
    
## 기여
### 1. 클론
클론을 해주세요. 이건 알죠?\
`git clone https://github.com/team-alpha-kr/KPaper.git`

### 2. 패치
터미널을 그 Clone이 된 위치로 열어주세요.\
그다음에 업스트림을 패치하세요. 업스트림은 자동으로 가져와져요!\
`./kpaper patch`

### 3. 개발
원하는 IDE에서 개발하세요.

### 4. 패치 적용
`./kpaper rb` 를 입력해 패치를 적용할 수 있습니다.\
그다음에 푸시 또는 Pull Request를 주시면 됩니다!

## 번외: WSL 사용
WSL IDE에서 작업한다면 상관없겠지만 윈도우에 있는 IDE를 사용하려면 리눅스의 `~/.m2`와 윈도우의 `C:\Users\유저이름\.m2`를 연결해야됩니다.\
[심볼릭 링크를 사용해 연결하기](https://stackoverflow.com/questions/56764503/windows-10-wsl-maven-config)
### 속도가 너무 느려요!
클론할때 `/mnt` 디렉터리(또는 그 하위)를 사용하지 마세요. 성능 이슈가 있습니다.\
WSL ~/ 디렉터리에서 클론하고 작업하세요.\
윈도우에 있는 IDE에 프로젝트를 불러오려면 [WSL 디렉터리를 윈도우로 마운트하세요](https://www.howtogeek.com/426749/how-to-access-your-linux-wsl-files-in-windows-10/)