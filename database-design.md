# Physical Database Design Document

## Age Table

| Column Name | Data Type | PK | FK | Column Size |
|-------------|-----------|----|----|-------------|
| age_code    | VARCHAR   | Yes| No | 10          |
| age_name    | VARCHAR   | No | No | 50          |
| age_rate    | INTEGER   | No | No | -           |

## Customer Table

| Column Name    | Data Type | PK | FK | Column Size |
|----------------|-----------|----|----|-------------|
| customer_code  | VARCHAR   | Yes| No | 8           |
| customer_name  | VARCHAR   | No | No | 100         |
| customer_kana  | VARCHAR   | No | No | 100         |
| customer_pass  | VARCHAR   | No | No | 100         |
| customer_birth | DATE      | No | No | -           |
| customer_job   | VARCHAR   | No | No | 100         |
| customer_mail  | VARCHAR   | No | No | 100         |
| customer_tel   | VARCHAR   | No | No | 20          |
| customer_post  | VARCHAR   | No | No | 10          |
| customer_add   | VARCHAR   | No | No | 200         |

## Reserve Table

| Column Name    | Data Type | PK | FK | Column Size |
|----------------|-----------|----|----|-------------|
| reserve_no     | VARCHAR   | Yes| No | 8           |
| tour_code      | VARCHAR   | No | Yes| 8           |
| reserved_day   | DATE      | No | No | -           |
| adult_count    | INTEGER   | No | No | -           |
| child_count    | INTEGER   | No | No | -           |
| customer_code  | VARCHAR   | No | Yes| 8           |
| transfer       | VARCHAR   | No | No | 1           |
| sum_price      | INTEGER   | No | No | -           |
| remarks        | VARCHAR   | No | No | 200         |

## TourInfo Table

| Column Name    | Data Type | PK | FK | Column Size |
|----------------|-----------|----|----|-------------|
| tour_code      | VARCHAR   | Yes| No | 8           |
| planned_day    | DATE      | No | No | -           |
| plan_no        | VARCHAR   | No | No | 8           |
| tour_name      | VARCHAR   | No | No | 100         |
| tour_days      | INTEGER   | No | No | -           |
| dep_day        | DATE      | No | No | -           |
| ava_rec_max    | INTEGER   | No | No | -           |
| dep_code       | VARCHAR   | No | Yes| 8           |
| arr_code       | VARCHAR   | No | Yes| 8           |
| accom_code     | VARCHAR   | No | Yes| 8           |
| base_price     | INTEGER   | No | No | -           |
| conductor      | VARCHAR   | No | No | 1           |
| tour_abs       | VARCHAR   | No | No | 200         |
