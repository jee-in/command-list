## DDL (Data Definition Language)

### 데이터베이스 생성
```SQL
CREATE DATABASE 데이터베이스 이름;
```
- 예시
```SQL
CREATE DATABASE project;
```

### 테이블 생성
```SQL
CREATE TABLE 테이블 이름 {
    컬럼 이름 자료형 제약 조건,
    컬럼 이름 자료형 제약 조건
};
```
- 예시
```SQL
CREATE TABLE users {
    id VARCHAR(10) PRIMARY KEY, 
    pw VARCHAR(10) NOT NULL
};
```
