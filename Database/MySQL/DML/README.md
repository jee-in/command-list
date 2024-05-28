## DML (Data Manipulation Language)

### 데이터 등록

```SQL
INSERT INTO {테이블 이름}({컬럼 이름}, {컬럼 이름}, {컬럼 이름})
VALUES ({값}, {값}, {값});
```
- 예시
```SQL
INSERT INTO users (id, pw)
VALUES ('jee-in', '1234');
```
- 모든 사원에 값을 입력하는 경우 컬럼명을 생략할 수 있습니다.
```SQL
INSERT INTO users
VALUES ('jee-in', '1234');
```

- 여러 레코드를 입력하는 경우 다음과 같이 작성할 수 있습니다.
```SQL
INSERT INTO users
VALUES ('jee-in', '1234'), ('ji-reong', '5678'), ('jing-jing', '0000');
```

> 주의 사항
    - 컬럼 목록과 값 목록의 개수는 반드시 일치해야 합니다.
    - 컬럼의 자료형과 값의 자료형은 반드시 일치해야 합니다.

