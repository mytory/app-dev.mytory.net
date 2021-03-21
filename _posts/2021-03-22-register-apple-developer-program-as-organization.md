---
layout: post
title: "애플 개발자 계정: 회사 계정으로 가입하기"
tags: 
    - ios
    - apple
---

애플 개발자 프로그램에 가입하는 과정을 다들 기록해 둔다. 나도 도움을 얻었으니 도움이 되고자 하는 용도다. D-U-N-S 번호 조회 신청을 하고 이메일을 받는 것을 미리 해 놨었기 때문에 며칠 걸렸는지 기억이 나지 않는다. 1~3일 정도 걸렸던 것으로 기억한다. 이후 아래에 설명한 등록 시작을 3월 15일에 해서 3월 19일에 절차가 완료되고 20일에 결제를 했으니 총 5일만에 끝났다. 2주는 걸리는 줄 알았는데 제깍제깍 하면 그 정도로 겁먹을 필요는 없겠다. 물론 D-U-N-S가 가장 시간이 오래 걸린다. 미리 신청을 해 두자. 

준비물: 

- **영문으로 된 사업자등록증**: 영문으로 회사 정보를 입력할 때 사용한다. 홈택스에서 발급할 수 있다고 한다.
- **대표자 생년월일**: 계정을 대표자명으로 가입할 때 사용한다. 물어 봐도 되고 통신판매등록증에서 볼 수도 있다고 한다.

## 1. 사전 개념: 내 개인 계정을 회사 계정으로 등록해도 되는가?

**회사 계정으로 등록하자.** 등록 완료 후 이메일로 날아온 애플의 안내를 보니 나중에 소유권을 이전할 수 있다고 한다. 즉, 지금 등록하는 아이디가 소유자가 된다. 법인이 있고 해당 법인의 관리인 아이디를 지정하는 것이 아니라 소유자가 있는 것이다.

> {Company} CO.,LTD.의 등록이 승인되면 App Store Connect를 통해 다른 팀원을 추가 및 관리할 수 있습니다. 계정 보안을 유지하시려면 팀원들이 각자의 Apple ID를 사용하도록 하고 각 팀원에게 적절한 역할을 지정해 주십시오. **나중에 역할이 변경될 경우 계정 소유자 역할을 다른 팀원에게 이전할 수 있습니다.** (강조는 내가 한 것이다.)

보통 회사 계정이라고 할 때는 두 가지 종류가 있다. 

예컨대 페이스북 페이지는, 페이지라는 공간이 있고 개인 계정들이 해당 페이지의 관리자가 된다. 페이지를 소유하는 주체는 "비즈니스"라는 추상물이다. 비즈니스를 만드는 것은 또 다른 절차가 있다. 이런 모델이라면 내 개인 계정으로 개발자 프로그램에 가입해도 아무 문제가 없고, 오히려 더 편하다.

반면 유튜브의 경우에는 특정한 계정이 채널을 만든다. 그리고 그 계정이 주 소유자가 되고, 다른 관리자들을 초대할 수 있다. 카카오 채널도 비슷한 모델로 보인다. 이런 모델이라면 회사 아이디를 새로 만드는 게 좋다.

애플 회사 계정은 후자인 것으로 보인다. 나중에 사고 같은 것으로 관리에 난항을 겪지 않으려면 회사 계정을 만들어서 그것으로 개발 계정을 만드는 편이 좋겠다. 

나도 회사 대표 메일로 계정을 따로 만들었다. 


## 2. 사전 준비: D-U-N-S 번호

회사 계정으로 개발자 프로그램에 가입하려면 D-U-N-S 번호가 필요하다. 계정을 만들기 전에도 아래 두 단계 중 1단계는 처리할 수 있으니 미리미리 해 두자. 지금 회사에서 아이폰 앱을 만들 예정이라면 그냥 지금 곧장 1번 단계는 처리하자. 나중에 편하다. 나도 그렇게 해놔서 나중에 편해졌다.

두 단계는 아래와 같다.

1. 미리 조회를 해서 임시 번호를 받는다. [조회 사이트](https://developer.apple.com/enroll/duns-lookup/#!/search)에서 회사 정보를 영문으로 잘 쳐서 넣는다. 이메일도 정성껏 넣는다. 그러면 메일로 D-U-N-S 번호가 날아온다. 그런데 이건 임시 번호다.

2. 이메일이 오면 정식 등록 요청을 한다. 이 때는 개발자 등록을 위한 계정이 있어야 한다. 따라서 1을 미리 완료해 두고, 계정을 만든 뒤 정식 등록 요청을 하자.


## 3. 아이디 발급

우선 대표자명과 회사 메일로 애플 아이디를 만들었다. 다른 블로그 글을 보면 보안 질문을 잘 적어 두라고 하던데, 최근에 변경된 것인지 보안 질문 같은 게 있지는 않았다. 

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

## 7. 3일 후인 3월 18일에 에 메일이 왔다

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

이제 Just a bit more info라고 하면서 주소를 다시 받는다. 

물론 추가로 받는 정보도 있다. 웹사이트 주소와 사업자등록번호(Tax ID/National ID)를 입력하라고 한다. 

그리고 지금 계정이 소유주/설립자(Owner/Founder)의 계정인지 대리인의 계정인지 묻는 부분이 나온다.

- 대표자 이름으로 만든 계정이다: 소유주/설립자 선택
- 내 계정이다: 대리인 선택(My organization has given me the authority to bind it to legal agreements.)

![](/assets/2021/7-just-a-bit-more-info-2.jpg)

Continue를 클릭하고 나면 한 차례 정보를 확인하라고 입력한 내용을 다시 보여주는 페이지가 나오고, 그 다음에는 신청이 됐으니 기다리라는 페이지가 나온다.

> 등록 신청이 처리중입니다. (Your enrollment is being processed.)

![](/assets/2021/9-your-enrollment-is-being-processed.jpg)

등록을 마치면 "프로그램 등록 신청이 완료됐습니다(Your program enrollment has been received)" 하고 `developer@email.apple.com`으로부터 이메일이 온다.

**여기까지가 Step 2다.**

------

## 9. 하루 뒤에 애플코리아에서 전화가 왔다

다음날인 19일 오전 11시 40분쯤에 애플 코리아로부터 전화가 왔다. 18일 밤에 D-U-N-S 번호 입력과 함께 신청을 마쳤는데 말이다. D-U-N-S가 확실히 제일 오래 걸리나 보다. 

발신자 번호는 `080-333-4000`이었고, 수신한 번호는 계정 등록할 때 적은 번호다. 

세 가지를 물었다.

1. 회사의 영문명은 무엇인가?
2. 당신은 회사의 근무자인가?
3. 당신에게는 약관 동의 권한이 있는가?

1은 D-U-N-S 신청한 대로, 2와 3은 그냥 예라고 답하니 문제 없었다. 애플코리아 측은 "곧 약관 동의 메일이 갈 것이다. 약관에 동의하면 24시간 내 계정이 활성화된다" 하고 안내했다.

그리고 한 가지를 더 물었다. 연락이 되지 않는 경우 대체할 연락처가 있다면 알려 달라고 했다. 필수는 아니라고 했다. 회사 대표 번호를 알려 줬다.

통화 직후에 이메일이 두 통 왔다. 하나는 영어 하나는 한글.

- Apple 개발자 프로그램 지원 - 케이스 번호: 0000000000
- Continue your Apple Developer Program enrollment.

## 10. 알찬 한글 안내 메일

우선 한글 메일은 간단한 안내문이었다. 

> 안녕하세요. 조금 전 개발자님과 전화상으로 만나 뵌 Apple 개발자 프로그램 지원팀의 {이름}입니다. 신청해주신 등록신청서가 완료되었으며, 아래의 정보가 도움이 되시길 바랍니다.
> 
> Apple Developer Program은 개발자들에게 기술 리소스, 지원, 사전 공개 소프트웨어에 대한 접근 권한과 함께 iOS와 macOS를 위한 혁신적인 응용 프로그램, Safari용 확장 프로그램 및 iPod, iPhone, iPad용 액세서리를 개발하는 데 필요한 모든 것을 제공합니다.
> 
> Apple Developer Program 및 Apple Developer Enterprise Program에 대한 정보는 다음 웹 사이트에서 찾으실 수 있습니다.
> 
> [멤버십 지원](https://developer.apple.com/kr/support/membership/)  
> [Apple Developer Program](https://developer.apple.com/kr/programs/)  
> [Apple Developer Enterprise Program](https://developer.apple.com/kr/programs/enterprise/)  
> 
> 처음 시작하시는 경우 다음 리소스를 확인해 보십시오.
> 
> [Xcode 도움말](https://help.apple.com/xcode/)
> [개발자 계정 도움말](https://help.apple.com/developer-account/?lang=ko)
> [App Store Connect 도움말](https://help.apple.com/app-store-connect/?lang=ko)
> [개발 리소스](https://developer.apple.com/kr/develop/)
> [Developer Forums](https://developer.apple.com/devforums/)
> 
> 이중 인증을 사용하시려면 신뢰할 수 있는 전화번호에 언제든 접근하실 수 있어야 합니다. 개발자 계정에 접근할 수 없는 경우가 발생하지 않도록 [Apple ID 계정 페이지](https://appleid.apple.com/)의 보안 섹션에 [신뢰할 수 있는 전화번호](https://support.apple.com/ko-kr/HT204915#trusted)를 추가해 주시기 바랍니다.
> 
> [이중 인증에 대해 자세히 알아보십시오.](https://support.apple.com/ko-kr/HT204915)
> 
> {Company} CO.,LTD.의 등록이 승인되면 App Store Connect를 통해 다른 팀원을 추가 및 관리할 수 있습니다. 계정 보안을 유지하시려면 팀원들이 각자의 Apple ID를 사용하도록 하고 각 팀원에게 적절한 역할을 지정해 주십시오. 나중에 역할이 변경될 경우 [계정 소유자 역할을 다른 팀원에게 이전](https://developer.apple.com/kr/support/account-holder-transfer/)할 수 있습니다.
> 
> [팀 역할에 관하여](https://developer.apple.com/kr/support/roles/) 자세히 알아보십시오.
> 
> (후략)

꽤 알찬 정보를 메일로 보내 줬다. 특히 소유권을 넘길 수 있다고 안내해 줘서 개인 계정과 회사 계정의 관계에 대한 궁금증이 어느 정도 해소됐다.

## 11. 결제로 가는 링크를 담은 영문 메일

이제 결제를 할 시점이다. 참고로 결제로 고생하는 사람들이 있던데 나는 맥에서 파이어폭스로 결제해서 성공했다.

> 등록 신청이 승인됐습니다. 프로그램 라이센스 계약을 검토하고 조직이 애플 개발자 프로그램에 등록하는 절차를 계속하실 수 있습니다. 
> 
> [지금 검토하기 >](https://developer.apple.com/enroll)
> 
> Your enrollment request has been accepted. You may now review the Program License Agreement to continue your organization's enrollment in the Apple Developer Program. 
> 
> [Review Now >](https://developer.apple.com/enroll)

## 12. 검토하러 가면 이번에는 계약 동의 페이지가 나온다!

![](/assets/2021/10-review-and-accept.png)

계약(License Agreement)에 동의할 수밖에 없지 뭐 어떡하겠나. 하지만 그래도 좌측 상단에 있는 Download PDF 버튼을 눌러서 계약서를 다운받자. 회사의 문서 관리팀이 있다면 넘겨 주자.

체크박스의 레이블이 상당히 긴데 대충 해석하면 체크박스에 체크하고 "계속" 버튼을 누름으로써 내가 계약서를 읽었다는 것과 계약에 동의했다는 것을 확인한다. 그리고 내가 법적으로 성인이라는 것을 확인한다. 이런 내용이다.


## 13. 결제로 이동!

![](/assets/2021/11-complete-your-purchase.png)

위와 같은 페이지가 나온다. 결제 직전 확인 단계다. "일단 구입이 완료되면, 구입했음을 알리고 멤버십을 확인하는 이메일을 받게 될 것입니다" 하고 씌어 있다.

가격을 확인하고 구입(Purchase) 버튼을 누르자. 그러면 대망의 결제 페이지가 아니라(!) 로그인 화면이 뜬다. 결제 전에 한 번 해 주는 건가 보다. 로그인을 또 해준다.

로그인을 하면 결제 페이지가 뜬다?! 아니다. 결제 방법을 선택하는 페이지가 나온다. 그러나 선택지는 하나밖에 없다. "신용 카드 또는 직불 카드, 할부". 그리고 신용 카드니까 청구 주소를 입력해 줘야 한다. 주소를 몇 번 입력하는지 모르겠다. 연락처 정보도 마지막으로 한 번 더 입력해 준다.

이제 주문 검토 버튼을 누르자. 이제 결제 페이지가 나올까? 아니다. 주문 검토 페이지가 나온다. 그래도 마지막이니 이미지 한 번 보고 가자.

![](/assets/2021/14-paygate-ing.png)

이제 결제 페이지다. 카드 수기결제다(카드번호, 유효기간, 비밀번호 앞 두자리, 생년월일을 입력하면 따로 프로그램 설치 없이 결제가 되는 방식). PG사는 이니시스다. 국내카드와 해외카드가 모두 지원되는 것으로 나와 있다. 그러나 이상하게 법인카드가 먹지 않아서 나 같은 경우는 내 개인 직불카드로 결제하고 비용을 청구했다.

결제는 수월하게 진행됐다.

결제 완료 페이지는 아래와 같다. 뿌듯하다.

![](/assets/2021/16-complete.png)


## 끝이 아니다. 활성화까지 기다려야 한다.

아직 끝나지 않았다. 활성화까지 기다려야 한다. 

앱스토어 커넥트 약관 동의도 남았다. [앱스토어 커넥트](https://appstoreconnect.apple.com/)에 로그인해서 약관에 동의해 줘야 한다. 곧장 로그인했을 때는 약관 동의 페이지가 나오지 않았다. 계정 활성화까지 최대 24시간이 걸린다고 했으니 느긋이 다음날 로그인해 보자. 

(앱스토어 커넥트는 앱을 등록하고 판매를 관리하는 페이지다. 개발자 센터는 개발 관련한 인증 등을 수행하고 정보를 얻는 곳이다. 역할이 구분돼 있다.)

![](/assets/2021/23-app-store-connect-terms-of-services.png)

[애플 개발자 사이트](https://developer.apple.com) 계정도 바로 활성화되지 않는다. 내 경우는 20-30분 지나니까 됐다. 

아래 이미지는 결제 직후에 로그인한 개발자 사이트다. 구입하라는 안내 메시지가 나온다! 그러나 다행히도 우측 상단 계정명을 보면 "대기중(Pending)"이라고 씌어 있다.

![](/assets/2021/17-developer-site-after-complete.png)

느것하게 다음날 앱스토어 커넥트에 접속하자. 그러면 약관 동의가 나올 거다. 동의하면 진짜 끝난 거다.

**참고.** 약관 동의하기 전에도 사용자 추가는 할 수 있으니 서둘러 자신의 개인 애플 아이디를 [사용자로 추가](https://appstoreconnect.apple.com/access/users)해 주자. 앱 개발할 때마다 Xcode와 앱스토어 커넥트와 개발자 사이트에서 회사 아이디로 로그인하고 인증번호 받으려면 귀찮다.


## 기타 - 완료 이메일

결제를 마치면 이메일이 4통 온다.

- 이니시스의 결제 확인 메일
- 애플 스토어의 주문 승인 메일
- 애플 개발자 센터의 개발자 프로그램 환영 메일. [시작하기](https://developer.apple.com/programs/how-it-works/) 페이지로 가는 링크를 담고 있다.
- 앱스토어 커넥트에서 보내 준 메일. 애플 개발자 아이디로 앱스토어 커넥트 사이트에 로그인할 수 있다는 안내 메일이다.


## 감상

블로그 글을 보면 과정이 무시무시해 보이고, 2주는 걸릴 줄 알았는데 생각보다 빨리 됐다. 미리 걱정이 돼 준비를 많이 한 덕인 듯하다.

찾아 본 블로그 글들과 조금 다른 점들이 있었다. 예컨대 결제가 윈도우로만 된다는 글도 있었는데, 맥으로 무난히 할 수 있었다. 그것도 파이어폭스로 말이다. 여하간 이런 점들이 다른 분들에게 (2021년 3월 22일 현재) 최신 정보를 제공해 줄 수 있다면 뿌듯할 것 같다.






