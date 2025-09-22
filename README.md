# DjangoPractice
회원가입과 게시판 만들어보기

Python 설치는 기존에 학교 강의를 수강하면서 완료했었다.

<img width="394" height="90" alt="image" src="https://github.com/user-attachments/assets/839cbb08-6c1d-4096-a39e-fdcc9ab9a470" />


Django 프로젝트 폴더 생성 및 가상 환경 설정

가상 환경이란.
파이썬 프로젝트의 독립적인 실행 공간이다. 

# 1. 가상환경 생성
python -m venv venv

# 2. 가상환경 활성화 (윈도우)
venv\Scripts\activate

<img width="383" height="38" alt="image" src="https://github.com/user-attachments/assets/90f96541-3cfd-4a15-843c-dc810b7840fd" />

위 화면처럼 프롬프트 앞에 (.venv)라고 표시되면 가상 환경이 성공적으로 활성화된 것이다.

# 3. 가상환경에서 Django 설치
pip install django

# 4. Django 프로젝트 생성
django-admin startproject [프로젝트이름] [설치경로]

여기까지 아무런 문제 없이 진행이 됐을 경우
C:\workspace\my_django_project\config
이 경로에 settings.py 파일이 생성되어 있을 것이다.

해당 파일을 열어
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'accounts', 
    'posts', 
]
을 붙여 넣고,
데이터베이스 설정을 
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': '내가 생성한 DB명',
        'USER': 'postgres',   
        'PASSWORD': 'postgre설치시에 설정한 비밀번호',    
        'HOST': 'localhost',
        'PORT': '5432',
    }
}






