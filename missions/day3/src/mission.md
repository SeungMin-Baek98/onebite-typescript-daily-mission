# Day 3 Quiz

### **_Quiz 1._**

다음 요구사항을 만족하는 4개의 타입을 정의하세요

- Any 타입은 사용할 수 없습니다.
- Nums 타입은 숫자만 담을 수 있는 배열 타입입니다.
- Colors 타입은 문자열만 담을 수 있는 배열 타입입니다.
- Coords 타입은 [숫자, 숫자] 형태의 배열만 허용하는 타입입니다.
- Info 타입은 [숫자, 문자열] 형태의 배열만 허용하는 타입입니다.

  ```TypeScript
  type Nums = never;
  type Colors = never;
  type Coords = never;
  type Info = never;
  // 위 4개의 타입을 각각 어떻게 구현해야 할까요?
  ```

  > [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKhCgAIUhtTAsC4CMnIF0o0DejgGOsAujlAVecB2WwH07JBE8cEZBwF1XAficA5BwFLGNJARUcAz2yQVAnBXpskBaZwDYLkQIBjgW9HAGuORAJGOANTsAANZEA1A4B92wBwTgH1HIgS1XAE02ATpoCEGYOHAAXAJ4AHAKaQAcgFcAtgGdIAXkgA7VwCNbACdYVABuCxt7AGEAewAbWKCPbzdzIIBLHwBzUIirO0g4pIATFLg-F0CggBpK6vDIwoBJHwAzWK84NMycuoDgxvBQCGg4bj4hNBYcQADewAZFwBSmicARcYFBQA1V7EhAEHHAHVXIQEqxwBHmwB0OyEBBycBECchADCGuDcATochAEVXGSEAx0cBWoYMAOhYOFJiPg5IpVIABycALl0TGoyBSQQAR44Aeceh0h4gFDxgzGaCmcAZFzWJLmSAAb0gAFEAI5OACG8Vh5IAHnYAMbmWEOWLmACCPkskAAvpA2kFYi5IAAiAACBVsAFoWQALOnxWw5WxuYBOcwZeJuCURcAs2I+NK+AbJABcjlc5VgAEZYQAmWEAZlhABZYQBWRrG03E42JK1FBJJO0SoK2EoS2ES7JRtWxyX+eJOWwSv0ms3G0pZGnmDXW4pBMpdWDuyC+iL+s1ZDrW1odcsSwAu41xABpryadAHYhrLICyaW4NeWoBTmbY2QAeTk8vmz22QAA+oeDHlXJbLq6bsQAfHuauOmazzNOqbT4ov3LD6sFQgej5AJ6fz9S6dO4uvYT0srlUI+x6TjOF4flubiwrAd61OaVSDIBz4nlOZ6gVeu6Qb+fSwQ0B7gI0QA)

#

### **_Quiz 2._**

다음 요구사항을 만족하는 **Course 타입**을 정의하세요
<br>
(이 타입은 마치 **인프런**에서 활용할 것 같군요?)

- Any 타입은 사용할 수 없습니다.
- Course 타입은 온라인 강의 정보를 포함하는 객체 타입을 정의합니다.
- 문자열을 저장하는 name 프로퍼티를 가져야 합니다.
- 숫자를 저장하는 price 프로퍼티를 가져야 합니다.
- 숫자를 저장하는 student_cnt 프로퍼티를 가져야 합니다.
- 문자열을 저장하는 author 프로퍼티를 가져야 합니다.
- 문자열 배열을 저장하는 related_courses 프로퍼티를 가져야 합니다.
  ```TypeScript
  type Course = never;
  // Course 타입을 어떻게 구현해야 할까요?
  ```
  > [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKhCgAIUhtTAsC4CMnIF0o0DejgGOsAujlAVecB2WwH07JBE8cEZBwF1XAficA5BwFLGNJARUcAz2yQVAnBXpskBaZwDYLkQIBjgW9HAGuORAJGOANTsAANZEA1A4B92wBwTgH1HIgS1XAE02ATpoCEGYOHAAXAJ4AHAKaQAwgHsArgCcAzvYC8kAN5QkAB2AIYAtrYAXB7mbgCWQQDmANyB1vEAxlFBLmEARrZuqZCQMS4AJrZB5gD6GdWROfmFxZAhLuYAFk5u0bEJKYFutgA2Iea25XWunrYeffFJsKipAL6p4KAQ0HDcfEJoLDiAAb2ADIuAKU17gCLjAoKAGqvYkIAg44A6q5CAlWOAI82AOh2QgIOTgEQJyCADCGuHdACdDkEAIquMSCAMdHAK1DBgAdCwOFJiPg5IpVIABycALl17AA0MgUkEAEeOAHnHCdIeIBQ8YMxmgpjiYWsPXM-kgAFEAI4uEIjEncgAedgy5hJADknOYAIJBSyQVaQABmbicYUgACIAAJWOwAWgynUFIyqiTmwA6cRGHm1GwyTiCMUgTvcXkijhmXkgvgCJVCES92redMggmwv0AGeMqQCcXZdAAMLdMAJUOCQC9nYAOpe1RLSmSikAArIWAAxl3MlMqVap1BqQACMJYAHABOCttDrdXo6wAu41xABprkAAPpAAOoJCZuEZOJzlHNDUbjSbTD1zL2wQIlUOQcORmPxy6AGs7AIaj2fbW8An2OQQAgq4ADDszgBXR0jPN6ABPHACg9aazkEA1TOQQAeNYAMuPziUqC5usZgGvYAAqczmA4IReB4fpwIEoriuYAA8MryoqmHOKuAB8hHtuhtgSphm48vygqYQA1rYlhOKq3qriS2pBrY2rDjq6RxFk3EjtqVZVLU9TmIJOrtF0PSSdqwxjBMUzurM9qEYEJFoWK5FYXyAojPhPq2LAHHhFxYGlP0STEaR2kUXptEEbMJl8QJFlNAUbg2VpGGYQ5BlOV4JkiTW4nau5uSed5JRkfZNEBUZJnSV24UkjEiyJNFPJ2bp8WGauJkKUuylGfaFnpQMyzEeAKzgEAA)

#

### **_Quiz 3._**

다음 요구사항을 만족하는 User 타입을 구현하세요

- Any 타입은 사용할 수 없습니다.
- 객체 타입이어야 합니다.
- String 타입의 name 프로퍼티가 있어야 합니다.
- String 타입의 email 프로퍼티가 있어야 합니다.
- 그 외의 String **타입의 동적 프로퍼티들도 추가**할 수 있어야 합니다.

  ```TypeScript
  type User = never;
  // User 타입을 어떻게 구현해야 할까요?
  ```

  > [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKhCgAIUhtTAsC4CMnIF0o0DejgGOsAujlAVecB2WwH07JBE8cEZBwF1XAficA5BwFLGNJARUcAz2yQVAnBXpskBaZwDYLkQIBjgW9HAGuORAJGOANTsAANZEA1A4B92wBwTgH1HIgS1XAE02ATpoCEGYOHAAXAJ4AHAKaQAqgGdbAJ0gBeSAG8okAHYAhgC2tgBcTuauAJb+AOYA3H62wYHRADYRUbGJfrAA1raWWTHxqJBhkJGluQC+SeCgENBw3HxCaCw4gAG9gAyLgClNbYAi4wKCgBqr2JCAIOOAOquQgJVjgCPNgDodkICDk4CIE5CAGENcY4AnQ5CAIquMkIBjo4CtQwYAdCwcUsT4coqqgAOTgC5dbQA0MgqQgBHjgB5xz7SHiAUPGDMZoKYAMYAe38kUgAFcXK5Ks43J4fH4gqFKgAiABScIAFv4CV9kqkMoSAFZk-wAAVsAA8QtZ0rZrvDgpTkqyooEAIyE8y2SL8yCQNlCgBMhLicLhABN+fVwEA)
