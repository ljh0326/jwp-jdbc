# JDBC 라이브러리 구현
## 진행 방법
* 프레임워크 구현에 대한 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

## Step 1 - REST API 및 테스트 리팩토링
- 요구사항 1. HTML 이외에 JSON으로 데이터를 요청하고 응답을 받도록 지원해야 한다.
    - `core.mvc.JsonViewTest`의 모든 테스트를 pass하도록 JsonView를 구현한다.
    - `next.controller.UserAcceptanceTest` 테스트를 pass하도록 Controller를 추가한다. Controller는 애노테이션 기반 MVC를 사용한다.
        - @ResponseBody 애노테이션 구현하기
