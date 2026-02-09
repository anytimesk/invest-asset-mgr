# Infra 구성 안내

- 작성일: 2026-02-10

이 폴더는 보유 중인 주식의 종목과 수량 정보를 기반으로 수익률을 확인하는 프로그램의  
로컬 개발 및 실행에 필요한 인프라 구성을 정의합니다.  
Docker Compose를 사용하여 PostgreSQL을 실행하며, Git clone 이후 동일한 개발 환경을 재현할 수 있도록 구성합니다.

---

## 구성 요소

현재 포함된 구성:

- PostgreSQL (Docker 컨테이너 기반 실행)
- docker-compose.yml (PostgreSQL 컨테이너 실행 설정)

향후 확장 예정:

- Backend 컨테이너
- Frontend 컨테이너
- 운영용 compose 분리(dev / prod)

---

## PostgreSQL 실행

PostgreSQL은 docker-compose.yml을 통해 Docker 컨테이너로 실행됩니다.

### 실행

```bash
docker compose up -d