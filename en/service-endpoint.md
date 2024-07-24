## Network > Service Gateway > 연동 서비스 엔드포인트

서비스 게이트웨이를 이용하여 NHN Cloud 내부 네트워크로 통신할 수 있는 서비스 목록 및 각 서비스별 엔드포인트입니다.

### 리전 코드

* 리전 서비스는 각 리전별로 엔드포인트 주소가 다르므로 `{region code}`에 아래의 리전 코드를 기입해야 합니다.

| 리전 | 리전 코드 |
| --- | ----- |
| 한국(판교) | kr1 |
| 한국(평촌) | kr2 |
| 일본(도쿄) | jp1 |
| 미국(캘리포니아) | us1 |

### 서비스 게이트웨이 연동 서비스

* 아래 서비스로 서비스 게이트웨이를 생성하면 인터넷을 경유하지 않고, NHN Cloud 내부 네트워크로 접근할 수 있습니다.
    * 서비스 게이트를 생성하는 방법은 [Service Gateway > 콘솔 사용 가이드](https://docs.nhncloud.com/ko/Network/Service%20Gateway/ko/console-guide/)를 참고하시기 바랍니다.
    * 아래 기재되지 않은 서비스는 [고객센터](https://www.nhncloud.com/kr/support/inquiry)로 문의해 주시기 바랍니다.
* 서비스 게이트웨이를 생성할 수 있는 서비스 및 엔드포인트 주소입니다.
    * `/etc/hosts` 파일에 서비스 게이트웨이의 IP 주소와 접근하고자 하는 서비스 엔드포인트 주소를 추가해야 URL로 접속할 수 있습니다.
        * 예시) <span style="color:rgb(68, 68, 68);">192</span><span style="color:rgb(136, 0, 0);" class="hljs-selector-class">.168.1.42</span><span style="color:rgb(68, 68, 68);"> </span><span style="color:rgb(68, 68, 68);" class="hljs-selector-tag">kr1-api-object-storage</span><span style="color:rgb(136, 0, 0);" class="hljs-selector-class">.nhncloudservice.com</span>

| 서비스 | <span style="color:rgb(255, 255, 255);">서비스 게이트웨이 엔드포인트 이름</span> | 엔드포인트 주소 |
| --- | ------------------ | -------- |
| IaaS API Identity (nhncloudservice.com) | IaaS API Identity (nhncloudservice.com) | <span style="color:rgb(49, 51, 56);">[https://api-identity-infrastructure.nhncloudservice.com](https://api-identity-infrastructure.nhncloudservice.com)</span> |
| IaaS API Key-Manager | IaaS API Key-Manager | <span style="color:rgb(49, 51, 56);">[https://](https://kr1-api-key-manager-infrastructure.nhncloudservice.com)</span>`{region code}`<span style="color:rgb(49, 51, 56);">[-api-key-manager-infrastructure.nhncloudservice.com](https://kr1-api-key-manager-infrastructure.nhncloudservice.com)</span> |
| IaaS API Compute | IaaS API Compute | <span style="color:rgb(49, 51, 56);">[https://](https://kr1-api-instance-infrastructure.nhncloudservice.com)</span>`{region code}`<span style="color:rgb(49, 51, 56);">[-api-instance-infrastructure.nhncloudservice.com](https://kr1-api-instance-infrastructure.nhncloudservice.com)</span> |
| IaaS API Network | IaaS API Network | <span style="color:rgb(49, 51, 56);">[https://](https://kr1-api-network-infrastructure.nhncloudservice.com)</span>`{region code}`<span style="color:rgb(49, 51, 56);">[-api-network-infrastructure.nhncloudservice.com](https://kr1-api-network-infrastructure.nhncloudservice.com)</span> |
| IaaS API Volume v2 | IaaS API Volume v2 | <span style="color:rgb(49, 51, 56);">[https://](https://kr1-api-block-storage-infrastructure.nhncloudservice.com)</span>`{region code}`<span style="color:rgb(49, 51, 56);">[-api-block-storage-infrastructure.nhncloudservice.com](https://kr1-api-block-storage-infrastructure.nhncloudservice.com)</span> |
| IaaS API Container - Infra | IaaS API Container - Infra |  |
| NHN Container Registry(NCR) | NHN Container Registry(NCR)<br>API Gateway | 사용자 레지스트리 URI<br>[https://](https://kr1-ncr.api.nhncloudservice.com/)`{region code}`[-ncr.api.nhncloudservice.com](https://kr1-ncr.api.nhncloudservice.com/) |
| DNS Plus | API Gateway | <span style="color:rgb(49, 51, 56);">[https://dnsplus.api.nhncloudservice.com](https://dnsplus.api.nhncloudservice.com/)</span> |
| Object Storage | Object Storage | <span style="color:rgb(49, 51, 56);">[https://](https://kr1-api-object-storage.nhncloudservice.com)</span>`{region code}`<span style="color:rgb(49, 51, 56);">[-api-object-storage.nhncloudservice.com](https://kr1-api-object-storage.nhncloudservice.com)</span> |
| RDS for MySQL | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-rds-mysql.api.nhncloudservice.com</span> |
| RDS for MariaDB | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-rds-mariadb.api.nhncloudservice.com</span> |
| Server Security Check | Server Security Check |  |
| Security Monitoring | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-secmon.api.nhncloudservice.com</span> |
| Gamebase | API Gateway | <span style="color:rgb(49, 51, 56);">[https://api-gamebase.nhncloudservice.com](https://api-gamebase.nhncloudservice.com)</span> |
| Launching | API Gateway | [https://launching.api.nhncloudservice.com](https://launching.api.nhncloudservice.com/) |
| CDN | API Gateway | [https://cdn.api.nhncloudservice.com](https://cdn.api.nhncloudservice.com) |
| RCS Bizmessage | API Gateway | [https://rcs-bizmessage.api.nhncloudservice.com](https://rcs-bizmessage.api.nhncloudservice.com) |
| Email | API Gateway | [https://email.api.nhncloudservice.com](https://email.api.nhncloudservice.com) |
| Face Recognition | API Gateway | [https://face-recognition.api.nhncloudservice.com](https://face-recognition.api.nhncloudservice.com) |
| AI Fashion | API Gateway | <span style="color:rgb(49, 51, 56);">[https://api-aifashion.nhncloudservice.com](https://api-aifashion.nhncloudservice.com)</span> |
| OCR | API Gateway | <span style="color:rgb(49, 51, 56);">[https://ocr.api.nhncloudservice.com](https://ocr.api.nhncloudservice.com)</span> |
| Text to Speech | API Gateway | <span style="color:rgb(49, 51, 56);">[https://speech.api.nhncloudservice.com](https://speech.api.nhncloudservice.com)</span> |
| Speech to Text | API Gateway | <span style="color:rgb(49, 51, 56);">[https://speech.api.nhncloudservice.com](https://speech.api.nhncloudservice.com)</span> |
| Pose Estimation | API Gateway | <span style="color:rgb(49, 51, 56);">[https://pose-estimation.api.nhncloudservice.com](https://pose-estimation.api.nhncloudservice.com)</span> |
| Maps | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-maps.api.nhncloudservice.com</span> |
| ROLE | API Gateway | [https://role.api.nhncloudservice.com](https://role.api.nhncloudservice.com) |
| API Gateway | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-apigateway.api.nhncloudservice.com</span> |
| Cloud Search | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-search.api.nhncloudservice.com</span> |
| Autocomplete | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-autocomplete.api.nhncloudservice.com</span> |
| Word Suggestion | API Gateway | [https://word-suggestion.api.nhncloudservice.com](https://word-suggestion.api.nhncloudservice.com/v1.0/appkeys/%7BappKey%7D/word-suggestion/suggestion) |
| Pipeline | API Gateway | <span style="color:rgb(49, 51, 56);">https://</span>`{region code}`<span style="color:rgb(49, 51, 56);">-pipeline.api.nhncloudservice.com/</span> |
| Certificate Manager | API Gateway | [https://certmanager.api.nhncloudservice.com](https://certmanager.api.nhncloudservice.com) |
| CloudTrail | CloudTrail<br>API Gateway | [https://cloud-trail.api.nhncloudservice.com](https://cloud-trail.api.nhncloudservice.com) |
| Resource Watcher | API Gateway | [https://resource-watcher.api.nhncloudservice.com](https://resource-watcher.api.nhncloudservice.com) |