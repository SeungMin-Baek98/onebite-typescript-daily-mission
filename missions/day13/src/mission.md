# Day 13 Quiz

### **_Quiz 1._**

다음 요구사항을 만족하는 IsProductKey 타입을 완성하세요

- IsProductKey 타입은 조건부 타입으로 다음 조건에 따라 각각 다른 타입으로 결정됩니다.
  - T가 Product의 key(프로퍼티 이름)중 하나일 경우 결과는 true 타입이 됩니다.
  - T가 Product의 key(프로퍼티 이름)중 하나가 아닐 경우 결과는 false 타입이 됩니다.
  - 예를 들면 다음과 같습니다.
    - ex) IsProductKey<"id"> 타입은 true 타입이 됩니다.
    - ex) IsProductKey<"author"> 타입은 false 타입이 됩니다.

```TypeScript
interface Product {
  id: number;
  name: string;
  price: number;
  seller: {
    id: number;
    name: string;
    company: string;
  };
}

type IsProductKey<T> = any;
```

> [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVAJIDOACgE4D2AJgK4BjAC4BpAKYBPADwAVAHxRAAwuBQ8YqARMcCMg7UAcg3jABaZu279h4iUuWABcaiAHCcAuNYADey4B5xwDodUHHfuAF0aiAGVsAfdqhAQBqQz0APTtcPQAaawFQJwEoWwAmmzAA6MCgoQxlAABqoTl5BIUANcagAa0kACkAQVbdAH2XAB6WoQBdxwBDOgEpAREmoWkAMhsAfcahAXprABrGoGMAfmsYhDj4xS2aoZLSMrKhc-JMi0oqJGvqmtq6e3rzAEVHABabhscnGADMAQwAbFnmVReX0zMNACDHAH06oIATlsALl2ebATKCATBrAK1DKS+mTWYgAHu0jAVTKJJFIAEQASx42IUKhsMzmCyWcNW3ygyNRrHRRXMOIefCEAAsuBxCZYbI8Xm9lB9KSBgGAwKAoBAAIp8XEALzQUDOgAz20qAFXnADstAMAGENxHR4KAisC4gB2QjEHEeAnmDOEUAA3qt8QAuKAmvgAWwARhaANyrE0PD1iV0sGamgDm-syAAcOLjra73d6-atXk8nhbXY6EVAXW7PT6ONGEYHg6Hwyao1SoAIuB6Yw8TRIK-GqyWAL7+jtioQSGPzelbMxY+RQAC86xpSPNJp4LHKki4d02hTtAH4oKT5q6+a9-eKQJKZGIw4rADejgAY6xyABkXGHFAK9NFEALTOAGwXaJeoIAQccAOqtQQCVY4AI80eLqtCAAOTUCAFKjsKYIaoq4g2nJCA6UAAKIAI58M8AA0aFIgOdodlAdzcB6UDYgAAn2A76AIbLPJmVansArK4i82IHtR8wnmGADCDyvAuk4QKsqH4WIwhSBhWFPFIQ5rpi0h4gSci4duciqaJ4mSdJzxycYClMtiZZiISamzGIGnYVpBFCFJmF6fJGJGSy7KcmZxHPK8Vk2RJdm6bJTmMli2IAO6muaHBPFwvAeXullyGAaD+kAA)

#

### **_Quiz 2._**

다음 조건을 만족하는 Extract<T, U> 타입을 구현하세요

- Extract<T, U> 타입은 T로부터 U만 추출하는 타입입니다.
  - ex) Extract<string | boolean, boolean>은 boolean 타입이 됩니다.
  - ex) Extract<number | string, string>은 string 타입이 됩니다.

```TypeScript
type Extract<T, U> = any;
```

> [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUA4TgLjWAi41IDOdgjhOAaq4ClNUAogB4AuATgIYDGTAPACoA0UAKoA+KIAGFwKHjJQDa1gEDXKgDkHAKWNgAtPWbsufQaImTAAuNRegHQ7AAb2AGReGkogFNnAObM0DkwBNNmAHRgoUDQFMGAEpNVk4eAGdWAEsAOwBzKAAfKAAjAHs0gBs-NhjBdKycmJFjAuzcg0AXcahAShb3Lx9-IJDtHhiAVwBbFL8WJKhIlli4wUHhkoHo+Kra+rAwAApAGPXADqXAXg3AQp2oQFQawA1xqEBESahAQcnARAmoeWdGDkz2gBM-A33ADB7AAGbAH3bAA5qoQF2BwEAawAuq4AXnpUAEJAmAQMB5qAoBAAIrtKIALzQUEAIqOADPb9oAVecAOy2AH06oIAMIcAqBNKZRQKFgJgATwADo9GKEdAJhGIALwmKABJh+GJ3cLCKAAfm5AC4oDE-AA3XoAbhhIDhvD8kTRgBvRwAMdVZaKTAK9NJEALTOAGwXKFqoIAQccAOqtQQCVY4AR5tMJPJgAHJqCAKVHAK1D7ip0KinXpaRYTCgAG96ABHdpsTKCRiMrhQAC+UAAZiw0p0oAAiAACdMZag4AAtY9l4mrgO0mFFMuEc4qaQzHqrIgBhNjhNVQLkQbyaRM8OjR2PcZmtbhjabJDrdXqjKZxESLobxEQrgcJvw6EcxzLjrRhKdL-pznosQTn3orqVdC8bsBoRVAA)

#

### **_Quiz 3._**

배열 타입의 요소를 추출하는 InferArrayType 타입을 구현하세요

```TypeScript
type InferArrayType<T> = any;
```

> [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yAYewL6NUAMLgoeOAa41ICljigPp1SAps4DmzgGquApTVAJIB2AZgKYBOAgjx4BDAJ4AVEQAcuAHjEA+fAUAi41EA2tYBA1+oA5B0mBDAwYUFAgBFAK4BLAF5oogEVHAGe0lAKvOAdlqqAMIcCoEztJQBmAALlJcrJy8AsLiYXKKALxQYlBcAB7BXGwAJgDOUAAUVpE8UABKAJQQ9gD85VAAXFBsXABuvMYgpmJcucH2gDejgAx1gAG9gAyLzD6Ar02qgC0zgDYL9ENQgCDjgDqrUICVY4AjzYA6HVC+9IADk1CAUqOArUOAE02AJ02BhlYAtpIA9jzBUADeUACiadIAxsEADQ-ACOFiEABsoABfKAcHjPB5QABEAAFQtIALT-AAWUMhWQA5r1gBZglZIbkUQBuIz-Z5sPpQISCACMUCSEDZIIATCCAMxoOkMpnvVk8Xmc0wo3FcSGQ54okEoh4iNhCB5cZWogDuxUyPEVz2yKOFYFFzIlAul3JBwR4Fi4KtxVjNdJCYWSvWCAGEhLlerawFAfn8uICZN9wVCZOxuPxBKIJNIZJiuM8OCz2fIQWwLA8AEa8eS5kNhgHBKMxyFxkrRZNxdOZ7OS3NQPo8YpE0tA8u-SvViG1+NRJOxVPNrPW9v5ou8KAAHw7Du7S6gheez0JQjYpbA5qAA)
