# n8n 환경 설정 가이드

이 문서는 n8n 워크플로우 자동화 도구의 환경 설정에 대한 안내입니다.

## 환경 설정 가이드
이 프로젝트를 실행하기 위해서는 `.env` 파일에 다음 설정을 추가해야 합니다.
### 필수 환경 변수
아래의 설정을 `.env` 파일에 복사하여 붙여넣으세요:
``` ini
GENERIC_TIMEZONE=Asia/Seoul
TZ=Asia/Seoul

WEBHOOK_TUNNEL_URL=https://n8n.example.com
DOMAIN_NAME=example.com
SUBDOMAIN=n8n

N8N_BASIC_AUTH_ACTIVE=true
N8N_BASIC_AUTH_USER=yourusername
N8N_BASIC_AUTH_PASSWORD=yourpassword
```
### 설정 설명
- `GENERIC_TIMEZONE`, `TZ`: 시스템의 시간대를 서울로 설정합니다.
- `WEBHOOK_TUNNEL_URL`: 웹훅 터널 URL 주소입니다.
- `DOMAIN_NAME`, `SUBDOMAIN`: 도메인 관련 설정입니다.
- `N8N_BASIC_AUTH_ACTIVE`: 기본 인증 활성화 여부입니다.
- `N8N_BASIC_AUTH_USER`, `N8N_BASIC_AUTH_PASSWORD`: 기본 인증 시 사용할 사용자 이름과 비밀번호입니다.

실제 사용 시에는 `yourusername`과 `yourpassword`를 안전한 값으로 변경하세요.
