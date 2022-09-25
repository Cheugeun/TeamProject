![header](https://capsule-render.vercel.app/api?type=wave&color=auto&height=300&section=header&text=2022%20OSS%20TeamProject&fontSize=60)



# Open Source SoftWare 
> 2022 OSS 수요일 오전반 6조



## 5장 서버
1. [서버 저장소](#서버-저장소)
2. [깃허브 서버 준비](#깃허브-서버-준비)
3. [깃허브 연동 및 원격 등록](#깃허브-연동-및-원격-등록)
4. [서버 전송](#서버-전송)
5. [자동으로 내려받기](#자동으로-내려받기)
6. [수동으로 내려받기](#수동으로-내려받기)
7. [순서](#순서)

## 서버 저장소

서버 저장소는 다른 말로 원격(remote) 저장소라고도 합니다.
- 5.1.1 협업 저장소

    - ```깃은 여러 개발자와 협업하려고 탄생한 도구입니다. 인터넷에 연결하여 작업할 수 없는 개발환경도 많이 있기때문에 이 두 가지 환경을 고려하여 분산형 모델을 선택했습니다.```

- 5.1.2 연속된 작업
  - ```서버 저장소는 여러 컴퓨터에 동일한 깃 저장소를 복제하고, 작업한 결과물을 다시 서버로 통합합니다.```

- 5.1.3 새 멤버
    - ```새 멤버가 추가 되어도 깃은 깃의 원격 저장소 주소만 알려 주면 모두 해결됩니다.```

## 깃허브 서버 준비
독립적인 깃 서버를 직접 운영하여 사용할 수 있습니다. 하지만 365일 안정적인 서버를 운영하는 것은 쉽지 않습니다. 직접 서버를 운영하지 않아도 전문적인 깃 호스팅으로 서버를 대체할 수 있습니다. 호스팅을 받으면 직접 서버를 관리하지 않아도 쉽게 원격 저장소를 운영할 수 있습니다.

- 5.2.1 깃허브

    - 깃허브는 대표적인 깃호스팅 서비스입니다. 깃허브의 모든 서비스는 무료로 사용할 수 있습니다. 서비스를 사용하려면 먼저 회원 가입이 필요합니다. 회원 가입을 하려면 이메일 주소가 필요합니다. 사용자 이름은 영문으로 작성하며, 저장소를 구별하는 주소 값으로 사용합니다. 일반적으로 개별 깃허브 주소는 다음과 같이 표현합니다.  ```"https://github.com/사용자이름"``` 

- 5.2.2 저장소 생성
  - 한 소유자 안에서 같은 저장소 이름은 중복하여 생성할 수 없습니다.


## 깃허브 연동 및 원격 등록
깃허브에 새 저장소를 생성했다면 이제 로컬 저장소와 연결해야 합니다. 기존 로컬 저장소와 연결하거나 새 로컬 저장소를 생성하여 연결할 수도 있습니다.

- 5.3.1 로컬 저장소

    - (깃허브에 new repository생성 후)   
    ```$ git init``` 명령어로 깃을 초기화한 다음저장소의 소개페이지 파일을 생성합니다.  
   ``$ echo "# gitstudy" >> README.md  -- 파일생성  
   $ git add README.md     
   $ git commit -m "first commit"``

- 5.3.2 프로토콜
  - 서버와 통신하려면 프로토콜을 사용해야 합니다. 깃은 기본적으로 Local, HTTP, SSH, Git 네 종류의 전송 방식을 지원합니다.
  - Local(로컬)  
  로컬 컴퓨터에 원격 저장소를 생성하는것을 의미합니다.자신의 컴퓨터를 NFS(Network File System)등 서버로 이용할때 편리합니다. 로컬저장소를 서버로 이용할때는 폴더경로만 입력합니다.   
  ```$ git remote add 원격저장소별칭 폴더경로```   
  로컬은 간단한 원격서버 구축이 가능하고 빠른 동작이 가능하나 모든 자료가 자신의 컴퓨터에 집중되는 위험이 있습니다.  


## 서버 전송

모든 개발 의존성 설치 방법과 자동 테스트 슈트 실행 방법을 운영체제 별로 작성합니다.

```sh
make install
npm test
```

## 자동으로 내려 받기

* 0.2.1
    * 수정: 문서 업데이트 (모듈 코드 동일)
* 0.2.0
    * 수정: `setDefaultXYZ()` 메서드 제거
    * 추가: `init()` 메서드 추가
* 0.1.1
    * 버그 수정: `baz()` 메서드 호출 시 부팅되지 않는 현상 (@컨트리뷰터 감사합니다!)
* 0.1.0
    * 첫 출시
    * 수정: `foo()` 메서드 네이밍을 `bar()`로 수정
* 0.0.1
    * 작업 진행 중

## 수동으로 내려 받기

* 0.2.1
    * 수정: 문서 업데이트 (모듈 코드 동일)
* 0.2.0
    * 수정: `setDefaultXYZ()` 메서드 제거
    * 추가: `init()` 메서드 추가

## 순서

* 0.2.1
    * 수정: 문서 업데이트 (모듈 코드 동일)
* 0.2.0
    * 수정: `setDefaultXYZ()` 메서드 제거
    * 추가: `init()` 메서드 추가

## 정보

이름 – [@트위터 주소](https://twitter.com/dbader_org) – 이메일주소@example.com

XYZ 라이센스를 준수하며 ``LICENSE``에서 자세한 정보를 확인할 수 있습니다.

[https://github.com/yourname/github-link](https://github.com/dbader/)
