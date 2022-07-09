# Django and Pythonanywhere

이 글은 Django와 Pythonanywhere를 이용하면서 겪은 삽질들을 기록하기위해 만들었습니다.

> **warning**
잘못된 정보가 있을 수 있습니다.


> os -> window, tool -> vscode

## How to host web using Django and Pythonanywhere

1. Local 에서 정상적으로 실행되는 Django project를 구현합니다.
    * Project Create
        ~~~ python
        python -m venv venv # project 폴더에 venv라는 가상환경을 생성해줍니다.
        ~~~
    * Install module to venv and Test
        1. F1을 눌러서 인터프리터를 가상환경의 python으로 지정해준다

        2. vscode의 터미널에서 가상환경에 필요한 모듈을 설치한다
            >가상환경에 접근이 안되는 경우 관리자 권한으로 powershell을 실행후,
            > Set-ExecutionPolicy Unrestricted 를 입력

        3. pip install django 를 가상환경의 터미널에 입력 (가상환경에 django install)

        4. python django-admin startproject "project name" 를 입력 (프로젝트 폴더에 django 프로젝트 폴더 생성)

        5. python django-admin startapp "app name"을 입력 (프로젝트 폴더에 django app 폴더 생성)

        6. django project 구현 (django project 폴더를 지정한 터미널로 아래 코드 입력)

            ~~~
            python manage.py runserver # django project running in Local
            ~~~

        7. Local에서 정상적으로 실행이 됨을 확인
## ERROR