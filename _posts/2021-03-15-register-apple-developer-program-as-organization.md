---
layout: post
title: "애플 개발자 계정: 회사 계정으로 가입하기(진행중)"
tags: 
    - ios
    - apple
---

애플 개발자 프로그램에 가입하는 과정을 다들 기록해 둔다. 나도 도움을 얻었으니 도움이 되고자 하는 용도다.

준비물: 

- **영문으로 된 사업자등록증**: 영문으로 회사 정보를 입력할 때 사용한다. 홈택스에서 발급할 수 있다고 한다.
- **대표자 생년월일**: 계정을 대표자명으로 가입할 때 사용한다. 물어 봐도 되고 통신판매등록증에서 볼 수도 있다고 한다.

## 1. 사전 개념: 내 개인 계정을 회사 계정으로 등록해도 되는가?

**아직 확신이 없다.** 다른 블로그 글들에서 보기로는 대표 이름으로 애플 아이디를 신규 발급한 뒤에 그걸로 등록(enroll)하라고 한다.

보통 회사 계정이라고 할 때는 두 가지 종류가 있다. 

예컨대 페이스북 페이지는, 페이지라는 공간이 있고 개인 계정들이 해당 페이지의 관리자가 된다. 페이지를 소유하는 주체는 "비즈니스"라는 추상물이다. 비즈니스를 만드는 것은 또 다른 절차가 있다. 이런 모델이라면 내 개인 계정으로 개발자 프로그램에 가입해도 아무 문제가 없고, 오히려 더 편하다.

반면 유튜브의 경우에는 특정한 계정이 채널을 만든다. 그리고 그 계정이 주 소유자가 되고, 다른 관리자들을 초대할 수 있다. 카카오 채널도 비슷한 모델로 보인다. 이런 모델이라면 회사 아이디를 새로 만드는 게 좋다.

애플 개발자 계정은 어디에 해당하는지 아직 모르겠다. 그래서 나는 일단 회사 계정을 따로 만들었다. 뭐가 됐든 회사 계정으로 개발자 프로그램에 등록한 다음 내 개인 아이디를 개발자로 추가하는 건 된다(개인이나 1인회사로 등록하면 이게 안 되는 것 같다).


## 2. 사전 준비: D-U-N-S 번호

회사 계정으로 가입하려면 D-U-N-S 번호가 필요하다. 두 단계를 거친다고 생각하면 된다.

1. 미리 조회를 해서 임시 번호를 받는다. [조회 사이트](https://developer.apple.com/enroll/duns-lookup/#!/search)에서 회사 정보를 영문으로 잘 쳐서 넣는다. 이메일도 정성껏 넣는다. 그러면 메일로 D-U-N-S 번호가 날아온다. 그런데 이건 임시 번호다.

2. 이메일이 오면 정식 등록 요청을 한다. 그런데 이 때 개발자 등록을 위한 계정이 있어야 한다. 따라서 1을 미리 완료해 두고, 계정을 만든 뒤 정식 등록 요청을 하자.


## 3. 아이디 발급

우선 대표자명으로 애플 아이디를 만들었다. 다른 블로그 글을 보면 보안 질문을 잘 적어 두라고 하던데, 최근에 변경된 것인지 보안 질문 같은 게 있지는 않았다. 

전화번호를 적게 돼 있는데 대표자의 전화번호가 아니라 실무자의 전화번호를 적자. 인증번호가 계속 날아온다. 거의 로그인할 때마다 날아온다고 생각하면 된다.

## 4. 개발자 계정 등록

계정을 만들었다면 [애플 개발자 사이트](https://developer.apple.com)에 가서 로그인을 한 뒤 내비게이션 우측의 Account 클릭. 그러면 개발자 계정을 만들거냐고 묻는데 하겠다고 답한다.

이후 Account를 클릭하면 아래와 같은 화면이 나오는데 Join the Apple Developer Program을 클릭한다.

![](/assets/2021/1-join-the-apple-developer-program.jpg)

그리고 우측 상단의 작은 enroll 버튼을 누른다.

![](/assets/2021/2-enroll-button-position.jpg)

이제 안내 페이지가 나온다. 맨 아래 Start Your Enrollment 버튼을 누르자.

![](/assets/2021/2-what-you-need-to-enroll.jpg)

그러면 다시 개인정보를 입력하는 칸이 나온다. 

**개인 개발자인지 회사 개발자인지 선택하는 것은 이 절차 후에 나온다.** 다른 블로그들에 있는 정보를 보면 조직인지 아닌지를 먼저 고른다고 안내돼 있는데 최근에 변경됐나 보다.

위쪽 칸은 한글로, 아래쪽 칸은 영문으로 입력한다. 네이버에서 회사 주소를 입력한 뒤 영문 주소라고 하면 영문 주소를 찾을 수 있다. ([예시: 충무로역 영문 주소](https://search.naver.com/search.naver?where=nexearch&sm=top_hty&fbm=1&ie=utf8&query=%EC%84%9C%EC%9A%B8%ED%8A%B9%EB%B3%84%EC%8B%9C+%EC%A4%91%EA%B5%AC+%ED%87%B4%EA%B3%84%EB%A1%9C+%EC%A7%80%ED%95%98199++%EC%98%81%EB%AC%B8+%EC%A3%BC%EC%86%8C)) 

기억이 좀 가물한데 여기에서 계정 주인(즉, 대표자)의 생년월일을 입력했던 것 같다.

## 5. 회사 계정 선택

위의 단계를 거치고 나면 계정의 유형을 고르는 항목이 나온다. 아래 이미지에서 볼 수 있듯이 계정에는 5가지 유형이 있다. 

- 개인/1인기업(Individual/Sole Proprietor)
- 회사/조직(Company/Organization)
- 비영리단체(Nonprofit)
- 인가받은 교육 단체(Accredited Educational Institution)
- 정부 조직(Government Organization)

원하는 대로 고르자. 단, 이 포스트에서 향후 설명은 회사/조직을 선택했을 때로 맞춘다.

아래쪽에 애플의 안내문이 있는데, 회사명이 앱스토어에 제대로 뜨려면 소재지에서 법인으로 인식돼야 한다, 개인으로 선택하면 앱스토어 개발자에 개인이름이 뜬다는 내용이다.

![](/assets/2021/3-select-yout-entity-type.jpg)

## 6. 회사 정보 등록

이제 애플이 조직 정보를 알려 달라고 한다. 아래 이미지를 참고하자.

![](/assets/2021/4-tell-us-your-organization.jpg)

Legal Entity Name에는 앞서 **"사전 준비: D-U-N-S 번호"** 단계에서 받은 이메일에 있는 회사명을 입력하자. 아마 끝이 **Co., Ltd.**로 끝나는 경우가 많은가 보다. 마지막 마침표까지 빼놓지 말고 영문으로 잘 입력해 주자. 이름이 틀려도 빨간 경고가 뜨더라.

D-U-N-S Number에는 이메일로 온 숫자를 입력해 주는데 아마도 버튼을 누르고 나면 빨간 에러가 뜰 것이다. 

> (번역) 이 조직은 법인으로 인증되지 않습니다. 개인기업이나 1인기업이라면 개인으로 등록하세요. 조직이 법인으로 나와야 한다면 [D&B 프로필을 업데이트하세요(update your D&B profile).](https://developer.apple.com/enroll/duns-update/?referralReasons=legalStatus)
> 
> (영문) This organization could not be verified as a legal entity. If you are a sole proprietorship/single person company, enroll as an individual. If this organization should be listed as a legal entity, update your D&B profile.

자, update your D&B profile을 클릭할 시간이다. 클릭하면 또 신청 페이지가 나온다(아래 이미지).

![](/assets/2021/5-update-your-d&b-profile.jpg)

신청을 완료하면 이메일이 온다. 발신자는 `iResearch@dnb.com`이다.

> 문의 접수 확인 # 0000000 - {회사명} 정보 갱신 요청.
> 
> 문의해 주셔서 감사합니다. 보내 주신 문의는 0000000번으로 할당됐습니다. 문의에 대한 처리가 완료되는 대로 이메일을 통해 알려드리겠습니다.
> 
> 일련번호: 0000000  
> 신청일시: March 15, 2021, 06:46 AM (UTC)  
> 비즈니스명: {회사명}  
> Duns: 000000000  
> 위치: Seoul Seoul KR  
> 요청자 본인 요청 키: xxxxxxxxxx  
> 관련 분류: 법적 형태 , 주요 비즈니스명  
> 
> **각 문의에 대한 처리가 완료되는 대로 각각의 알림 메일이 갈 수 있습니다. 유의해 주세요.
> 
> 감사합니다,
> D&B iResearch Team
> 
> 이 메일에 답장하지 마세요. 자동 응답 메일입니다.

아래는 영문.

> Inquiry # 0000000 Received - Update for {회사명}.
> 
> Thank you for your inquiry. Your inquiry has been assigned Tracking ID # 0000000. We will notify you through email as soon as the resolution(s) on your inquiry are complete. 
> 
> Case Number(s): 0000000  
> Submitted Date/Time: March 15, 2021, 06:46 AM (UTC)  
> Business name: {회사명}  
> Duns: 000000000  
> Location: Seoul Seoul KR  
> Requester's Own Request Key: xxxxxxxxxx  
> Concern categories: Legal Form , Primary Business Name 
> 
> **Please note that a separate notification of the results will be sent after the completion of each case.
> 
> Sincerely,
> D&B iResearch Team
> 
> Please do not respond to this message. This is a system generated email.

**여기까지가 Step 1이다.**

-----

## 7. 3일 후에 메일이 왔다

> **요청 완료 알림 # 0000000 (일련번호 # 0000000) - COMPANY CO.,LTD. 정보 갱신 요청**
> 
> (중략)
> 
> 처리: 데이터 변경 혹은 추가  
> 보조 처리: 외부 소스를 통해 확인
> 
> 처리 메모: 안녕하세요. Duns 000000000(COMPANY CO.,LTD.)이 새롭게 갱신됐습니다. 지역 데이터베이스에 적용되기까지는 24-48시간이 소요되고, 글로벌 제품에 적용되기까지는 2-3주가 걸립니다. 감사합니다.

다시 애플 개발자 사이트에 들어가서 로그인을 하고 enroll을 진행한다. 이번에는 D-U-N-S 번호를 넣었을 때 인식하게 될 것이다.

## 8. 정보를 조금만 더...

이제 Just a bit more info라고 하면서 주소를 다시 받는다. 웹사이트 주소와 사업자등록번호(Tax ID/National ID)를 입력하라고 한다.

그리고 지금 계정이 소유주/설립자(Owner/Founder)의 계정인지 대리인의 계정인지 묻는 부분이 나온다.

- 대표자 이름으로 만든 계정이다: 소유주/설립자 선택
- 내 계정이다: 대리인 선택(My organization has given me the authority to bind it to legal agreements.)

![](/assets/2021/7-just-a-bit-more-info-2.jpg)

Continue를 클릭하고 나면 한 차례 정보를 확인하라고 입력한 내용을 다시 보여주는 페이지가 나오고, 그 다음에는 신청이 됐으니 기다리라는 페이지가 나온다.

> 등록 신청이 처리중입니다. (Your enrollment is being processed.)

![](/assets/2021/9-your-enrollment-is-being-processed.jpg)

**여기까지가 Step 2다.**

다시 기다리는 중...



