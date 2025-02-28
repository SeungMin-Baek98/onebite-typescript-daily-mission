# Day 11 Quiz

### **_Quiz 1._**

다음 요구사항을 만족하는 3개의 인터페이스를 정의하세요

1. Content Interface
   - name(String 타입), info(T 타입) 프로퍼티를 갖습니다.
2. Video Interface
   - playTime(Number 타입) 프로퍼티를 갖습니다.
3. Book Interface

   - pageNumber(Number 타입) 프로퍼티를 갖습니다.

```TypeScript
  interface Video {}

  interface Book {}

  interface Content {}
```

> [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVAMzKAa41IB7jgDIuAZy4C7jgEqHAPp1RAqBOtagDkG8YAIwA6KAGEA9gDsALgFNNUAJKatAJwBmAQwDGWsFCgBaKGrMBbLQAoAyhqMBLNQHMoQAGFwFDxgEoAGig-ExU3ABVg8KhAEFXAHQ7AH2XAB6WRQDQawFahwAmmzHkwACZFADUfABMtFX1DU0trWwcABwAbMwBPeJ9XNwA5AFdnACNjJLDUzJyoAuLFMCZFACEVFQBrRu1mqxt7KHazfy1RieNhscmjadnsvKKSsBBgMDBQKAgARRGfABeaCggBFRwAZ7exACrzgB2WkSADCHRFI8FA3h8-HtzFYoNU6g0AN6HLq9fquKAALkcN2MYAAvmimpitFANtsoATbCczhdbuTKZcjABuWn0jEtZTqbSaAA88QAfGzDk5SRSAM7ePz+IW2GINCnxYWfEDfeJaNXAwA3o4AGOsAAb1cRiiQCvTRRAC0zgBsF2iWqCAEHHADqrUEAlWOAEea0lAEbRAAOTUEAUqPPFHvEwjNQWDQ+dRQADuZg0FgAFjj6m4LBKdBoKapDNL8ypZTN2VAi2oVSpOlp5J0VP43AADAAkeIbko08h18iJfQGWhpgB2hwAgNexAKg1rBEU8AtTOAC1Wu2EhXSwAmkym00YtGYaiytoXi5oy5eNFKzzWFbYG02W22O92+wOS8O1LFR6dzipIwaUAGNr2EAURmKEAX3HsE3bcPkzbM81qAs6yVLQKQAIj9EIoFdS0Q0ADPHAB92wBOLsYUIBFdQBezsADqXMIiQ4dQpOsOW6cdXApWQAAZ5AAVkY2waUYmktw+I8TzPNw0JcDCoGwqBcPwoiyMYQAazsAQ1H6ME6JfxUFjDg5ADuWMCkAHZuO4nThNpMSgA)

#

### **_Quiz 2._**

getComments 함수의 적절한 반환값 타입을 정의 하세요

- getComments 함수는 여러개의 Comment 타입 객체를 담는 배열을 비동기적으로 반환하는 함수입니다.
- 반환값 타입이 Promise이 아닌 좀 더 정확한 타입으로 추론되게 하여도 정답으로 인정합니다.

```TypeScript
  interface Comment {
    id: number;
    author: string;
    content: string;
  }

  function getComments() {
    return new Promise((resolve) => {
      setTimeout(() => {
        resolve([
          {
            id: 1,
            author: "이정환 & 김효빈",
            content: "한입 FE 챌린지! 완강까지 화이팅!",
          },
        ]);
      }, 2000);
    });
  }
```

> [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0wHMCmAXAwgPYC2x2AdrgM5SAWq4BhDgGuNSCAE4BATgOqtSAYPYBprgSDVRAAwuBQ8cAi41ECoE80Aaq4A5BwCljYALRQcBEmUo0GgFKaogG9HAN+3JmRUhVzCRUQLg1gFpnAPp1RAL037ADD2AX0YmARPsCbzYAMdSyAPOOAOh08vDL6DCKAE02AJ00AdCoRgqKALuNQAAoATiQAllTYADwAruQA1uSEAO7kAHyZgCKjgDNNUIABE1CAKs1SgKprXKJhUIAps4AGHYAYLYAxNVAyBoAjzVKAr01DgB7jkoCWqwnJIMBgYKBQEACKpfkAXmhQTYAZ7cyAKvOAOy3O9JLyClA7YPmU2DkAZgBDADG2Cg5i0VgA3mAoFB8gATABcUHIpWIACNfgBuGFQAGlXAAC0IOWRVFwOW+mBxsKBhB+lDJFKpOIAvns-uUgbh8vS1HhwZYqAAKACUUGRuQKRWKgsoEDQ9Sg0NhOTwpRy5BR2Bq2TyxEK2GFwrVVEIABsAG7YcUAXiVKthUCKuAAKvkyIQCca7Q7cU6oKaLdbhRB-QHleGI3CkVAAIwAGijEfxRJJyIAROlJLwoAAyKCAATrABVrgAk+jNJ6MBukM3CZjg2ABiAFEoIAZGcADZ2AAcmAIRQQAiY4BUGsAMnVdqCAFTX0oBQZZ7FeTsNZlYjaFFNKdi6gACYAAy71e41n79n7ECHV3YcmXAwBQABvYAGRf0kkWEnsgBsFmQBKCAEHGuIBKsbm4QvDIY6AFKjgCtQwkHy7B6AAOJJQlAzYAI6lAC5oJohAAeMHYNyGEAHKELgyGoeaUCslAfz6lAGYAAK4AAnjhyhAoSaHmhQOBUMABL5OaVAZjiYCMThUDnuS+AAkUNC2ocuLNthuG4MUhHEShaHFAASuqmqukxJQidghB-PyGgWNo9QYVKBoygC5AMfUjlLgpOHcipREkRp2m4Bq5B6ThxSGcZplytQll6tKJTlFUtQNE58mKW5qmeeaWk6X5+mBfpwXqKFVDhdZhrFOQ2DWjkjmWQlrnKSlaU+bpmVBSZuWaEKBX6kVoUKhVYBoDiQA)
