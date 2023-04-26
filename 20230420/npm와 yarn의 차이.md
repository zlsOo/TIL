# npm과 yarn의 차이

```
npm과 yarn은 자바스크립트 런타임 환경인 노드(Node.js)의 패키지 관리자이다.
```

### npm 명령어
npm init : package.json 생성
npm install : package.json 파일 및 해당 종속성에 나열된 모든 모듈을 설치
npm install package_name@버전 : 특정 패키지의 특정 버전 설치
npm install 주소 : 특정 저장소 내 패키지 설치. 주로 github을 이와 같이 설치합니다.
npm install package_name -g : 옵션. 글로벌로 설치. 로컬의 다른 프로젝트도 이 패키지를 사용 가능하게 됩니다.
npm uninstall : 패키지 삭제 명령어입니다.
npm update : 설치한 패키지들을 업데이트해줍니다.
npm dedupe : 중복 설치된 패키지들을 정리해주는 명령어입니다.

### yarn 명령어
yarn init : package.json 생성
yarn or yarn install : package.json 파일 및 해당 종속성에 나열된 모든 모듈을 설치
yarn add package_name@버전 : 특정 패키지의 특정 버전 설치`yarn add 주소 : 특정 저장소 내 패키지 설치. 주로 github을 이와 같이 설치합니다.
yarn global add package_name : 옵션. 글로벌로 설치. 로컬의 다른 프로젝트도 이 패키지를 사용 가능하게 됩니다.
yarn remove : 패키지 삭제 명령어입니다.
yarn upgrade : 설치한 패키지들을 업데이트해줍니다.
npm dedupe : 중복 설치된 패키지들을 정리해주는 명령어입니다.

### npm vs yarn
#### 속도

```
npm과 yarn의 차이점 중 하나는 패키지 설치 프로세스를 처리하는 법이다. npm은 패키지를 한 번에 
하나씩 순차적으로 설치하는 방면 yarn은 여러 패키지를 동시에 가져오고 설치하도록 되어 있어 패키지 설치 속도에선 yarn이 npm보다 빠르다.
```

#### 보안
```
yarn은 보안 측면에서 npm보다 더 안전하다. npm은 자동으로 패키지에 포함된 다른 패키지 코드를 실행한다.
이 특징은 편리하지만 안정성을 위협할 수 있다. 이로 인해 보안에 취약성이 발생하고 나중에 심각한 문제가 발생할 수 있다. 반면에 yarn은
yarn.lock 또는 package.json파일에 있는 파일만을 설치한다. 보안은 yarn의 핵심 기능 중 하나지만 최근 npm의 업데이트에서 npm의 모안 업데이트도 크게 향상 됐다.
```