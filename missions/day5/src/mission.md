# Day 5 Quiz

### **_Quiz 1._**

아래 코드의 변수 a,b,c,d,e의 타입은 각각 어떻게 추론될까요?

```TypeScript
let a = 10;
const b = 20;
const c = [1, 2];
const d = [1, "hello", true];
const e = [1, 2, 3] as const;
```

> [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBFRwGe1UCrzgOy2Aa41ACzImADPYBhDUAhgDQBGDAxgwCYmADC4KHjgAuNRAgDVCogFtHA3a2AYmqiAU2cAGHYAIWwDJ1gFLGA-FChgAtFBr0SCqIAaawD81gH06oAQSh9AC6NRAqBNFALquAficAcg6t37aTI3lTSygAITteRxcPb18DVkDgqwBhCKi3Lx89Ay45IPMrABE05wzY7NoAU0SCqABREujMsBBgMDAAG0qAF3ooAF4oAEYABgBuMFYAewA7AGdepgGoACZxydmFqFZliCGGVbQJ6fnejl39qAAiAAtKjo6pq4PugCcAV0qjjdOoSouDisDgBmND0ObbTbdCZgUBQCAARXeAEsAF5ggx0HgCKCAFm7AOOjgB5xwA6HXkVBooK0wN0AJ4AB3+tkGM3eAFsmJVXjC4YiUei-FAAhFBASSWS1JoqbSGWFlmtuSB4Ui0RjaAlhXiiaSFOTJW1pf9Usy2RzXhBvrDFbyVQLcnwRVrxRSpfT-sVBgAKFnszlQAA+UAWr2RMwA5v7BVMpl06DMAJTmhVKvmqv7Yh1inUSyn6131AFA0FJiAAFUqCzBgBvRwAMdYAA3sADIuAFKbnIBXpsAIuNQQAtM4AbBcAGqvVqCAEHHADqrUEAlWOAEebSdQnL3AAOTUEAUqOAVqHABNNgBOmnNgZGsulTV69ADe9QAju86B0DnUAB4M1jdA4AOSm3WsMxpUAAvlAAGavKastcAACBo6KwNwXl0YblsA7zdMiHRzFcMIGlAZYLMkdBzOWuxgFoN53t0AA8dRnheRHWAc3qmgAfDRDB4fUt6VPeJFkR0RGhICIx0Qx+HMaxpHnhxyRUSanLmrxjEESxxFCeRhQHF64mvBGQYhuGAZMFGMbxpJ9HSQJcnsSRBx7ICIJoHRYDfEAA)

#

### **_Quiz 2._**

다음 요구사항을 만족하는 Animal, DogCat(개냥이) 타입을 완성하세요
<br>

- Animal 타입은 Dog 타입일 수도 Cat 타입일 수도 있습니다.
- DogCat 타입은 Dog이자 Cat입니다.

```TypeScript

type Dog = {
  name: string;
  color: string;
  };

type Cat = {
name: string;
age: number;
};

type Animal = never;
type DogCat = never;

```

> [Answer](https://www.typescriptlang.org/play/?strict=false&noImplicitAny=false&ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVAIIB2AlgLYCGANgDRQAIgHsA5gGEuAFwAUyQKcNgF3GAlFEADC4FDxioBExwIyDtQByDeMAFpm7bj3UbAAuNCx1wD7jUQBhDgEeaokqU9cfAEeOArUOAE02YAHSm9hLS1nYiooqACeOe0hoh4SDAYGCgUBAAigCubABeaFCAIqOAGe2AGuNQgCrzgDstgD6dUHqALqtQgCRjgBqdLXCADjWGeFAZYFIAngAOAKaRUAC8UADeYFBQLFwc0wBcUADOUgBObCyiANyrUADGwjzCh7sHx6cXAL4XY1OzXgvLlxtbR5HE7nS5cUQ7dYFDgAI2mhzeHwmM3MnF4vziUAAPskpBdkbM4j9FpiAGS4j45CAAFWmBzKgBvRwAMdYAA3sADIuMQCoE4BXpoogBaZwA2C7QmVBACDjgB1VqCASrG3IAdDtcnNogAHJqCAKVHgpgRpkbiwDlAuBZeHtdqw0TwIGVFhBLis1msAZCAESAAsXAJLdikdfEuaxudweUEdMMOwgA7ixPZdXl61ra7Q7do7AChTgA-uiN2-UQ3YARgADNGoFGwGgPjq9QATMReXZE6KLWPxgMKD358GQgBM+d99wTgA05wARk4BJgYj7zAQA)
