# Day 8 Quiz

### **_Quiz 1._**

다음 요구사항을 만족하는 구현 시그니쳐를 완성하세요(매개변수 타입만 정의하면 됩니다)

- 이미 작성되어 있는 3개의 오버로드 시그니쳐를 모두 만족해야 합니다.
- a, b, c의 값을 모두 더한 값을 반환합니다.
- 만약 매개변수의 값이 undefined일 경우 모두 0으로 취급합니다.

  - a가 없을 경우 : 0
  - b가 없을 경우 : 0
  - c가 없을 경우 : 0

  ```TypeScript
  function add(): number;
  function add(a: number): number;
  function add(a: number, b: number, c: number): number;
  ```

  > [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVAYCBrUgO0OAftYBNNgCzOA+nVEAiY4EZB2oA5BvAApAJ53JAAz2AMIaiABhcCh45SiBUCcAa47UAuXVECULV0wBKMAFoogF3HAH91RAiePDAGC2AW0aiAI8cYBmZNqiAJGOAIT2AOh2AOy3s3PxQgBVdgAotVNSALquAPqNQgJarJgB0llAAhgA0UABGRQDG-oBINRTxUIAqzYA6q1DVUIAYPYAaa5mYOVaUgL6jULKKVdZQAK4AdgAmAKYAZgCWEzNTgD7jUIC9NYANY7EJAAyAPOMhUIAXs4CQdV05UFBWeYAANVCAY6MU21AAXFB7YNdWxQ-Pmx2Hy+PygZX+LyBnzAIGAYDAc0mZQALgsAPYTfJTKaSUwfCZjAC2xRmACcANwIpGojFYnF5fFEkmkvFQAnEsmUxETFHozF5bGSBlsplkorFRkc0nlSXM1ns5mUsCgKAQACKYwWAC80ExWJxeAIROI8FBYVSeTT+YK8gB+N4KsUle2O6Vgl2illQADe3ygpJmyLGpMxQqgtttn1MUAA1FBJMVw5G9tG45Iykmo5SAL5gIA)

#

### **_Quiz 2._**

다음 요구사항을 만족하도록 사용자 정의 **타입 가드**를 완성하세요

- isGuest 함수가 true를 반환하면 매개변수로 전달된 user는 Guest 타입임이 보장됩니다.
- isMember 함수가 true를 반환하면 매개변수로 전달된 user는 Member 타입임이 보장됩니다.

  ```TypeScript
  type Guest = {
    visitCount: number;
  };

  type Member = {
    id: string;
  };

  type User = Guest | Member;

  function isGuest(user: User) {}

  function isMember(user: User) {}
  ```

  > [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquAjzYLodURglWOAJ41IKgTgGuNSADC4FDxqIAAawDstgH06ogETHAjIO1AHIN4wAWigBLAM4BxAK4BTTQBcogC1XAGEMioRgE4GpgDB7AGmu1ALl1RAJ53JAAz3nAOh1QgCATgDdNgDgtULqa+jaAKU1QeoYmQoAh44Au41CALz2ApeOAlC2AE02YAHSqGpoAsvoAtgBG0WaW1nb6ji7uXr4BIeGR0XEVNXUp6dn5RWAgwGBgoFAQAIq66gBeaCwc3HxC4lJyingAFEJQ5lxQABoAlFATYEYAngAO+vEGxlAAvFAA3mBQUABuWnURgAwgB7XQAOyMAC4oJDdAMbABuMAAX1Rt0ez36tRsH2+vw0ABM4cYbOpIQBzVEYqb3J5QACqUXxnwSbwAPlBcdFMQAzKEAYyM6jBkNKHKM+x6NjhLOiFzhstKL0Sfx+fxs+iMuhsEplrKgAENNGrjBdCoDNMDwVCTABCd6fKHE-T8yn6YnoqaCyEisUSrS8myG6Ly1lXZVGrQ8qp4wlanV6g0q01xpGW9TEqBOl2Qt0eyFen3TECzAAqiVWgBvRwAMdYAA3sADItxLiAV6aKIAWmcANgu0OtQQAg44AdVagrHoAROtEAA5NQQBSo4BWoYK10mYD9AfFGkhgKM+gVodlEcViY0-Kg+y0UrDNguV01fygQvFmjBABt9IUX2CqfsAAYAEi+WUrSBUEIWhNFAAiewAPyagQBKHpgQQCh-C5UT+NEoH0F8ohPM9g3jaIrxvY8-kfSFnzfD8v1-ACgOzNFAA2mqBAAlRwBVRr2B1kNQqA0R9IA)

### **_Quiz 3._**

다음 조건을 만족하는 3가지 인터페이스를 추가로 구현하세요

- 모든 인터페이스는 Person 인터페이스를 확장합니다(extends).
  1. Student 인터페이스는 grade 프로퍼티를 갖습니다.
  - grade 프로퍼티에는 "A", "B", "C"만 저장할 수 있습니다.
  2. Developer 인터페이스는 skills 프로퍼티를 갖습니다.
  - skills 프로퍼티에는 문자열 배열을 저장할 수 있습니다.
  3.  Boss 인터페이스는 company 프로퍼티를 갖습니다.
  - company 프로퍼티에는 문자열을 저장할 수 있습니다.
  ```TypeScript
  interface Person {
  name: string;
  }
  ```
  > [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUA4TgLjWAi41IDOdgjhOAaq4ClNUAzIAA1gA5NSAe44AyLgGcuAu44CVDgPp1RAKbMNAOh1RANrWAQNcqAOQcApY2AC0UQBVdgA5a2XPrQAKAUwBOAZwD2AOy08BUQKprgUvHAlquAJpswAKfQA8ALvvMATYwBKADowKCgARhCoAGVvAFd-P28rHSgAc0MAQ2SoQBBV0UAfZcAHpcFANBrAVqHXGPCIqBUs3P0C4pLABdHaACIAQS6AGigugCEBoYBhLtIoQAAJ+0ADVahADCGoQAjx6swwiIAmGIARfQA3fQAbUwAHIzTeWmMAawBLE5PjVtKKja36lXunl7eOrQYIAE8cAL6NQQAMPaCSHNFit1jU6nQYsNTMZXhxrLQAMamAC252y5gAngCPoj6g0oLiCUTSYVSp1YGCYQtlmtPmAQMAwGBQFAIABFBIPABeaCggBqBwCVY8CoIBUCcAGuNQQADC4BQ8YYgB2WwSAETHAIyDcnkbnVy3lUAAGkEoNywA9zL5DAAzbLYloGEwWKAAbzq5myeP0AC4oMZvIY7RkANxgAC+vLtDudrriiWS9qgXl8AVe7rMlh9ESayWDvS6UAAPkNRhWJl1Y-H7UYky0DsczpdDBmfH5AlBc56CyHHs9jMHQ+HzBkIBg47bG06XS1Ueiu1ne-383UaYSSWOwxH6-yIAAVfShiWAG9HAAx1gADe9i0eWAV6aSIAWmcANguUK9QQAg44AdVag0qACPN4hLPKlAsIAUqMbNaPIPASpiGKkXpQAAogAjgk2QnIMKGeJc2LeIMABypjeD0JJQDGUCOoY+JDAAAt4xKXEo2IABZYScfgZGewAJN4TzGF00ZgLi5ihiGqYpMG8RJCkUAALzer6-pBkM3DyoAGmsDHURZqaW-SxtGYkSckbYXEYwatqcFmdkpg5+gGJYadphkRL8I7BhAXQAEr6C63hjF0x7MfosTYuG5yBWghkxsZFgSQARmio5QMurz2SpTnqVpOkRNudIlr+apQLwgA5S4AKK2ACRjOlxbyTGXFAp6huM2TGGeikCnUuH4d4AA86GYScfWyWm3jeXpXQxUMfQ1iMZaVl0kwAHzLW5qF4foBEDRhWF9dZ7ZGN5HkvFNgzjhG06retPVbf1g17el3kFSSZ2SROGSrWAaDRkAA)
