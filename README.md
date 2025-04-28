# gitx

#설치 방법

```
git clone https://github.com/pegasuskim/gitx.git
```

터미널에서 실행 권한을 부여합니다:

```
chmod +x gitx
```

원하는 프로젝트 디렉토리에 이 파일을 위치시키거나, PATH에 추가하여 어디서든 사용할 수 있게 합니다.

#사용 방법
###전체 워크플로우 (add + commit + push)

코드 변경 후 한 번에 스테이징, 커밋, 푸시를 진행할 때:
```
./gitx "[prefix] : 커밋 메시지"
```
예시:
```
./gitx "feature : 로그인 기능 추가"
```

```
./gitx "bug-fix : 사용자 프로필 오류 수정"
```

```
./gitx "docs : README 업데이트"
```



여기서 [prefix] 는 당신이 언급한 대로 커밋의 성격을 나타내는 태그입니다. 

아래와 같은 접두어를 사용할 수 있습니다:

- feature 또는 feat: 새로운 기능 추가

- bug-fix 또는 fix: 버그 수정

- docs: 문서 수정

- api: API 관련 변경사항

- testcase 또는 test: 테스트 관련 변경

- refactor: 코드 리팩토링 등등

### 커밋만 수행

변경사항 스테이징 및 커밋만 하고 싶을 때:

```
./gitx commit "feature : 사용자 인증 기능 추가"
```

### 푸시만 수행
이미 커밋된 변경사항을 현재 브랜치에서 원격으로 푸시:

```
./gitx push
```

### 로컬 변경사항 버리기

작업 중인 변경사항을 모두 취소하고 싶을 때:

```
./gitx discard
(이 명령은 위험하므로 실행 전 확인 메시지가 나타납니다)
```

### 현재 브랜치 main으로 병합하기

작업 브랜치를 main 브랜치로 병합:

```
./gitx merge
```

### 원격 저장소 정보 가져오기

모든 원격 저장소의 최신 정보 가져오기:

```
./gitx fetch
```
