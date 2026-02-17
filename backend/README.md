# Invest Asset Manager - Backend Dev Environment Setup

## 1. Overview

이 문서는 Invest Asset Manager Backend 개발을 위한 Python 환경 구성 절차를 정리한다.

- Python: 3.12
- Conda Environment: invest-api
- Database: PostgreSQL 17.2 (Docker 기반)
- Backend Framework: FastAPI

---

## 2. Conda Environment 생성

### 2.1 환경 생성

```bash
conda create -n invest-api python=3.12 -y
```

### 2.2 환경 활성화

```bash
conda activate invest-api
```

## 3. Backend 디렉토리 이동

프로젝트 루트 기준:

```bash
cd invest-asset-mgr/backend
```

requirements.txt는 반드시 backend 폴더 기준으로 생성함.
