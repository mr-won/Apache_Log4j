# Apache_Log4j
Apache_Log4j
Payload
GET /struts/utils.js HTTP/1.1

- 공격 이름: `Log4Shell`
- 판단 근거: 페이로드에 `${jndi:ldap://}` 패턴이 포함되어 있음
- 탐지 패턴: `${jndi:ldap://}`
- 설명: Log4Shell은 Log4j 라이브러리의 취약점을 이용한 원격 코드 실행 공격입니다.
- 대응 방법: JNDI 룩업을 비활성화하고 Log4j를 최신 버전으로 업데이트하며, 네트워크 트래픽을 모니터링하여 의심스러운 LDAP/RMI 아웃바운드 연결을 차단합니다.
