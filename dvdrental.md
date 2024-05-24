1. 映画探索:
　要件: filmテーブルから全映画のタイトルとリリース年を取得する。
　提出物: この要件を満たすSQL文。


        SELECT title,release_year
        FROM film;


2. 指定カテゴリの映画取得:
　要件: film テーブルからrental_rateが4以上の映画のタイトルのみを取得する。
　提出物: この要件を満たすSQL文。


        SELECT title
        FROM film
        WHERE rental_rate>=4;

3. 新規顧客の追加:
　要件: customerテーブルに新しい顧客を追加する。具体的なデータ値は自由に選択してください。
　提出物: この要件を満たすSQL文。


        INSERT INTO customer (customer_id,store_id, first_name, last_name, email, address_id, activebool, create_date, last_update, active)
        VALUES (600, 1,'John', 'Dare', 'johndare@sakilacustomer.org', 1, TRUE, '2024-05-24', CURRENT_TIMESTAMP, 1);

4. 顧客情報の更新:
　要件: 顧客IDが5の顧客のメールアドレスを"updated@email.com"に変更する。
　提出物: この要件を満たすSQL文。


        UPDATE customer
        SET email='updated@email.com'
        WHERE customer_id=5;