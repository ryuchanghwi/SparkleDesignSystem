

# 프로젝트 소개
- 연인 간 미션 승부를 통한 소원권 내기 서비스 앱의 디자인 시스템

🔗 [앱 다운로드 링크](https://apps.apple.com/kr/app/sparkle-%EC%8A%A4%ED%8C%8C%ED%81%B4-%EC%97%B0%EC%95%A0%EC%97%90-%EC%83%88%EB%A1%9C%EC%9A%B4-%EC%A7%9C%EB%A6%BF%ED%95%A8%EC%9D%B4-%ED%95%84%EC%9A%94%ED%95%A0%EB%95%8C/id6451497605)



<img src="https://github.com/ryuchanghwi/swiftAlgorithim/assets/78063938/72d6e048-adea-4e08-9f1b-96735acdcfd4" width=150></img>&nbsp;&nbsp;<img src="https://github.com/ryuchanghwi/swiftAlgorithim/assets/78063938/0f823165-d0ac-4764-9d2a-7c5d94397974" width=150></img>&nbsp;&nbsp;<img src="https://github.com/ryuchanghwi/swiftAlgorithim/assets/78063938/01f09ef6-94b3-499d-a201-c35003988225" width=150></img>&nbsp;&nbsp;<img src="https://github.com/ryuchanghwi/swiftAlgorithim/assets/78063938/c167a1b6-3b9f-46a5-a8eb-be59614469ac" width=150></img>&nbsp;&nbsp;<img src="https://github.com/ryuchanghwi/swiftAlgorithim/assets/78063938/74bebcea-5770-43bc-adca-52b69c8e583b" width=150></img>

- 진행 기간
    - 개발 : 2023.07 ~ 2023.12(진행중)
- 출시
    - 1.0.0 : 2023.12.11
    - 1.0.1 : 2023.12.22(타이머, 로그인 수정)
- 기술 스택
    - iOS : UIKit, SwiftUI, Combine, SwiftLint 
    - Deployment Target : iOS 15.0

# Trouble Shooting
### 확장성 있는 디자인 시스템을 위한 고민
- 처음 디자인 시스템을 구축할 때 
# 주요 화면 및 기능
### NavigationView(SwiftUI)
<img src="https://github.com/U-is-Ni-in-Korea/iOS-United/assets/78063938/5a8fb04d-c05a-4d9d-bf6d-7b6fb0c98363" width=150></img>


<img src="https://github.com/U-is-Ni-in-Korea/iOS-United/assets/78063938/81ee1f5a-06fd-4f49-8f75-a0b13b3d7b80" width=150></img>&nbsp;&nbsp;
``` swift
public enum SDSNavigationStyle {
    case leftTitleRightDismissButton(title: String, dismissImage: Image, action: () -> Void)
    case leftPopButtonMiddleTitle(title: String, action: () -> Void)
    case titleRightDismissButton(title: String, dismissImage: Image, action: () -> Void)
    case leftPopButtonMiddleTitleRightDismissButton(title: String, dismissImage: Image, popAction: () -> Void, dismissAction: () -> Void)
    case leftPopButtonMiddleTitleRightCustomButton(title: String, customButtonTitle: String, popAction: () -> Void, dismissAction: () -> Void)
}
```
``` swift
public struct SDSNavigationView: View {
    let style: SDSNavigationStyle
    public init(style: SDSNavigationStyle) {
        self.style = style
    }
    public var body: some View {
        switch style {
            // 디자인 시스템 코드
        }
    }
}

```
# Todo
- 기존에 있던 디자인 시스템을 확장성을 고려하여 수정할 계획입니다.
- 기회가 된다면 UIKit과 SwiftUI를 따로 분리하지 만들지 않고 한 번에 해결할 수 있는 방법을 연구해보고 싶습니다. 
# Commit message

```swift
🔨[FIX] : 버그, 오류 해결
➕[ADD] : Feat 이외의 부수적인 코드 추가, 라이브러리 추가, 새로운 파일 생성 시
✨[FEAT] : 새로운 기능 구현
✅[CHORE] : 코드 수정, 내부 파일 수정
⚰️[DEL] : 쓸모없는 파일,코드 삭제
♻️[REFACTOR] : 전면 수정이 있을 때 사용합니다
🔀[MERGE]: 다른브렌치를 merge 할 때 사용합니다.
```
