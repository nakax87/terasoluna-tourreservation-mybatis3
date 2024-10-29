# データベーステーブル設計

## 出発地

| カラム名     | データ型   | サイズ | PK | FK | Not Null |
|--------------|------------|--------|----|----|----------|
| DEP_CODE     | CHAR       | 2      | Yes| No | Yes      |
| DEP_NAME     | VARCHAR    | 20     | No | No | Yes      |

## 目的地

| カラム名     | データ型   | サイズ | PK | FK | Not Null |
|--------------|------------|--------|----|----|----------|
| ARR_CODE     | CHAR       | 2      | Yes| No | Yes      |
| ARR_NAME     | VARCHAR    | 20     | No | No | Yes      |

## 宿泊施設

| カラム名     | データ型   | サイズ | PK | FK | Not Null |
|--------------|------------|--------|----|----|----------|
| ACCOM_CODE   | CHAR       | 4      | Yes| No | Yes      |
| ACCOM_NAME   | VARCHAR    | 100    | No | No | Yes      |
| ACCOM_TEL    | VARCHAR    | 13     | No | No | Yes      |

## 年令区分

| カラム名     | データ型   | サイズ | PK | FK | Not Null |
|--------------|------------|--------|----|----|----------|
| AGE_CODE     | CHAR       | 1      | Yes| No | Yes      |
| AGE_NAME     | VARCHAR    | 10     | No | No | Yes      |
| AGE_RATE     | NUMERIC    | 3,0    | No | No | Yes      |

## 社員

| カラム名     | データ型   | サイズ | PK | FK | Not Null |
|--------------|------------|--------|----|----|----------|
| STAFF_CODE   | CHAR       | 8      | Yes| No | Yes      |
| STAFF_NAME   | VARCHAR    | 100    | No | No | Yes      |
| STAFF_KANA   | VARCHAR    | 100    | No | No | Yes      |
| STAFF_PASS   | VARCHAR    | 20     | No | No | Yes      |

## 顧客

| カラム名        | データ型   | サイズ | PK | FK | Not Null |
|-----------------|------------|--------|----|----|----------|
| CUSTOMER_CODE   | CHAR       | 8      | Yes| No | Yes      |
| CUSTOMER_NAME   | VARCHAR    | 100    | No | No | Yes      |
| CUSTOMER_KANA   | VARCHAR    | 100    | No | No | Yes      |
| CUSTOMER_PASS   | VARCHAR    | 88     | No | No | Yes      |
| CUSTOMER_BIRTH  | DATE       | -      | No | No | Yes      |
| CUSTOMER_JOB    | VARCHAR    | 100    | No | No | Yes      |
| CUSTOMER_MAIL   | VARCHAR    | 300    | No | No | No       |
| CUSTOMER_TEL    | VARCHAR    | 13     | No | No | Yes      |
| CUSTOMER_POST   | VARCHAR    | 8      | No | No | Yes      |
| CUSTOMER_ADD    | VARCHAR    | 300    | No | No | Yes      |

## ツアー情報

| カラム名     | データ型   | サイズ | PK | FK | Not Null |
|--------------|------------|--------|----|----|----------|
| TOUR_CODE    | CHAR       | 10     | Yes| No | Yes      |
| PLANNED_DAY  | DATE       | -      | No | No | Yes      |
| PLAN_NO      | CHAR       | 4      | No | No | Yes      |
| TOUR_NAME    | VARCHAR    | 300    | No | No | Yes      |
| TOUR_DAYS    | NUMERIC    | 2,0    | No | No | Yes      |
| DEP_DAY      | DATE       | -      | No | No | Yes      |
| AVA_REC_MAX  | NUMERIC    | 10,0   | No | No | Yes      |
| DEP_CODE     | CHAR       | 2      | No | Yes| Yes      |
| ARR_CODE     | CHAR       | 2      | No | Yes| Yes      |
| ACCOM_CODE   | CHAR       | 4      | No | Yes| Yes      |
| BASE_PRICE   | NUMERIC    | 7,0    | No | No | Yes      |
| CONDUCTOR    | CHAR       | 1      | No | No | Yes      |
| TOUR_ABS     | VARCHAR    | 4000   | No | No | No       |

## ツアー担当者

| カラム名       | データ型   | サイズ | PK | FK | Not Null |
|----------------|------------|--------|----|----|----------|
| TOUR_CODE      | CHAR       | 10     | Yes| Yes| Yes      |
| TOUR_CON_CODE  | CHAR       | 10     | Yes| No | Yes      |
| TOUR_CON_NAME  | VARCHAR    | 100    | No | No | Yes      |
| TOUR_CON_MAIL  | VARCHAR    | 300    | No | No | Yes      |

## 予約

| カラム名        | データ型   | サイズ | PK | FK | Not Null |
|-----------------|------------|--------|----|----|----------|
| RESERVE_NO      | CHAR       | 8      | Yes| No | Yes      |
| TOUR_CODE       | CHAR       | 10     | No | Yes| Yes      |
| RESERVED_DAY    | DATE       | -      | No | No | Yes      |
| ADULT_COUNT     | NUMERIC    | 2,0    | No | No | Yes      |
| CHILD_COUNT     | NUMERIC    | 2,0    | No | No | Yes      |
| CUSTOMER_CODE   | CHAR       | 8      | No | Yes| Yes      |
| TRANSFER        | CHAR       | 1      | No | No | Yes      |
| SUM_PRICE       | NUMERIC    | 7,0    | No | No | Yes      |
| REMARKS         | VARCHAR    | 1000   | No | No | No       |
