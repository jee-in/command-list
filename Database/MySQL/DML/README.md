## DML (Data Manipulation Language)

### 데이터 등록

```SQL
INSERT INTO 테이블명 (컬럼명1, 컬럼명2, 컬럼명3)
VALUES (값1, 값2, 값3);
```
- 예시
```SQL
INSERT INTO users (id, pw)
VALUES ('jee-in', '1234');
```
- 모든 컬럼에 값을 입력하는 경우 컬럼명을 생략할 수 있습니다.
```SQL
INSERT INTO users
VALUES ('jee-in', '1234');
```

- 여러 레코드를 등록하는 경우 다음과 같이 작성할 수 있습니다.
```SQL
INSERT INTO users
VALUES ('jee-in', '1234'), ('ji-reong', '5678'), ('jing-jing', '0000');
```

> 주의 사항
 - 컬럼 목록과 값 목록의 개수는 반드시 일치해야 합니다.
 - 컬럼의 자료형과 값의 자료형은 반드시 일치해야 합니다.

### 데이터 수정
```SQL
UPDATE 테이블명 SET 컬럼명 = 새로운 값
WHERE 원하는 조건식;
```
- 예시
```SQL
UPDATE users set password = '9999'
WHERE id = 'jee-in';
```
- 테이블에 있는 모든 레코드의 컬럼 값을 변경하려면 WHERE문을 생략하면 됩니다.
```SQL
UPDATE users set password = '9999';
```

### 데이터 삭제
```SQL
DELETE FROM 테이블명
WHERE 원하는 조건식;
```
- 예시
```SQL
DELETE FROM users
WHERE id = 'jee-in';
```
- 테이블에 있는 모든 레코드를 삭제하려면 WHERE문을 생략하면 됩니다.
```SQL
DELETE FROM users;
```
