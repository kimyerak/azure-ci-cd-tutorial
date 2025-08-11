## Azure CI/CD Tutorial

간단한 Nginx 데모 이미지를 기반으로 정적 페이지(`index.html`)를 교체하여 Azure CI/CD 실습에 활용하는 예제입니다.

### 구성
- **베이스 이미지**: `nginxdemos/hello`
- **커스터마이즈**: `index.html`을 복사해 기본 페이지 대체
- **Dockerfile**: 빌드 시 정적 페이지를 이미지에 포함

### 빠른 시작
1) 로컬 빌드
```
docker build -t your-registry/azure-ci-cd-tutorial:local .
```
2) 실행
```
docker run --rm -p 8080:80 your-registry/azure-ci-cd-tutorial:local
```
브라우저에서 http://localhost:8080 으로 접속해 페이지를 확인하세요.


