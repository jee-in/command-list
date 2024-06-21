## DQL (Data Query Language)

### 데이터 조회
```SQL
SELECT 컬렴명1, 컬럼명2, 컬럼명3
FROM 테이블명
WHERE 원하는 조건식;
```

- 예시
```SQL
SELECT password
FROM users
WHERE id = 'jee-in';
```
- 테이블에 있는 모든 레코드를 조회하려면 WHERE문을 생략하면 됩니다.
- 레코드의 모든 컬럼을 조회하려면 SELECT 다음에 `*`을 입력하면 됩니다.
    - 예시: `SELECT * FROM users;`
