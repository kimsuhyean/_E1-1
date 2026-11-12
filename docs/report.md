# 개발 작업실 구축 기술문서

## 1. 프로젝트 개요
- 미션 목표: Windows PowerShell 기반 작업실에서 Git, GitHub, VS Code, Docker를 사용해 개발 환경을 구성하고 웹 페이지를 실행·검증하는 것이다.
- 작업 목적: 로컬 작업 폴더와 GitHub 저장소를 연결하고, Docker 컨테이너를 통해 웹 페이지를 실행하는 기본 개발 흐름을 익히기 위함이다.
본 작업을 통하여 로컬 작업 폴더를 생성하고, Git 저장소를 설정한 뒤, VS Code를 이용해 프로젝트 파일을 작성하고 GitHub에 반영하는 과정을 실습하였다.

## 2. 실행 환경
- OS: Windows
- Shell / Terminal: PowerShell
- Editor: VS Code
- Git 버전: git version 2.56.0.windows.4
- Docker 버전: Docker version 29.9.2, build a82e528
- 작업 폴더 경로: C:\작업실\_E1-1

## 3. 수행 항목 체크리스트
- [x] PowerShell 실행 및 기본 명령 확인
- [x] Git 저장소 초기화 또는 clone
- [x] main 브랜치 확인
- [x] GitHub 원격 저장소 연결
- [x] VS Code에서 프로젝트 열기
- [x] `web/index.html` 생성
- [x] Docker 컨테이너 실행
- [x] 포트 매핑 확인
- [x] 브라우저에서 localhost 접속 확인
- [x] 바인드 마운트 확인
- [x] Git status 확인
- [x] Git add / commit / push 수행

## 4. 수행 내용
### 4-1. 저장소 및 작업 폴더 준비
- 수행한 작업:
- 사용한 명령:
- 확인 결과:

### 4-2. VS Code 및 웹 파일 준비
- 수행한 작업:
- 사용한 명령 또는 방법:
- 확인 결과:

### 4-3. Docker 실행 및 웹 서비스 확인
- 수행한 작업:
- 사용한 명령:
- 확인 결과:

### 4-4. Git 및 GitHub 반영
- 수행한 작업:
- 사용한 명령:
- 확인 결과:

## 5. 검증 방법 및 결과 위치
### 5-1. Git 상태 확인
- 확인 명령:
- 정상 기준:
- 실제 결과:

### 5-2. Docker 실행 확인
- 확인 명령:
- 정상 기준:
- 실제 결과:

### 5-3. 웹 페이지 접속 확인
- 확인 방법:
- 정상 기준:
- 실제 결과:

### 5-4. 결과 위치
- GitHub 저장소:
- 기술문서 파일 경로:
- 웹 파일 경로:

## 6. 트러블슈팅
### 사례 1
- 문제:
- 원인 가설:
- 확인 방법:
- 해결 방법:
- 결과:

### 사례 2
- 문제:
- 원인 가설:
- 확인 방법:
- 해결 방법:
- 결과:

## 7. 최종 결과 요약
- 완료한 항목:
- 확인된 동작:
- 현재 저장소 상태:
- 다음 작업:

### Docker nginx 포트 매핑 실행

실행 명령:
```powershell
docker run -d --name my-nginx -p 8080:80 --mount type=bind,source="${PWD}\web",target=/usr/share/nginx/html,readonly nginx
