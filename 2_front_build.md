## 룰엔진 인수인계

### Frontend 빌드

#### 1. 로컬

평소에는 ng build로 파일들과 library 정보를 패킹해본다.

특히 ng serve를 로컬 환경에서 자주 쓸텐데, ng build 후 실행된다고 생각하면 된다.

```shell
ng build
```

#### 2. 배포

angular에서는 어떤 상황에서든 배포할 때는 --prod를 붙이도록 권장하고 있다.

--prod는 아래와 같은 여러가지 추가적인 규칙들을 적용해서 빌드하며 시간이 꽤 걸린다.

* 잘못된 binding 정보에 대해 error로 알림
* 잘못된 library 참조에 대해 error로 알림
* 그 외 syntax 에러 등등 dev 버전에서는 넘어가는 warning들을 상대적으로 빡빡하게 잡아냄
* 성능 optimizing 된 버전으로 컴파일한다.

```shell
ng build --prod
```

![image](https://user-images.githubusercontent.com/55048882/85667348-73d98000-b6f8-11ea-8d65-a70a4ba9dac8.png)


-- 위와 같이 몇가지 js 코드로 컴파일이 됨을 알 수 있으며, 이 파일들을 서버에 올리면 그대로 web page로 동작할 수 있는 상태.
