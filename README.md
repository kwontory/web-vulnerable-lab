# Web Vulnerability Lab

웹 취약점 점검 실습용 환경 (OWASP Juice Shop + DVWA)

## ⚠️ 주의
- 의도적으로 취약한 애플리케이션입니다. 외부에 노출하지 마세요.
- 실습은 반드시 이 로컬 환경에서만 진행합니다.

## 요구사항
- Git, Docker Desktop

## 실행
```bash
git clone https://github.com/<계정명>/web-vulnerable-lab.git
cd web-vulnerable-lab
docker compose up -d
```

## 접속
| 앱 | 주소 | 계정 |
|---|---|---|
| Juice Shop | http://localhost:3000 | 회원가입 후 사용 |
| DVWA | http://localhost:4280 | admin / password |

DVWA 첫 접속 시: Setup 페이지 → "Create / Reset Database" 클릭 → 재로그인

## 종료 / 초기화
```bash
docker compose down       # 종료
docker compose down -v    # 종료 + DVWA DB 초기화
docker compose pull       # 이미지 최신화
```
