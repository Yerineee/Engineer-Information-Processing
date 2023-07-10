#### 1. 상품(PRODUCT) 테이블에서 가격(PRICE)이 50000보다 크거나 같고 80000보다 작거나 같은 튜플 조회

```sql
SELECT *
FROM PRODUCT
WHERE PRICE BETWEEN 50000 AND 80000;
```
<br />

#### 2. 상품(PRODUCT) 테이블에서 가격(PRICE)이 40000 또는 50000 또는 60000인 튜플 조회

```sql
SELECT *
FROM PRODUCT
WHERE PRICE IN(40000, 50000, 60000);
```
<br />

#### 3. 상품(PRODUCT) 테이블에서 이름(NAME)이 ‘정보’로 시작되는 튜플 조회 ⭐⭐⭐

```sql
SELECT *
FROM PRODUCT
WHERE NAME LIKE '정보%';
```
<br />

#### 4. 첫 번째 문자가 ‘A’ 또는 ‘B’ 또는 ‘C’ 또는 ‘D’인 문자열과 일치하는 문자열 검색 ⭐⭐⭐

```sql
SELECT *
FROM PRODUCT
WHERE NAME LIKE '[ABCD]%';
```
<br />

#### 5. 상품 (PRODUCT) 테이블에서 가격(PRICE)이 NULL 값인 경우의 튜플 조회

```sql
SELECT *
FROM PRODUCT
WHERE PRICE IS NULL;
```
