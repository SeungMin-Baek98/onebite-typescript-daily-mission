# Day 12 Quiz

### **_Quiz 1._**

다음 요구사항을 만족하도록 getSellersFromProducts 함수의 매개변수와 반환값 타입을 정의하세요

- getSellersFromProducts 함수는 매개변수로 받은 Product 배열로부터, seller 객체만 추출해 새로운 배열로 반환하는 함수입니다.

- 반환값을 명시적으로 설정해야 합니다 (인덱스드 엑세스 타입)

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

function getSellersFromProducts(products: any): any {
  return products.map((product) => product.seller);
}
```

> [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquAjzYLodUA5gKYAuAymwDa9sATgGcAYoID2AWwAKkgCYBXAMYdhUQBargDCHAGuNRAJ53JAAz1bAAmNRAGD2ANNcBINVEADC4FDxioFQJnbUAcg3jABaVpx5+ITFJWQUVNU0tQBSmg2MtQB0OqEBsHsABcag5CSVVKEAGHsAX0YTAAN7ABkWAGihhPgFBKEBcGsAWmcooQBTZwBzZwBdVqEAJgYTAFrG8wssrWljtR0AJpswAOl9hmwpAUK7AHaHAQAnAHnGkwBJBlw7AH1GoQEtVqagACkAPccBHZsASocAdlqhARdGPa4dHAEowEGAwMFAoCAAiooAJYALzQUEAIqOADPa9IAVedugB9OqBaFyePBQL4-YEAOw4QgAZgBDZRsDLhHIAbzAUCgwPkAC4oDjFFIAEZCADcNOZRKkbCZwg4glxLG5tIADiLSUyWeyuTyqkFBEzqbTafTZayOYJxeqcXyBZVhaK9bTlNIJUScQBPQUmnFinkAX25zp+BMUONUwIkOP83GqwXE0ky2TUpylWQiwiZYYiEDQbzjFI4EAAREqaum0ImoGqoIJOIpBP6o+HhNMpESJadI6m3lAALwAPig5Yi0yzQjebp+fwgABU2EKIYAb0cADHWlWIuQCvTRQGoAbBdoE6ggBBxwA6q1BAJVj9CSqNogAHJqCAKVHAK1DJyxwKkEokgg4+agAFEAI6KIm8CpPgAeErYOWdKACVCKB0wAAQ4G0-x8ZQAAsPwER0R2ARQOGBXhhHTbkwEgv8oGHIUAGEiSqdQm3+Hkfz-VQAB5X3fXgaJkIlBENfERBo3C2AkAkA0CGoQlDVNhBbCAAAY0AqeNVETFsWzKSjf3-Dg6LfD8aIAJWLUtBygthOL0ni+KDEQQzCaNVBEqTUwzbtBBzWSWzANBuSAA)

#

### **_Quiz 2._**

다음 조건을 만족하는 3개의 타입을 추가로 정의하세요

- PartialProduct 타입은 Product 타입의 모든 프로퍼티를 다 선택적 프로퍼티로 바꾼 타입입니다.

- ReadonlyProduct 타입은 Product 타입의 모든 프로퍼티를 다 읽기 전용 프로퍼티로 바꾼 타입입니다.

- ReadonlyPartialProduct 타입은 Product 타입의 모든 프로퍼티를 다 선택적, 읽기 전용 프로퍼티로 바꾼 타입입니다.

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

type PartialProduct = any;

type ReadonlyProduct = any;

type ReadonlyPartialProduct = any;
```

> [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUA4TgLjWAi41IDOdgjhOAaq4ClNUAzMoBrjUgAwuCh4yYCmzgADWA6HVIFQJxpUAcg4BSxsAFooABQCGAJwAuASzkAbGQoD2AEwCuAYyWs2gAXHZOg8dPNAFV2ADlqiAQVd6AfZcAPS4B9OqJiiACQcBdhcBACZd3D35AFB7AHvrTNkAJpswAOikoACUAUzldbQA7dQBPLT0jE3YLYusytnsnV08fP0BfccAGOqhAEAnASrGwzyjY9gTk1MzsvML5ZTVNK1LTCpmbdlqe718AkIAaKFaO7vqIqBi4xJSQYDAwUCgIAEV9FQAvNChAEVHADPbmQBV5wB2Wn0AMIYEojEUDOYBUuSUGQUADM5IYMpYSjYAN5gKBQFS6ABcUFy+gAtgAjKEAbjRuLk+IyOIAzkoFOCAOZk9EABwZ8JxeKJpPJNIy6nUUJxqPR6MxXIJxIULLFuUp1KgdIZuWZ5PRhm0+NZclyBVp9KZsoAvmTjRclAVWQiJqoNJVZgBeKCi64AawyBQxuSgHoK2mhiKqaAA-DiHcYIH6MKaLVaESMcvkigsTM7XQosknCu7Pd7fZ6A0HSs9w6mo56Y3Hreks2Mioo7dMkWmXeTM6Nk7mveCC-7AxGlKGyy2KwUq5cQNcACoZOnPQA3oy1AAG9gAZF2gCQCvTSRAC0zgBsFyhtQAg44AdVagnUAI838AGUQADk1BAFKjgFahxIg84qbXaZQuqAAUQAjvoGhbL+AAe1rGFsABy2hKABQHqFAxpQNCOj4lAABEAAClrWpIhgABYaEKqpzsA+iqOoNIYWSYC4Qis50gAwnI-I0lAzoQOSYEQUoAA88EaHxtpTIOWwiUJg4AHwyRs3HgRkxgCYBQmJvWYm1p2hTCamMlSXJ6I8Yp-GCeofFqcmEnNlUWwWdpVk6S2elSWAaBkkAA)

#

### **_Quiz 3._**

다음 조건을 만족하는 Score 타입을 구현하세요

- Score 타입은 점수를 나타내기 위한 문자열 타입으로 '0부터 10까지의 정수-0부터 10까지의 정수'형식을 갖습니다.
  - ex) "1-0", "3-2", "0-4" 이런 형태의 문자열 타입입니다.
  - ex) 어느쪽의 점수에도 두 자리수는 올 수 없습니다.

```TypeScript
type Score = any;
```

> [Quiz Answer](https://www.typescriptlang.org/play/?ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUA4TgLjWAi41IDOdgjhOAaq4ClNUAygMYD2ATgKZSADC4KHjJgNrWAQNcqAOQcApY2AC09Zuy7dAAuNRACBOAMIcA+nVEAZDZ0AtDYAY6qIBBxwDqrsQAnjgF9G5gHnHAOh1QA5ABIA3gAZAAb2AGRagBGN4AydYADk4Aa41CAqBMqAL4Srp4+-sFhkVEOgKhrgLtDJIBoNYCtQ4ATTZgOYFBQUmwAHgCUUABEvhJutQA0dQDMEgBMLXVuEgAstVCALuOAD+1QaYA7C2EwlnLchQB0JWVQlTWALaOACU2AvVNhqoALo4AjzVCACi1QZoA1nSq0gDRjUCpQgGOjBZjLIMBgYKBQEACKAFcAJYALzQUEAIqOADPawoAVecAOy0aFThESiKAfMAAFwAngAHDgAOQBAFsAEZsFgAXigbgAPr5aZ1aW1af1aQBWWkANlpAHZaQAOWkATnpbi+OPx0lYHGpAANXESyRSYoqSeSWFE5V8fhAACpsADOmPBgBvRvTeWjhQCvTSRAC0zgBsFygGExQQCVY0d7MjKEEoIApUde6M+QOJuNYmKgLigAFEAI4AgCGABtWtGKviGJjU+m2Jm05i2AA7AAmhuzGcxADFk4aOFEoAAzFhMYl1AACkrYEgYAAtk0miwBzI3AAGYoFJw21ADcX2YheNUExDF8UGp9WFjRnYHni+XnTXdXZEl8vm3u4jy7ah9qm7Ps4vS4Y-RvnQkAvPTAXl4Y7JvvK6bcsTxDgDWNABhBNa0NQ8IBWNMK2rSc2AAHgQ3NMXzItSxQxgZVaTsmAbJ9fAAPlI5p4JzTMkNrNDqMwioCxLQ1cJkNgCJAoin06cjKNKdDM3oissJYtj8KXLjiKvPiqIrYSMNEnC8PYTj8W45d+lkgSGIUvMmOw1iVI4yT1Ok39yLANBZyAA)
