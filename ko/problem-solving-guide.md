# Cloud Access 문제 해결 가이드

**Security > Cloud Access > 문제 해결 가이드**

<br>

## 에이전트를 연결했으나 인스턴스에 접속되지 않습니다.

로그인 후 인스턴스에 접속하려면 아래 설정을 추가해야 합니다.

* 라우트 설정
    * 자세한 내용은 [콘솔 사용 가이드 - 시작하기](https://docs.nhncloud.com/ko/Security/Cloud%20Access/ko/console-user-guide/cloud-access-start/)를 참고하세요.
* ACL 정책 설정
    * 내부 인스턴스에 접근 시 적용되는 접근 제어 정책입니다. **ACL 정책** 탭에서 IP를 허용해야 합니다.
* Security Groups 설정
    * 인스턴스의 보안 그룹에서 출발지 IP를 허용해야 합니다.

<br>

## 윈도우 사용자인데 생체 인증이 적용되지 않습니다.

Cloud Access의 생체 인증 기능은 지문이나 얼굴 인식이 가능한 디바이스에서만 사용할 수 있습니다. 생체 인증이 없는 경우에는 **계정 > 로그인 옵션** 메뉴에서 PIN 설정 후 생체 인증을 대체하여 사용 가능합니다.

<br>

## 사용자 계정이 생성되어 있는데 사용자 객체 추가 버튼을 눌러도 항목이 나타나지 않습니다.

아래의 경우 사용자 객체 추가 목록에 노출되지 않습니다.

* 사용자 계정을 생성한 직후부터 인증 완료 전까지
    * 인증이 완료되어야 IP 확인이 가능합니다.
* 사용자 계정 생성 시 IP 타입을 유동 IP(dynamic IP)로 설정한 사용자 계정

<br>

## 비밀번호 정책을 사용으로 설정했는데 조건에 맞지 않는 비밀번호로도 로그인이 가능합니다.

비밀번호 정책을 **사용**으로 설정하고 저장했더라도 기존 사용자나 이미 비밀번호를 변경한 사용자 계정은 해당 정책이 적용되지 않습니다.
비밀번호 정책은 **초기 비밀번호 강제 변경** 옵션을 선택해 새로 생성한 사용자 계정만 적용됩니다. 이런 경우 해당 사용자 계정의 비밀번호를 초기화한 뒤 정책에 맞는 비밀번호를 사용하도록 안내하세요.  

<br>

## 초기 비밀번호 강제 변경을 설정했지만 로그인 시 변경 화면이 나타나지 않습니다.

**초기 비밀번호 강제 변경** 옵션을 선택하여 새로 생성한 사용자 계정에만 설정이 적용됩니다. 설정 전에 생성된 사용자 계정이나 이미 생성된 사용자 계정에서 옵션을 변경할 경우에는 설정이 적용되지 않습니다. 해당 사용자 계정의 비밀번호를 초기화한 뒤 변경을 진행하세요.

<br>

## 계정 연결 버튼을 클릭했는데 활성화된 서비스가 없다는 팝업이 나옵니다.

Cloud Access 서비스가 비활성화 상태일 경우 계정 연결이 불가능합니다. 서비스를 활성화한 후 연결을 다시 추가하거나 불필요한 연결이라면 삭제하세요.

<br>

## 판교와 평촌 리전 모두에서 서비스를 활성화한 뒤 하나의 리전만 비활성화할 수 없습니다.

현재는 모든 리전에서 동시에 비활성화되는 방식으로 구현되어 있어 특정 리전만 따로 비활성화하는 기능은 지원하지 않습니다.
원하는 리전에서만 사용하려면 서비스를 비활성화한 후 사용할 리전에서만 다시 활성화하세요(개별 리전 삭제 기능은 향후 추가 예정입니다).

<br>

!!! tip "문제가 해결되지 않을 경우"
    문제 해결 가이드의 안내에 따라 진행하였으나 문제가 해결되지 않을 경우 NHN Cloud 고객 센터로 문의하세요.
    * [온라인 1:1 문의 바로가기](https://www.nhncloud.com/kr/support/inquiry?alias=tab16_15)
    * 대표 전화: 1588-7967(운영시간: 월~금 10:00-19:00)