---

Copyright:
  Years: 2017
lastupdated: "2017-10-24"
---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# Compose for JanusGraph 시작하기
{: #getting-started-with-compose-for-janusgraph}

{{site.data.keyword.composeForJanusGraph_full}}는 수백만 또는 수십억 개의 정점과 에지로 모델링되는 고도로 상호 연결된 데이터를 저장하고 조회하는 데 최적화된 확장 가능한 그래프 데이터베이스입니다. 이러한 복잡한 구조에서 단순하고 효율적으로 데이터를 검색하는 것은 JanusGraph의 Apache Tinkerpop(TM) 호환성을 통해 가능합니다. 이는 기존 관계형 데이터베이스로는 어렵거나 불가능할 수 있는 조회를 효율적으로 수행할 수 있도록 합니다.{{site.data.keyword.composeForJanusGraph}}는 JanusGraph를 관리하고 고가용성 및 중복성과 자동화된 비정지 백업 등을 제공하여 JanusGraph를 더욱 향상시킵니다.
{:shortdesc}

## Compose for JanusGraph 서비스 인스턴스 작성

[{{site.data.keyword.composeForJanusGraph}} 인스턴스를 작성하십시오](https://console.bluemix.net/catalog/services/compose-for-janusgraph/).

서비스의 인스턴스를 작성하는 경우 서비스의 이름과 신임 정보 이름을 모두 선택하십시오. 서비스를 바인딩되지 않은 상태로 두십시오. 서비스가 프로비저닝될 때 제공되는 신임 정보를 사용하여 나중에 애플리케이션을 서비스에 연결할 수 있습니다. 다양한 신임 정보 값과 애플리케이션에서 이를 사용하는 방법은 [{{site.data.keyword.cloud}} 애플리케이션 연결](./connecting-bluemix-app.html)에 자세히 설명되어 있습니다.

서비스 인스턴스를 프로비저닝할 때 *표준* 또는 *엔터프라이즈* 플랜을 선택할 수 있습니다. *엔터프라이즈* 플랜을 사용하면 인스턴스를 사용 가능한 {{site.data.keyword.composeEnterprise}} 클러스터에 프로비저닝할 수 있습니다. {{site.data.keyword.composeEnterprise}}는 엔터프라이즈 준수에 필요한 보안 및 격리를 제공하며 전용 네트워킹을 사용하여 배치된 데이터베이스의 성능을 보장합니다. 세부사항은 [Compose Enterprise 문서](../ComposeEnterprise/index.html)를 참조하십시오.

## Compose for JanusGraph 관리

서비스 대시보드에서 서비스를 관리할 수 있습니다. 여기서 {{site.data.keyword.cloud_notm}} Compose 데이터베이스 및 연결 방법에 대한 정보를 찾을 수 있습니다. 또한 다음을 수행할 수 있습니다.
- 백업 관리
- 서비스에 대한 추가 리소스 할당
- 서비스 비밀번호 변경
- 화이트리스트를 사용하여 데이터베이스에 대한 액세스 제한.
자세한 정보는 [설정](./dashboard-settings.html)을 참조하십시오.

## Compose for JanusGraph에 연결

서비스와 함께 작성된 신임 정보를 사용하거나 서비스 대시보드의 *개요* 탭에서 제공되는 연결 문자열 및 명령행을 사용하여 서비스에 연결할 수 있습니다 

{{site.data.keyword.cloud_notm}} 외부에서 서비스에 연결하려는 경우 제공된 연결 문자열 또는 명령행을 사용할 수 있습니다. [JanusGraph에 연결](./connecting-external.html)에서 자세히 알아볼 수 있습니다.

## {{site.data.keyword.cloud_notm}} 애플리케이션 연결

{{site.data.keyword.cloud_notm}} 애플리케이션을 서비스에 연결하려면 서비스와 함께 작성되는 신임 정보를 사용하십시오. [{{site.data.keyword.cloud_notm}} 애플리케이션 연결](./connecting-bluemix-app.html)에서 {{site.data.keyword.cloud_notm}} 애플리케이션을 {{site.data.keyword.composeForJanusGraph}} 서비스에 연결하는 방법에 대한 정보를 찾을 수 있습니다.

## JanusGraph 데이터 브라우저 사용

명령행에서 그래프 데이터를 탐색하는 것은 복잡한 태스크일 수 있습니다. {{site.data.keyword.composeForJanusGraph}}용 데이터 브라우저는 사용하기 쉬운 조회 빌더와 대화식 JSON 보기 및 시각화된 그래프 모두로 조회를 결과를 표시하는 풍부한 조회 응답 카드를 결합합니다. 자세히 알아보려면 [JanusGraph 데이터 브라우저 사용](./data-browser.html)을 참조하십시오.