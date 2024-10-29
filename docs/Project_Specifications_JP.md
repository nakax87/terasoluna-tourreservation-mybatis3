# プロジェクト仕様書

## 目次
1. プロジェクトの全体構造を理解する
2. サブプロジェクトを理解する
   2.1 サブプロジェクトのパッケージ構造
   2.2 ���ブプロジェクトのアーキテクチャ
   2.3 サブプロジェクトが使用しているDBテーブル構造
   2.4 サブプロジェクトの共通機能
   2.5 サブプロジェクトの機能解説

## 1. プロジェクトの全体構造を理解する
このプロジェクトは、TERASOLUNA Server Framework for Java (5.x) を使用して構築されたツアー予約アプリケーションです。プロジェクトは以下のサブプロジェクトで構成されています。

- terasoluna-tourreservation-env
- terasoluna-tourreservation-domain
- terasoluna-tourreservation-web
- terasoluna-tourreservation-initdb
- terasoluna-tourreservation-selenium

## 2. サブプロジェクトを理解する

### 2.1 サブプロジェクトのパッケージ構造
各サブプロジェクトのパッケージ構造は以下の通りです。

- terasoluna-tourreservation-env
  - 環境依存の設定ファイルを含むプロジェクト
- terasoluna-tourreservation-domain
  - ドメイン層のロジックを含むプロジェクト
- terasoluna-tourreservation-web
  - Web層のロジックを含むプロジェクト
- terasoluna-tourreservation-initdb
  - データベースの初期化スクリプトを含むプロジェクト
- terasoluna-tourreservation-selenium
  - Selenium テストを含むプロジェクト

### 2.2 サブプロジェクトのアーキテクチャ
各サブプロジェクトのアーキテクチャは以下の通りです。

- terasoluna-tourreservation-env
  - 環境依存の設定ファイルを管理し、他のサブプロジェクトで使用される設定を提供します。
- terasoluna-tourreservation-domain
  - ドメイン層のロジックを実装し、ビジネスルールやデータアクセスを担当します。
- terasoluna-tourreservation-web
  - Web層のロジックを実装し、ユーザーインターフェースやコントローラーを担当します。
- terasoluna-tourreservation-initdb
  - データベースの初期化スクリプトを提供し、データベースのセットアップを行います。
- terasoluna-tourreservation-selenium
  - Selenium テストを実行し、アプリケーションの自動化テストを行います。

### 2.3 サブプロジェクトが使用しているDBテーブル構造
各サブプロジェクトが使用しているDBテーブル構造は以下の通りです。

- DEPARTURE
- ARRIVAL
- ACCOMMODATION
- AGE
- EMPLOYEE
- CUSTOMER
- TOURINFO
- TOURCON
- RESERVE

### 2.4 サブプロジェクトの共通機能
各サブプロジェクトの共通機能は以下の通りです。

- ログイン機能
- 予約機能
- 顧客管理機能
- ツアー情報管理機能
- レポート生成機能

### 2.5 サブプロジェクトの機能解説
各サブプロジェクトの機能解説は以下の通りです。

- terasoluna-tourreservation-env
  - 環境依存の設定ファイルを管理し、他のサブプロジェクトで使用される設定を提供します。
- terasoluna-tourreservation-domain
  - ドメイン層のロジックを実装し、ビジネスルールやデータアクセスを担当します。
- terasoluna-tourreservation-web
  - Web層のロジックを実装し、ユーザーインターフェースやコントローラーを担当します。
- terasoluna-tourreservation-initdb
  - データベースの初期化スクリプトを提供し、データベースのセットアップを行います。
- terasoluna-tourreservation-selenium
  - Selenium テストを実行し、アプリケーションの自動化テストを行います。
