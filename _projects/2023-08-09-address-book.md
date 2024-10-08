---
title: 배송지 관리 기능 개선
subtitle: 해묵은 VoC와 작별하기
date: 2023-08-09 00:00:00
description: 고질적인 VoC였던 불편 사항을 해결해 <br>고객의 매끄러운 주문 경험에 기여한 프로젝트예요.
featured_image: addressbook.jpg
accent_color: "#EF7014"
gallery_images:
  - addressbook.jpg
---


<style>
.no-inherit {
  margin: 0;
}

.custom-heading {
    color: #666;
    font-size: 16px;
    text-align: left;
    margin: 0px;
}
</style>


- **기간**: 2023.7 - 2023.8
- **역할**: 프로덕트 디자이너 (기여도 100%)
- **인원**: 10명
  > PO 1명, 디자이너 1명, 앱 개발자 3명, 웹 개발자 1명, 서버 개발자 3명, QA 1명

#### 배경

아이디어스 서비스에는 10년 가까이 변화 없이 그대로인 화면들이 있었어요.

지금의 보편적인 사용성과 다르고 고객의 눈높이에도 맞지 않기도 하죠. <br> 
불편하고 유쾌하지 못한 경험으로 인해 고객이 이탈하지 않도록 <br> 전사의 모든 구성원이 힘을 모아 한 스프린트 동안 Critical CX를 개선하기로 했습니다.


#### 문제

배송지 관리는 그야말로 '레거시' 화면으로, 기능 불만 관련 VOC 중 `4.1%`로 2위를 차지했어요.
<br>
<br>

![](/images/projects/10_addressbook/00.jpg)


{% include badge.html content="Problem 1" %}
###### 4개 이상 저장 불가
- 선물 구매가 많은 서비스 특성상, <b>주소를 여러 개 저장하려는 니즈</b>가 있으나 충족되지 못했어요.

{% include badge.html content="Problem 2" %}
###### 첫번째 칸 배송지 기본 사용됨
<!-- - <b>첫번째 칸의 배송지가 기본으로 사용돼요. </b> -->
- <b>배송지 오기입</b>으로 작가님[^1]에게 배송지 변경을 직접 요청하는 상황이 자주 발생했어요.

{% include badge.html content="Problem 3" %}

###### 수정/삭제 기능이 없음
- 3개 필드가 모두 찼을 때, 새 배송지가 필요하면 <b>기존 필드를 하나하나 수정해야</b> 해요. <br>삭제 기능이 없어서 한 번에 지울 수도 없었어요.

위와 같은 상황을 방지하기 위해 아이디어스 고객은 주문 시 배송지를 한 번 더 확인해야 하며, 
<br> 이는 결과적으로 <b>고객의 결제를 지연시키는 요인</b>이 되었어요.

![](/images/projects/10_addressbook/01.jpg)


#### Voice of Customer

##### 고객 Voice

{% include callout.html content="주소록 더 늘려주세요 <b>3개밖에 저장 안되니 불편</b>합니다" %}
{% include callout.html content="아이디어스에서 저는 반찬이나 디저트 등 식품 구매를 많이 하는 편인데요, 맛있는 것을 발견하면 부모님, 딸네, 친구들 ...생각나는 사람이 많죠~ 주욱 보내주려고 들어왔다가 주문하는 단계에서 배송지가 세군데밖에 저장이 안되어있으니 또 연락처 찾아서 일일이 검색하고 입력하다 귀찮아져서 어떨땐 5군데쯤 보내려던 마음이 사라지고, 세군데로 축소되기도 합니다. <b>자주 보내는 배송지 저장을 좀 더 늘려주시면 좋겠어요</b>" %}
{% include callout.html content="마지막 주문 주소가 남아있는 바람에 벌써 <b>여러 차례 엉뚱한 곳으로 물건을 보냈습니다.</b> 지인이면 돌려받기라도 할 텐데 선물 보낸 분들인 경우가 많아 돌려받지도 못했습니다. 마지막 주문 주소가 자동으로 입력되는 기능 좀 없애 주세요!!!" %}
{% include callout.html content="선물하기는 어플 없는 사람에게 보내면 불편해하고 노인들은 여러번 누른 후 주소 쓰고 하는거 자체를 어려워 합니다" %}
<!-- {% include callout.html content="기본적으로 주문을 할때 보통 배송기사님이 볼수있는 운송장에 메세지를 남길수 있게 되어있는데 (배송요청사항,배송메세지) 아이디어스는 작가님에게 남길 메세지로 표기가 되어있어 배송기사님이나, 배송메세지를 어디에 남겨야할지 고민하는 순간이 생깁니다. <br> 이런 경우를 생각해서 작가님에게 남기는 메세지와 배송관련 메세지를 따로 남길 수 있게 되어 있거나, 짧은 문구 하나정도 같이 적어놓으면(ex. 작가님or배송관련 메세지를 남겨주세요) 편리하게 이용할 수 있을거 같습니다." %} -->
<br>

##### 작가님 Voice

{% include callout.html content="결국은 주소지 변경건으로 생긴 문제인데 제가 입점하고 몇번을 요청 드렸지만 수정이 안되고 있네요." %}
{% include callout.html content="이 모든 이야기는 고객이 주소변경 가능하게 해달라는 요청을 드리려 한 이야기 입니다. 꼭 한번 다시 검토해 주셨으면 합니다." %}
{% include callout.html content="다시 한번 요청 드립니다. 다른 사이트도 되는 부분이니 꼭 한번 심사숙고 하셔서 수정해 주셨으면 합니다." %}

<br>

##### Data

그동안의 주문자 누적 배송지 수를 확인 결과, 최대 30개 저장을 허용하게 되면 21년 이후 <b>주문자의 99.9% 커버</b>가 가능하기에 <b>저장 가능한 배송지 수를 30개로 결정</b>했어요. 타사 대비 큰 숫자였지만 선물을 많이 하는 아이디어스의 특징을 고려했고, 개발쪽에서도 부담가지 않는 적정선을 찾았어요.

#### 해결 방법

배송지는 주문의 마지막 단계인 <b>주문 결제</b> 화면에서 입력해요. <br>
주문 완료까지의 매끄러운 여정을 위해 <b>클릭과 화면 이동을 최소화한 flow</b>에 중점을 두고 작업했습니다.

<br>

##### 리스트 방식 변경
기존 배송지는 최대 3개까지 탭 방식으로 제공되고 있었어요.

최대 30개까지 추가할 수 있게 바뀐 정책에 따라 <b>리스트를 세로 스크롤 방식으로 변경</b>했어요. <br>
기본 배송지가 최상단, 이후 최근 사용순으로 정렬해 최근 사용한 배송지를 먼저 볼 수 있도록 했어요.


![](/images/projects/10_addressbook/02.jpg)

<b>수정, 삭제는 상세에  들어가지 않고도 가능</b>하도록 리스트에 버튼을 꺼내 기능을 제공했습니다.

<br>

##### 배송지 추가
배송지를 추가 과정에서는 <b>불필요한 클릭을 없애기 위해</b> 특별히 노력했는데요.

![](/images/projects/10_addressbook/03.jpg)

첫째로 추가 버튼을 누르면 화면 위에 주소 검색 <b>화면을 바로 띄워</b> 클릭을 1번 줄였고<br>
둘째로 주소 입력후 추가 화면으로 돌아왔을 때 <b>다음 입력 필드가 바로 포커싱</b> 되도록 했습니다. 

아래 이미지에서 동작을 확인할 수 있어요.

<video autoplay muted loop playsinline>
  <source src="{{ "/images/projects/10_addressbook/04.mp4" | relative_url }}" type="video/mp4">
  Your browser does not support the video tag.
</video>


추가로 키보드 상단 툴바를 추가해 필드간 이동이 쉽도록 했고, 배송지명은 칩을 활용해 필드를 빠르게 채울 수 있게 하는 등 주소 추가 경험이 전반적으로 매끄러울 수 있도록 신경썼습니다.
<!-- 최초 주문시 주문자 정보와 배송지 정보가 N% 일치 data  -->

<!-- <br>

##### 수정/삭제


<br>

##### 배송지명 -->


<br>

#### Casual UT
사정상 Web은 App과는 다른 구조로 적용하게 되었어요.

새 화면에서 추가/수정을 하는 App과 다르게 Web에서는 <b>탭 이동으로 새 배송지를 추가</b>하고, <br>
수정 버튼을 눌러 별도의 화면 이동 없이 수정할 수 있는 구조로 설계했습니다. 

![](/images/projects/10_addressbook/06.gif)

누르는 액션 영역이 상대적으로 많아졌기에 의도대로 사용하는지 Casual UT를 통해 확인했어요.

<br>

##### 1차 테스트

{% include callout.html content="<b>Task:</b> 주소록에 저장되어있는 다른 배송지로 변경해보세요." %}

![](/images/projects/10_addressbook/07.jpg)

3명의 참여자 모두가 상단의 '배송지 변경'이 아닌 '정보 수정' 버튼을 통해 배송지를 변경하려고 하는 모습을 확인할 수 있었어요. 배송지 변경 버튼이 훨씬 크고 강조가 되어있음에도 사용자는 시선이 머물던 주소와 더 가까이 있는 버튼에 반응한다는 레슨런을 얻을 수 있었습니다.

<br>

##### 2차 테스트

{% include callout.html content="<b>Task:</b> 주소록에 저장되어있는 다른 배송지로 변경해보세요. (1차와 동일)" %}

![](/images/projects/10_addressbook/08.jpg)

1차 테스트를 바탕으로 '정보 수정' 버튼을 왼쪽 하단으로 옮겨보았는데요. 추후 진행한 2차 테스트에서 참여자 모두 의도한 대로 사용하는 데 어려움이 없음을 확인하고 테스트를 마쳤습니다.

<!-- 1명의 참여자가 '신규 입력'을 먼저 눌러보긴 했지만 그 후 '배송지 변경' 버튼을 눌러 배송지 변경을 시도했기에 설계대로 동작한다고 판단해 테스트를 마쳤습니다.  -->

<br>

#### 결과

고객이 잘 사용하고 있는지 확인하기 위해 배포 후 1개월 뒤 데이터를 살펴보았는데요.

저장 가능한 배송지수를 늘린 효과가 있는지 확인하기 위해서 배송지를 4개 이상 사용하는 고객을 확인해보았고 배송지 등록 유저 대비 `17%`인 점을 확인할 수 있었어요. 눈에 띄게 높아진 수치였죠.

기본 배송지를 잘 활용하고 있는지를 확인하기 위해서는 **배송지 추가/수정시에 기본 배송지를 설정하는 고객 비중**을 확인해보았고 추가/수정하는 고객의 `20%`가 기본 배송지를 바꿔서 설정한 부분을 확인할 수 있었어요.

기능 관련 불만 2위였던 만큼,VoC 감소도 크게 효과를 느꼈어요. 배송지 관리 기능과 함께 주문 취소 기능이 오픈되었는데요. 그럼에도 취소 비율이 크게 늘지 않은 이유 중 하나로 배송지 관련 어려움이 해소되었기 때문일 거라고 회고하기도 했습니다.



#### 소감

프로덕트 디자이너로 일하면서 비즈니스 목표와 고객의 사용성 사이에서 어디에 더 무게를 둘지 고민하는 순간이 종종 있는데요. 이 프로젝트는 ‘hygiene issue’[^2]를 해결하자는 큰 목표가 있었기에 평소에 가지던 부담에서 벗어나 오로지 사용성에 집중해본 시간이었습니다. Casual UT를 통해 사용성을 검증했던 과정이 특히 기억에 남습니다. 

아주 오래 묵은 VoC를, 앓던 이를 제가 뽑았다는 점도 의미있었어요. 디자이너 이전에 사용자로서 저와 제 동료들 역시 불편함을 겪었던 부분이라 사용자의 입장에서 느낀 기쁨까지 뿌듯함이 배가 되었습니다.


[^1]: 아이디어스에서는 판매자 대신 '작가님', 상품 대신 '작품'이라고 부르고 있어요.
[^2]: 위생요인 : 어떤 분야에서 자신이 경쟁하는 데 필요한 최소한의 서비스나 제품의 스펙. 필수조건. [Link](https://www.bain.com/ko/insights/hygiene-versus-wow-factors/)
