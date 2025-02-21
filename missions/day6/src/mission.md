# Day 6 Quiz

### **_Quiz 1._**

타입 단언을 이용해 person 변수에 빈 객체를 할당하세요
(힌트. 초과 프로퍼티 검사 방지를 위한 타입 단언)

```TypeScript
  type Person = {
    name: string;
    age: number;
  };

  let person: Person = {};
```

> [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yAGFwoeNUBdNgHaOAi41IC7jglWOAuq1AA4CmATgM4D2AdlIAM9gGEOALo1IAk+qIFwawC0zgH06ogA1XAn02ANVcAcg4BSxsAApAMeuAOpYB0UQBCzgH5qogEFXAOh2AfZcAPS1EABNYBqBqIEoewAOTkwCDjgHVWoOfAQCUYCDAYGAALgCe9FAACoysHAC8UADeYFBQbACGALZ0AFxQTKEMAJZsAOYA3GlQmeX5GQCu2QBGjNUAvtVgADZ0obRx7AWxzOxQSckdtUwxQ2yVQA)

#

### **_Quiz 2._**

타입 단언을 이용해 함수 호출에서의 오류를 해결하세요
(힌트. const 단언)

```TypeScript
  let value = 10;
  giveMe10(value);

  function giveMe10(value: 10) {
    return value;
  }
```

> [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yAGFwoeNUBdNgHaOAi41IC7jglWOAuq1IBargGENSAca4DmzgC6OA4g4BrjUgJGOAanYB9OqJUANNYA1VwByDgFLGwACkAx64A6lgHRQAxgHsAdgGcALvgIBKMCGBgwAGwCmBgG4BDSwFdrUALxQAjAAYoDnXVtfQBuMABzAEs7awBZa19ZRxdrIzCwUCgIABVrfTQoQBvRwAY6wADewAZFwBSmqEBUCcBXppJAFpnAGwWxYqhAEHHAHVWockAR5sAdDqg6GrFAAcmoQClRwFahwAmmwBOmqDMwADNnLTU9SO0oKJj4xOTXAC5vHyMoAG8wKCgAJ1tnO60oI+swgF8wIA)

### **_Quiz 3._**

다음 요구사항을 만족하는 코드를 작성하세요
<br>

- CompanyMember 타입을 Boss와 Employee의 서로소 유니온 타입으로 정의하세요.

```TypeScript

  type Boss = {
    car: string;
  };

  type Employee = {
    salary: number;
  };

  type CompanyMember = Employee | Boss;
```

> [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6&ssl=13&ssc=18&pln=12&pc=1#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVICrzgOy2A+nVIInjgjIO2Acg3jABaKAGEA9gFsADgEMAdgE8AsgFNJAI1UAnKIAGFwKHjFAELiAzmcACY1ACiMgDbjFq1YA1xqIBxBwDodiKIAJxwAmmwAox-QNAHnGvKEBUCdd+QRBgMDBQKAgARQBXAEsALzQoQBFRwAz291YOQBEx7kAXVahAEjHADU6OOEAHGrioBLAAF0VpVShTCygAXigAbzAoKG7eqAAuKAAiAbMFgG4JqABjWW15s07tLPkAc3WAX3Wunr67aUdnPpHxyenVeYXb+5c1jbNZex2inm8gymh050urzEUjkSjUYN0I0+ThcUAAPv1zGZLikIAAVVT7fKAG9HAAx1gADewAMi4wooBXpoogBaZwA2C7RSVBACDjgB1VqCASrHACPNkUAGENRWiAAcmoIApUcArUMBTDtRIAMwy8k2nSy4nkU0JnQAFJsYQoVOotLtoTJDfCTQBKMYbLIKqB6g1w406AB0UKGXsWywWNueky2GrM4nsqjdjmOOoWREApeOADaaoIAENqggAoZqCAFB7ABf1cveABog+aXQi3dttFb1pMzlBVPYzH17Y79UWjSXPd6Pg4Uao-bbA0H5CGwxHxFGFgVAIOTfKggBWxwCQdYABcbmiwLzdhrZNbr+AO0igrGzOYEPQA)
