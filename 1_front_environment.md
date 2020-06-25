## 룰엔진 인수인계

### Frontend 환경

#### 0. Cloud HIS 프로젝트 개발자에 한해
* rulebase 코드에 대한 접근 권한이 있어야함
* 디버그 모드 로컬 실행 시 프로젝트 서버에 대한 접근 권한이 있어야함

#### 1. npm

Cloud HIS 프로젝트를 진행 했다면 npm은 기본으로 깔려 있을 것.

[없다면 다운로드](https://nodejs.org/en/download/)
```shell
##터미널
npm -v
## 결과: 6.9.0
```

#### 2. Angular

#### (1) angular CLI

[이 링크에서 다운로드](https://cli.angular.io/)

```shell
##터미널
ng v
## 결과:
     _                      _                 ____ _     ___
    / \   _ __   __ _ _   _| | __ _ _ __     / ___| |   |_ _|
   / △ \ | '_ \ / _` | | | | |/ _` | '__|   | |   | |    | |
  / ___ \| | | | (_| | |_| | | (_| | |      | |___| |___ | |
 /_/   \_\_| |_|\__, |\__,_|_|\__,_|_|       \____|_____|___|
                |___/


Angular CLI: 8.2.1
Node: 10.16.3
OS: win32 x64
Angular:
.... 생략
```
** rule engine은 8.2.1 cli를 갖고 만들었습니다.


#### (2) angular Application

rule engine 코드를 받은 후 develop branch에서 전체 패키지 install

```Shell
cd D:\CHIS\Frontend\rulebase
npm install
## package.json을 바라보며 인스톨 진행
```

#### (3) angular 실행

rule engine 로컬 환경 실행

```Shell
ng serve
### 기본적으로 environment.ts 파일에 environment.development.ts를 엎어 실행
```
![image](https://user-images.githubusercontent.com/55048882/85658112-d6794e80-b6ed-11ea-8326-679dc7587bb3.png)

위와 같이 localhost:4200 포트에서 실행되며, 로그인까지 가능하면 성공.