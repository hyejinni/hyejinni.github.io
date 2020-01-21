---
layout: post
title:  검색 기능 추가하기
date:   2019-09-04 15:01:35 +0300
image:  02.jpg
tags:   Design
---
## Background

젤라또는 예쁜 네일 디자인을 찾을 수 있는 서비스입니다. 다자인을 찾는 ‘탐색’이 가장 큰 비중을 차지하는 액션임에도 원하는 디자인을 직접 ‘검색’ 할 수 없어 많은 사용자들이 불편함을 감수하고 있었는데요. 가장 많은 VOC가 있었던 만큼 오랜만의 메이저 업데이트 과제로 ‘검색 기능 추가’를 선정했습니다.

## 어떻게 쓰고 있었나요?

젤라또 서비스를 잘 모르시는 분들을 위해 간략한 설명을 드릴게요. 젤라또에서는 해시태그 (#태그)와, 몇가지 필터 기능을 통해 디자인을 분류해서 볼 수 있습니다.
기존 버전에서 원하는 디자인을 찾는 모습입니다. 유저가 __‘하트프렌치’__ 디자인을 찾고 있다고 가정해보겠습니다.

보고 싶은 태그 목록이 있다면, 일단 열심히 스크롤 하면서 __그 태그가 들어가있는 디자인을 먼저 찾아야 합니다.__ 유저들은 보고 싶은 태그가 있을때마다 이 플로우를 반복했는데, 이 과정에서 검색에 대한 많은 VOC 가 들어오게 됐습니다.

젤라또는 디자인을 분류해서 볼 수 있는 필터 기능도 제공하고 있는데요. 유저의 65프로 이상이 사용하고 있는 기능입니다. 3가지 카테고리에서 한가지씩 선택 가능하고, 선택한 항목들은 AND 조건으로 적용됩니다. 마지막 화면에서 보이는 목록은 __‘프렌치 스타일의 레드 네일’__ 입니다.


## 어디까지 검색이 가능한가요?
검색이라는 기능은 범주가 넓습니다. 네일, 예쁜네일, 여름에 하면 좋은 네일, 심지어는 이미지 검색도 검색의 범주에 포함되는데, 우리는 이중 어디까지 개발 할지를 정해야 했는데요.
다양한 논의 끝에 젤라또는 검색 기능의 오픈 스펙을 __‘#태그 검색’__ 으로 한정하기로 했습니다. 이미 가지고 있는 #태그 풀을 활용한 Start small 인 셈이죠.

예를 들어 ‘가을’이라는 태그를 검색한다면 ‘#가을’ 태그가 있는 디자인들을 볼 수 있게 되겠죠?


You lived before you met me?! Ow, my spirit! Humans dating robots is sick. __You people wonder why I'm still single?__ *It's 'cause all the fine robot sisters are dating humans!* I guess if you want children beaten, you have to do it yourself.

## Are you crazy? I can't swallow that.

Oh, I don't have time for this. I have to go and buy a single piece of fruit with a coupon and then return it, making people wait behind me while I complain. Meh. So, how 'bout them Knicks? Also Zoidberg.

1. We need rest. The spirit is willing, but the flesh is spongy and bruised.
2. Fry, we have a crate to deliver.
3. Have you ever tried just turning off the TV, sitting down with your children, and hitting them?

### Why not indeed!

Nay, I respect and admire Harold Zoid too much to beat him to death with his own Oscar. I don't 'need' to drink. I can quit anytime I want! Soothe us with sweet lies. Bender?! You stole the atom. You don't know how to do any of those.

* Shinier than yours, meatbag.
* This is the worst part. The calm before the battle.
* Ooh, name it after me!

Say what? Throw her in the brig. Hey, you add a one and two zeros to that or we walk! You guys aren't Santa! You're not even robots. How dare you lie in front of Jesus? Ow, my spirit! Who's brave enough to fly into something we all keep calling a death sphere?

Hey, you add a one and two zeros to that or we walk! You won't have time for sleeping, soldier, not with all the bed making you'll be doing. It's okay, Bender. I like cooking too. Hey, what kinda party is this? There's no booze and only one hooker.

![]({{ site.baseurl }}/images/07.jpg)
*Minimalism*
