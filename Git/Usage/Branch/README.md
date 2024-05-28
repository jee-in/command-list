## 브랜치 관리

### 현재 위치한 브랜치 확인
```Shell
git branch
```

### 브랜치 생성
```Shell
git branch {생성하려는 브랜치의 이름}

#예시: git branch test
```

### 브랜치 이동
- 구 버전 명령어
```Shell
git checkout {이동하려는 브랜치의 이름}

#예시: git checkout test
```
- 신 버전 명령어
```Shell
git switch {이동하려는 브랜치의 이름}

#예시: git switch test
```

## 업로드와 다운로드

### 로컬 저장소의 변경 사항을 원격 저장소에 업로드
```Shell
git push {원격 저장소의 이름 또는 주소} {브랜치의 이름}

#예시: git push origin test
```

### 원격 저장소의 변경 사항을 로컬 저장소에 업데이트
```Shell
git fetch {원격 저장소의 이름 또는 주소} {브랜치의 이름}

#예시: git fetch origin test
```
- fetch는 마지막 pull 이후 원격 저장소에 생긴 변경 사항을 다운로드합니다.
- fetch를 수행한 결과 원격 저장소에서 변경 사항이 발견되었다면 merge나 rebase를 수행하여 로컬 저장소에 이를 업데이트해야 합니다.

### 원격 저장소의 변경 사항을 로컬 저장소에 업데이트 + 병합
```Shell
git pull {원격 저장소의 이름 또는 주소} {브랜치의 이름}

#예시: git pull origin test
```
- git pull은 원격 저장소에 생긴 변경 사항을 다운로드하고 이를 로컬 저장소에 바로 병합합니다.
- 일반적으로 pull로 인해 로컬 저장소에서 작업 중인 내용이 날아가는 것을 방지하기 위하여 pull을 수행하기 전에 fetch를 먼저 수행합니다. 

## 충돌 관리

### 로컬 저장소에서 다른 브랜치를 현 브랜치로 병합
```Shell
git merge {현 브랜치에 병합하려는 브랜치의 이름}

#예시: git merge main
```
- merge를 수행한 후, push까지 수행해야 원격 저장소에도 병합이 이루어집니다.