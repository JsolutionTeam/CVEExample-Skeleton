# CVEExampleBackend
인증 기능(auth)만 담은 최소한의 Spring Boot (3.x) 예시 프로젝트입니다.

## 기술 스택
- Spring Boot Web, Security, JPA
- H2(메모리 DB)
- JWT(jjwt)

## 실행 방법
```
./gradlew bootRun
```

애플리케이션은 포트 `:8081`에서 기동됩니다. H2 콘솔은 `/h2-console`에서 확인할 수 있습니다.