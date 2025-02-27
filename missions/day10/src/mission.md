# Day 10 Quiz

### **_Quiz 1._**

다음 요구사항을 만족하는 func 함수의 타입을 정의하세요

- func 함수는 매개변수를 그대로 반환하는 함수입니다.
- 매개변수 value에는 모든 타입의 값이 들어올 수 있습니다.
- 반환값의 타입은 매개변수로 전달된 값의 타입과 같습니다.

  - ex) value의 값이 1일 경우 반환값은 number 타입입니다.
  - ex) value의 값이 'hi'일 경우 반환값은 string 타입입니다.
  - ex) value의 값이 [1,2]일 경우 반환값은 number[] 타입입니다.

  ```TypeScript
  function func(value: any) {
  return value;
  }
  ```

  > [Quiz Answer](https://www.typescriptlang.org/play/?ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVAGYCuAdgMZSAWq4BhDgGuNRAAwuBQ8YqBUCf61AHIN4wAWmbsufRoBPO5IAGe3oB9OqIA-awADNgHQ6ogDB7AGmsMevEYAmmzADoFUDdqgA3AIYAbFgFNABdHGQAquwAOW4RFBQCQawBdxqEATlsAW0cAaMaheKEAI8cBWoYdnRUtowVFAAXHXLV5TQBAJwBumwBwWqCLIwB+aqEBMGtynMCgoRX8ADwBKT18AmPiARkAfcahAXprABrHzC2iythYAWwAjfwAnSPsunr6hkb9-cagAcgALAEtLmYWllagAZwAXHdu2AHN9vO6vSgA2G3jOFwgEwANAAmNCPRaFVYbbY7CBof5dEDAMBgUBQCAARRYtwAXhjACKjgAz2wSAFXnADstel44hkeCg2LArE471uAHs2EpOAAeAAqAD4ABRggIALigIsGcpFUAA3oCdv53iwdgLpf4ANxgAC+uPxEBF-g+GMAN6OABjrAAG9gAZFxjiQCvTRRAC0zgBsF2i2qCAEHHADqrUEAlWOAEebTMzaIAByaggClRzrsnFgW7rAAOvJ271VUAAogBHFi+KF5-pp-wcd4lgByvPeAEE2ABPKBG5g7XnrKAAIgAAu8m+X5Bxrr4fP5fpbgCweT5Xt3DWAOPyPlB3hwJnK1ltdlAALyCjgSiaDQ3Ltir9cwuUfL6-feHiXd67+Hw+Xnd09LlfZ9cAZjlTZeV5ccvAFA8uSPT4AigLxXigICQP8MCv3PS8OAAFi3FFdnRB9IIlSESxhEs-zQL8wAHct5Utd4AGE4MtB8IEBXMywrd4hVrBtmyFAAFLwdi8dZNV2V4hSo-xeSYQ8xQgAAGNAxTFEtgGAKBAGqZwAInsAD8moEAGGXAB92wAP7sdQAAGtg5tIniClAAWmqBAGCa1j2MrIUCyLHwJMHKSZPXaEoG3VFlKhZzy1c9zfC88tpLXDgSLeT5vh+YLQo4tzC0iySYv-EtENAtgUp6Niws4iLPKy3zMJLQLcKUsUwDQQ0gA)

#

### **_Quiz 2._**

다음 요구사항을 만족하는 getLastValue 함수의 타입을 정의하세요

- getLastValue 함수는 매개변수로 배열을 받아 배열의 마지막 값을 반환하는 함수입니다.
- 매개변수 data에는 빈 배열을 제외한 모든 배열이 들어올 수 있습니다.
- 반환값의 타입은 매개변수 data 배열의 마지막 요소의 타입이어야 합니다.

  - ex) data 배열의 값이 [1, "hello"] 일 경우 반환값은 string 타입입니다.
  - ex) data 배열의 값이 ["hello", 1] 일 경우 반환값은 number 타입입니다.

  ```TypeScript
  function getLastValue(data: any) {
    return data[data.length - 1];
  }
  ```

  > [Quiz Answer](https://www.typescriptlang.org/play/?ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVAOYCmALgDICGAzmwGpcANgFcWUQBargDCHAGuNRAAwuBQ8YqBUCZm1AHIN4wAWmbtufQaPHTGgE87kgAZ6pgHQ6ogBh7AL6MVA2D2ARUcdO5gCc7AA5OAk51QgEg1FIAYPYAaawySUoqAE02YAHS6UJY2UAAmXGxcgAujjIASfV4UcIAeY4A6q1CAFV2ABy1egC7jUIAnLYAto4A0Y1BSUIAR44CtQwnJepHBckqAAuOp1l1ZOV6+gfiIo4r1LYA+o1CAlqsDYFBQeiwAHgCUmdlccyGNEACMADRQAEQAFixCQgD2j2hQgD7jUIBemsADWNQYYTPgAJwAlgA7JgKRTxJK7fZQI6nGYXZxyYLXF5vT6PB43H7-YGgiLBCYwkQAWwARiwIQikckQMAwGBQFAIABFERQgBeP3cgAz2uSAFXnADstgB9OzoqTR4KDssAAMxEMIAxmwoR8YfpOLwBMIxAAeAAqAD4ABSYgBcEESTq4MIAnndzWhjnbzVAAN4oiHsEQQ-WYiCYxJCFhwtjPVEkgDcYAAvpzuRBzSw+D9ADejgAY6wABvYAGRcYKkAr00UQAtM4AbBdo+aggBBxyqASrHACPN9ikCr8UEAUqP9TDKjmavV8KBcO1QSGw+EAXgNhmNJmttweACYHo8AMzfY7Jkcwsf0yf0j4faMuqDz1iGowmlgr+5QDdQNgQsRe5NgKG0gAOHwhNh-SgABRABHERhAeEDDl-FhtQeAA5D42AAQTdKAUygVUIQ+WkngAATYV04J0TVnmEaM4WzYARB1IQeEeL8DzHNhNRuK8FyNYwxEfYlPzAFigLYtdOJvRceIfVcnjXXd91HYTNS3MSDG4+8+Nfd8WAEoTX01AAWFTbyXXjpI1DIWFVWEWAyASwGIuCoCzPgAGFeGzTiIBRGC4O1U1kLQt1TQABS4CEuFpdgmR4U0HJYD5VS4u8TEtCAAAY0EtS0HmAYAoEAapnAAiewAPyagQAYZcAH3bAA-u4tAAAa8cMKURp3EABaaoEAYJrvNg+C2FNcDIKEWKSPixK2KfGkGSZLK7i63zev64QhrghK9Jfac4Wm2aer6iDFrila2K3B5T3PFgXU2vYfO2hbBv20aDIeczLOsjIsrANBkyAA)

#

### **_Quiz 3._**

다음 요구사항을 만족하는 map 함수의 타입을 구현하세요

- map 함수는 자바스크립트 배열 메서드 map을 본따 만든 함수입니다.
- 2개의 매개변수 arr과 callback을 받습니다.
- arr 배열의 모든 요소에 callback 함수를 수행한 결과를 배열로 모아 반환합니다.

  ```TypeScript
  function map(arr, callback) {
    let result = [];
    for (let i = 0; i < arr.length; i++) {
      result.push(callback(arr[i]));
    }
    return result;
  }
  ```

  > [Quiz Answer](https://www.typescriptlang.org/play/?ts=5.1.6#code/PQKgUA2gBIHN2DgTVAxg4HBqoF0yBOmwMuNUCljgNrWA1A4LargIuNSAznYI4TgGquApTVALYCGADlIBargGEOAa41IAGFwKHjFAoBA12oA5BvGAC0zdl26NACeOAUHsAlQ4BsFwL2dgDqWogBh7AL6NRAKl2AcQcA7LQrYVAHz2AGVqqADlqVDAE02YAdHKgAmZH5AE87kQAGe7igWACdowB+aqABjFgAbFIAjFkSAawpAbB7AVqGvX3kY6KNjfkAKrrc8REAF0aTUjKzspUAfTqhuQEjVwB1VqEAGmrjOk0AdDqgqwBFRqEAMHsANNcBLVeKwEGAwMFAoCABFAFcASwAvNChJwAz2-kAVeatO7kBUCak8KFWwADNdgDtEgBd9gHsPrYADwAFQANABVAB8AAoygAuEEQNBgpppTI5eFQGH7b4AUyYUCxIIAlFAALxQqAQklYiHIqAAbzAUCgKTx3yg0TxAGddilOeStmgANwsqCvP7lGHszn7ClQAAMIqg8qBUVi3nZHwA5t8ABYq-YAamNZOZrNZ3L5Au8bF2PP1MOS6NacNiEH2aBJJLFrIAvuLud9dtFAdb+d8xYGNiAtiDed8ToAb0cADHWAAN7AAyLjDugFemiiAFpmtLRU1BACDj-UAlWOAEebxvdaIAByaggClRoqYZ5rfZMNhSzmMqAAUQAjrtUqiBwAPNh4n6ogByf2+AEEPgBPKD+iXRP6EgBEAAFvqvp7JEvrmnjdbzgLtfikebuxYkATzOd9EgBGLEfXZMdJ46IGSFVg2BhCAP1RfxUQAZhRbFcQJMlKVVfEmF9MBnw+V8oHffwsVfaJ9l1IDbDAiCAhguCcVQpCqQQphvG+P4AGVvkI3UYR9MUwCPacoATV8AGEWB5XkFQgcVJ2nH4gQXZc1yBAAFGIWCYDkAJ5IFeLxP5XlsKEIEVNAoShMFJKnGdvlkxcV1XJSVLU-Fok07TdP08DjNM8zpKs4dRxSLTjx0vT33In8-wA5ETLM1kpMsoE-NSQLpzc3DUQIoidSiqEwFFMAgA)
