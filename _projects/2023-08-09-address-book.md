---
title: idus
subtitle: 배송지 관리 기능 개선
date: 2023-08-09 00:00:00
description: 배송지 관리 기능을 도입해 고객과 작가님의 고질적인 VOC였던 배송지 관련 불편사항을 해결하고, 고객의 매끄러운 주문 경험에 기여한 프로젝트입니다.
featured_image: addressbook.jpg
accent_color: "#EF7014"
gallery_images:
  - addressbook.jpg
layout: protected
password: "240608"

---

- **기간**: 2023.7 - 2023.8
- **역할**: 프로덕트 디자이너 (기여도 100%)
- **인원**: 10명
  > PO 1명, 디자이너 1명, 앱 개발자 3명, 웹 개발자 1명, 서버 개발자 3명, QA 1명

#### 배경

아이디어스는 2023년 기준 9년이 된 서비스로, 9년 전에 만든 화면을 그대로 사용하는 곳이 존재하기도 해요. 지금의 보편적인 사용성과 다르고 고객의 눈높이에도 맞지 않기도 하죠.

불편하고 유쾌하지 못한 경험으로 인해 고객이 이탈하지 않도록 보완하는 작업이 그 어느 때 보다 필요한 시점이었기에 전사의 모든 구성원이 힘을 모아 한 스프린트 동안 Critical CX를 개선하기로 했습니다.


#### 문제점

배송지 관리는 첫 배포 이후 추가 개선이 없던 그야말로 '레거시' 화면이에요. 실제로 9개월 간 수집한 기능 불만 관련 VOC 중 `4.1%`가 배송지 기능에 대한 의견이었고, 이는 찜 기능 다음으로 많은 비중이었어요.

- 고객은 배송지를 **최대 3개**까지 저장할 수 있어요.
  - 배송지가 3개까지만 저장되므로, 새로운 배송지가 필요한 경우 기존 배송지 중 하나를 수정하는 식으로 입력해야 해요. 삭제 기능이 없기 때문에 한 번에 지울 수도 없었어요.
  - 선물용 작품 구매 빈도가 높은 아이디어스 특성상, 선물 받을 지인들의 주소를 여러 개 저장하려는 고객 니즈가 있으나 충족되지 못하는 상황이었어요. 

![](/images/projects/10_addressbook/00.jpg)

- 첫번째 칸에 입력한 배송지가 주문 결제 시 기본으로 선택돼요. 
  - 첫번째 칸에 지인의 배송지를 입력했다가 다음 주문 시 잘못된 주소로 주문하는 등, 배송지 오기입으로 인해 작가님에게 배송지 변경을 직접 요청해야하는 상황이 자주 발생했어요.
  - 배송지 변경을 위해 주문 전체를 취소하는 상황이 발생하기도 해요. 정책상 작가님에게 직접 연락해야 취소할 수 있기 때문에 이로 인한 작가님의 불편, 고객의 불편 모두 VOC를 통해 확인되고 있었어요.

위와 같은 상황을 방지하기 위해 아이디어스 고객은 주문 시 배송지를 한 번 더 확인해야 하며, 이는 결과적으로 고객의 결제를 지연시키는 요인이 되었어요.

![](/images/projects/10_addressbook/01.jpg)

#### 리서치

##### 고객 VOC

{% include callout.html content="주소록 더 늘려주세요 3개밖에 저장 안되니 불편합니다" %}
{% include callout.html content="선물하기가 있지만 어플 없는 사람에게 보내면 불편해하고 노인들은 여러번 누른후 주소쓰고 하는거 자체를 어려워 합니다" %}
{% include callout.html content="아이디어스에서 저는 반찬이나 디저트 등 식품 구매를 많이 하는 편인데요, 맛있는 것을 발견하면 부모님, 딸네, 친구들 ...생각나는 사람이 많죠~ 주욱 보내주려고 들어왔다가 주문하는 단계에서 배송지가 세군데밖에 저장이 안되어있으니 또 연락처 찾아서 일일이 검색하고 입력하다 귀찮아져서 어떨땐 5군데쯤 보내려던 마음이 사라지고, 세군데로 축소되기도 합니다. 자주 보내는 배송지 저장을 좀 더 늘려주시면 좋겠어요" %}
{% include callout.html content="마지막 주문 주소가 남아있는 바람에 벌써 여러 차례 엉뚱한 곳으로 물건을 보냈습니다. 지인이면 돌려받기라도 할 텐데 선물 보낸 분들인 경우가 많아 돌려받지도 못했습니다. 마지막 주문 주소가 자동으로 입력되는 기능 좀 없애 주세요!!!" %}
<!-- {% include callout.html content="기본적으로 주문을 할때 보통 배송기사님이 볼수있는 운송장에 메세지를 남길수 있게 되어있는데 (배송요청사항,배송메세지) 아이디어스는 작가님에게 남길 메세지로 표기가 되어있어 배송기사님이나, 배송메세지를 어디에 남겨야할지 고민하는 순간이 생깁니다. <br> 이런 경우를 생각해서 작가님에게 남기는 메세지와 배송관련 메세지를 따로 남길 수 있게 되어 있거나, 짧은 문구 하나정도 같이 적어놓으면(ex. 작가님or배송관련 메세지를 남겨주세요) 편리하게 이용할 수 있을거 같습니다." %} -->
<br>
##### 작가 VOC

{% include callout.html content="결국은 주소지 변경건으로 생긴 문제인데 제가 입점하고 몇번을 요청 드렸지만 수정이 안되고 있네요." %}
{% include callout.html content="다시 한번 요청 드립니다. 다른사이트도 되는 부분이니 꼭 한번 심사숙고 하셔서 수정해 주셨으면 합니다." %}
{% include callout.html content="이 모든 이야기는 주소변경 고객이 가능하게 해달라는 요청을 드리려 한 이야기 입니다. 꼭 한번 다시 검토 해 주셨으면 합니다." %}

<br>
##### 현황 파악

주문자의 누적 배송지 개수 분포를 확인 결과, 최대 30개 저장을 허용하게 되면 21년 이후 주문자의 99.9% 커버가 가능하기에 <b>저장 가능한 배송지 수를 30개로 결정</b>했어요. 타사 대비 큰 숫자였지만 선물을 많이 하는 아이디어스의 특징을 고려했고, 개발쪽에서도 부담가지 않는 적정선을 찾았어요.

#### 개선 방향

배송지는 주문의 마지막 단계인 <b>주문 결제</b> 화면에서 입력해요. <br>
주문 완료까지의 매끄러운 여정을 위해 <b>클릭과 화면 이동을 최소화한 flow</b>를 만드는 데 중점을 두고 작업했습니다.

<br>

##### 리스트 방식 변경
탭으로 3개까지만 제공되던 기존 방식에서 30개까지 늘어난 정책에 맞추어 세로 스크롤되는 리스트로 변경했습니다. 기본 배송지가 최상단, 이후 최근 사용순으로 정렬해 최근 사용한 배송지를 먼저 확인할 수 있도록 했어요.


![](/images/projects/10_addressbook/02.jpg)

해당 플로우에서 추가 및 수정, 삭제가 바로 가능하며 특히 수정, 삭제는 상세에  들어가지 않고도 가능하도록 리스트에 버튼을 꺼내 기능을 제공했습니다.

<br>

##### 배송지 추가
배송지를 추가 과정에서는 불필요한 클릭을 없애기 위해 특별히 노력했는데요.

![](/images/projects/10_addressbook/03.jpg)

첫째로 추가 버튼을 누르면 화면 위에 주소 검색 화면을 바로 띄워 클릭을 1번 줄였고<br>
둘째로 주소 입력 완료후에 추가 화면으로 돌아왔을 때 세부 주소 입력 필드가 바로 포커싱 되도록 했습니다. 

아래 이미지에서 동작을 확인할 수 있어요.

![](/images/projects/10_addressbook/04.gif)


추가로 키보드 상단 툴바를 추가해 필드간 이동이 쉽도록 했고, 배송지명은 칩을 활용해 필드를 빠르게 채울 수 있게 하는 등 주소 추가 경험이 전반적으로 매끄러울 수 있도록 신경썼습니다.
<!-- 최초 주문시 주문자 정보와 배송지 정보가 N% 일치 data  -->

<!-- <br>

##### 수정/삭제


<br>

##### 배송지명 -->


<br>

##### Web 케이스
Web은 기술전환이 진행중이던 상황이어서 App과는 다른 구조로 적용할 수밖에 없었는데요.
App처럼 새 화면에서 추가/수정을 수행할 수 없었기 때문에 탭 이동으로 새 배송지를 추가하고, 수정 버튼을 눌러 별도의 화면 이동 없이 수정할 수 있는 구조로 설계했습니다. 

![](/images/projects/10_addressbook/06.gif)

상대적으로 누를 수 있는 액션 영역이 많아졌기에  의도한 방향으로 사용하는지 Casual UT를 통해 확인했습니다.

총 2번의 테스트에 각각 3명씩 총 6명 대상으로 테스트했고, 참여자에게 현재 배송지에서 다른 배송지로 변경하는 task를 제시했습니다.

초기 시안을 활용한 1차 테스트에서는 3명의 참여자 모두가 상단의 '배송지 변경'이 아닌 '정보 수정' 버튼을 통해 배송지를 수정하려고 하는 모습을 확인할 수 있었는데요. 배송지 변경 버튼이 훨씬 크고 강조가 되어있음에도 사용자는 시선이 머물던 주소와 더 가까이 있는 버튼에 반응한다는 레슨런을 얻을 수 있었습니다.

![](/images/projects/10_addressbook/07.jpg)

2차 테스트에서는 '정보 수정' 버튼을 왼쪽 하단으로 옮긴 후 또 다른 3명의 참여자를 대상으로 테스트 했습니다. 3명 중 2명의 참여자가 '배송지 변경' 버튼을 눌러 설계한 의도대로 배송지 변경을 시도했고, 나머지 1명의 참여자는 '신규 입력'을 먼저 눌러보긴 했지만 그 후 '배송지 변경' 버튼을 눌러 배송지 변경을 시도했습니다. 3명의 참여자 모두 의도한 대로 '배송지 변경'으로 이동했기에 설계대로 동작한다고 판단해 테스트를 마쳤습니다.

![](/images/projects/10_addressbook/08.jpg)

<br>

#### 결과

고객이 잘 사용하고 있는지 확인하기 위해 배포 후 1개월 뒤 데이터를 살펴보았는데요.

저장 가능한 배송지수를 늘린 효과가 있는지 확인하기 위해서 배송지를 4개 이상 사용하는 고객을 확인해보았고 배송지 등록 유저 대비 `17%`인 점을 확인할 수 있었어요. 눈에 띄게 높아진 수치였죠.

기본 배송지를 잘 활용하고 있는지를 확인하기 위해서는 **배송지 추가/수정시에 기본 배송지를 설정하는 고객 비중**을 확인해보았고 추가/수정하는 고객의 `20%`가 기본 배송지를 바꿔서 설정한 부분을 확인할 수 있었어요.

기능 관련 불만 2위였던 만큼, VOC 감소도 크게 효과를 느꼈어요. 배송지 관리 기능과 함께 주문 취소 기능이 도입되었는데요. 그럼에도 취소 비율이 크게 늘지 않은 이유 중 하나로 배송지 관련 어려움이 해소되었기 때문일 거라고 회고하기도 했습니다.



#### 소감

프로덕트 디자이너로 일하면서 비즈니스 목표와 고객의 사용성 사이에서 무게추를 어디로 기울여야 할지 고민하는 순간이 종종 있는데요. 이 프로젝트는 ‘hygiene issue’[^1]를 해결하자는 큰 목표가 있었기에 평소에 가지던 부담에서 벗어나 오로지 사용성에 집중해본 시간이었습니다. Casual UT를 통해 사용성을 검증했던 과정이 특히 기억에 남습니다. 

아주 오래 묵은 voc를, 앓던 이를 제가 뽑았다는 점도 의미있었어요. 디자이너 이전에 사용자로서 저와 제 동료들 역시 불편함을 겪었던 부분이라 사용자의 입장에서 느낀 기쁨까지 뿌듯함이 배가 되었습니다.

[^1]: 위생요인 : 어떤 분야에서 자신이 경쟁하는 데 필요한 최소한의 서비스나 제품의 스펙. 필수조건. [Link](https://www.bain.com/ko/insights/hygiene-versus-wow-factors/)