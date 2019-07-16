1. 로컬 환경에서 빌드하기

로컬 환경에서 애플리케이션을 운영용을 빌드하려면 StackBlitz 프로젝트의 소스 코드를 다운받아야 합니다. 메뉴 왼쪽에 있는 Download Project 아이콘을 클릭해서 프로젝트를 다운로드 받으세요.

소스 코드를 다운로드받고 압축을 해제했다면 Angular 콘솔로 애플리케이션을 실행해볼 수 있습니다. 이 때 Node.js와 Angular CLI가 먼저 설치되어 있어야 합니다.

Angular CLI를 설치하려면 터미널에서 다음 명령을 실행하면 됩니다:

content_copy
npm install -g @angular/cli

이 명령을 실행해서 Angular CLI를 설치하고 나면 터미널에서 ng 명령을 실행할 수 있습니다. Angular CLI를 활용하면 새로운 워크스페이스를 만들거나 새로운 프로젝트를 만들 수 있고, 애플리케이션을 개발용 서버에서 띄울 수 있으며 운영용으로 빌드할 수도 있습니다.

새로운 Angular CLI 워크스페이스를 생성하려면 ng new 명령을 다음과 같이 실행하면 됩니다:

content_copy
ng new my-project-name
그리고 이렇게 생성한 프로젝트나 StackBlitz 에서 다운로드받은 프로젝트의 /src 폴더로 이동한 후에 다음 명령을 실행하면 애플리케이션을 빌드할 수 있습니다:

content_copy
ng build --prod
이제 배포할 준비는 끝났습니다.
