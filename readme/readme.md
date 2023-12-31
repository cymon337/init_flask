# 플라스크 환경 구축하기

## 가상환경 설치

```bash
# 가상환경 설치
python3 -m venv venv
# 가상환경 실행
source venv/bin/activate
# 가상환경 비활성
deactivate
```

## 플라스크 설치

작업 디렉터리 flaskbook 에 venv 설치 후 activate

```bash(venv)
pip install flask
```

### flask 기본 패키지

- click 
    명령어 라인용 프레임워크. 플라스크의 커스텀 명령어를 사용한다. 
- itsdangerous 
    안전하게 위해서 사용한다. HMAC(Hash-based Message Authentication Code)을 사용하여 데이터에 서명을 추가.
    데이터를 직렬화하여 문자열로 변환합니다. 이 문자열은 서명과 함께 저장됩니다.추후에 다시 역직렬화하여 사용.
    플라스크의 세션이나 쿠키(Cookie)를 보호하기 Jinja2 디폴트 HTML 템플릿 엔진. 다른 템플릿 엔진을 사용할 수도 있다. 
- MarkupSafe 
    인젝션 공격을 회피하기 위해 템플릿을 렌더링할 때에 신뢰할 수 없는 입력을 취소한다. 
- Werkzeug 
    WSGI 툴킷으로 플라스크의 코어 구현은 Werkzeug(werkzeug.palletsprojects.com)를 바탕으로 만들어져 있다.


