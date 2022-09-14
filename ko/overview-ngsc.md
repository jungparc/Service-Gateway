## Network > Service Gateway > 개요

**Service Gateway** 서비스를 이용하면 **플로팅 IP**를 쓰지 않고 트래픽이 인터넷을 경유하지 않고도 **VPC** 외부의 NHN Cloud의 **서비스**를 이용할 수 있습니다. **서비스 게이트웨이 생성** 시 선택된 **서비스**와 자동으로 할당된 IP는 1:1 연결 관계를 유지하며, **VPC**에서는 **서비스 게이트웨이**의 IP를 이용하여 NHN Cloud의 내부 네트워크를 경유해 대상 **서비스**를 안전하게 이용할 수 있습니다.

### 주요 기능

* VPC에서 인터넷을 경유하지 않고 서비스 게이트웨이에서 제공하는 NHN Cloud의 서비스에 연결할 수 있습니다.
* 서비스 게이트웨이 생성 시 서비스 목록에 제공되는 서비스만 이용이 가능합니다.
* 서비스 게이트웨이의 IP 주소는 서비스 게이트웨이 생성 시 선택된 서비스와 1:1로 연결됩니다.
* 서비스 게이트웨이는 서비스 게이트웨이가 생성된 VPC 내에서만 사용이 가능합니다.
* VPC의 VM Instance에서 서비스 게이트웨이의 IP 주소로 통신 시 서비스 게이트웨이와 연결된 서비스와 통신됩니다.

### 제공 서비스

VPC의 VM Instance에서 인터넷을 경유하지 않고 NHN Cloud의 서비스에 접근이 필요한 경우 서비스 게이트웨이에서 제공되는 서비스를 선택하여 서비스 게이트웨이를 생성합니다.
자세한 사용 방법은 [**사용자 가이드**](https://docs.ngsc-nhncloud.com/ko/TOAST/ko/Overview-ngsc/)를 참고하시기 바랍니다. 제공되는 서비스는 점차 늘려나갈 예정입니다.

* IaaS API Identify 항목은 오브젝트 스토리지 이용에 필요한 서비스입니다. 더 자세한 설명은 [**사용자 가이드 > Storage > Object Storage > API 가이드 > 인증 토큰 발급**](https://docs.ngsc-nhncloud.com/ko/Storage/Object%20Storage/ko/api-guide-gov/)을 참고하시기 바랍니다.