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

## 주요 엔드포인트
- `POST /api/auth/register` 요청 본문: `{ email, password, name }`
- `POST /api/auth/login` 요청 본문: `{ email, password }` → 응답: `{ token }`

보호된 엔드포인트 호출 시, 로그인 응답의 토큰을 헤더에 포함하세요:
`Authorization: Bearer <token>`

## 비고
- 원본 프로젝트와 형제 경로로 사용하려면, 이 폴더를 `../CVEExampleBackend`로 이동해 사용하실 수 있습니다.
