# Day 7 Quiz

### **_Quiz 1._**

다음 요구사항을 만족하도록 introduce 함수의 매개변수의 타입을 정의하세요

- name 매개변수는 String 타입이며, "이정환" 이라는 기본값이 설정됩니다.
- tall 매개변수는 Number 타입이며, 선택적 매개변수 입니다.

  ```TypeScript
  function introduce(name, tall) {
    if (!tall) {
      console.log(`안녕하세요 ${name}입니다!`);
    } else {
      console.log(`안녕하세요 ${name}입니다. 키는 ${tall}입니다`);
    }
  }
  ```

  > [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquAjzYLodUAlgHYAuATgPYAmAVwDGAUyiALVcAYQ4A1xqIBPO5IAGemVEADC4FDxioFQJ6bUAcg3jABaKGwCGAWzELlgFKaoAZW7sA5mvWAXccAOXQBooAIg8tQA01-ygPQB92+0AGOsAPnsAkGo8oQBJBrUBKFsAJpswAOmMoDjMAG0L5JUl7ADkBCwAjES53bz9AAkHAXYXAQAnS5Sh1LNyQYDAwUCgIAEUBFgAvNChAEVHADPbZQBV5wB2WwB9OqEARMcBGQcAXVahAEjHADU7NuEAHGv08KAGwADMBNiEOFh42Vk5eQVEACnMrABcAGdnGw3ABeAJBUJ+ArFAD8ALY1TqXAAlFAAN5gKCsO5QH4AQjhhQx2NxuKEbyBPEKImyhR4Lh+AANABKjgFVGq5QAAkmP+IgAvr1MISWWiANw4qCCqAiQpAsTkilUtg0ukMpmszncvkC4V9KCAEoX7HySQbMOKpbjBWBbcMQKMACoiEGzQA3o9FAAG9gAZF+xaQCvTRRAC0zgBsF2jRKCAEHHADqrUEAlWP0QA6HVBJFpaIAByaggClRwCtQ1kboN2Nx+MIRD9JWBi18yz9AiF-JXq6XfvWYVAAIwAdgArJWgA)

#

### **_Quiz 2._**

함수 타입 표현식을 이용해 다음 요구사항을 만족하는 타입 Func를 정의하세요

- 2개의 매개변수 a와 b를 받습니다.
- 매개변수 a는 Number, b는 String 타입입니다.
- 반환값 타입은 boolean 입니다.

  ```TypeScript
  type Func = any;
  ```

  > [Quiz Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yAtVwGENUAMLgoeNSA6K4CBrgu0OAi41IC7jglWOAuq1ICdNgMuNSApY4Da1gNQOC2q9UAznYEcJwBqrgFKb8RAGIBXAHYBjQD6dUQKgTgDXHRgDkGOYALRQATMg1RAJ53JAAz24AhoAExqACNVgbB7ArUOAJpuYA6Axes7SQA5WQBbJwBTACcAGmdJAGUAF2iAS3kAcykCbz9DQAwewA01wCQaqUABcecAeyqAG0jbeShc3zAQYDAwUCgIAEVZNIAvNChAEVHADPazQBV5wB2W1UARMcBGQaZAEjHADU7VOEAHGp0OKHawZIBPAAdIqDklKABeKAAKWwAueXCouOdHgGdUjMyAShuAD5qnUGvIANydboQAAqkW+I0AN6OABjrAAG9gAZFyRqQCvTdRAC0zgBsF0TIqCAEHHADqrUDogBHmwA6HVBsGpRIAByaggClRrzMfYdRRVeTfKAAMwUikeFxFN3utniTgB12BAG8wFAoLz+aCfLUqpkHj5klVpGkAB6RAAmdz+f0hKrVnw1Wp1Tj1VQAMlVFLZ6m6AO4xADCtk+kQtVuVUGikWSsmiTVSskikIAvpCwGkwicqtFklAFVAAKIAR1knvieaNZ0UyXiwSqyQAgvIjlBE0LolUwlAAEQAAWOZ30igAFp76ll4cBZMk0rVPp2U33znDvgGg59JRAw2WK8kADw1+uNneXRSAwGxTflyKVneF4u1HcABVs0VsYUjMU+R5FgIgAAY0PELwRDEp7niqW5Xrut6eo+z6vu+0SfseP4AIwAVA3zpFkp5gGgkJAA)
