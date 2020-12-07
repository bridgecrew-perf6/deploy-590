# 구조
/
    L requirements.txt : 특정 환경에서 사용한 모듈들을 기술
                         환경이 구축될때 이 서비스 운영/개발시 사용한 필요한 모듈 설치
                         하기 위해 기술되는 파일이다
                         - 반드시 버전을 명시하여, 향후에 서버가 변경되도, 문제없이 
                           구동되겠음 동일한 환경을 제공
    L run.py :          : 서비스 메인
    L wsgi.py :         : 엔트리 포인트, 아파치서버가 바라보는 파일이다
    L deploy.jason      : 페브릭 배포작업을 하는데 필요한 상수값들을 저장한 파일
                            - 환경변수가 저장된 파일


# faric 설치
- pip (or conda) install fabric (x)
    => python 2.7xx 버전에 맞게 설치가 된다
    => python 3.x 버전 사용 불가

- pip (or conda) install fabric3 (o)

# github 사용
1. github.com 접속후 저장소 생성
2. 로컬 pc에서 git 명령어를 이용하여 적절한 위치 저장소를 다운로드
    - git hub clone https://github.com/kdh9787/deploy.git
    
- 커밋 
    에러 : make sure you configure .....~
    - 조치 : $ git config --global user.name "tjdtlr1020"
              $ git config --global user.email "qkrtjdtlr102@gmail.com"