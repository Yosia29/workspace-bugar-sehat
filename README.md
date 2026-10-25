
Bugar Sehat
------------
- DDL Database	: https://dbdiagram.io/d/GymApp-ver2-686b7ef3f413ba350894c555
- Repository	: https://github.com/idberteknologi/bugar-sehat.git
   Branch Main -> Untuk mengerjakan (development biar gk conflict atau setiap orang bisa create branch sendiri nanti bisa di merge jadi satu)
   Branch Live -> untuk publish ke server 

Source File : https://drive.google.com/drive/u/1/folders/10QmqQ34Stwsk5Q3Ayf994wQRGCCRXGv6
------------------
- template : Landing Page & Admin (atau mungkin ada masukan template yang lebih sesuai bisa d share)
- Bisnis Proses


1. Config -> running script
    - copy .env.example to .env
    - composer install
    - php artisan key:generate
    - php artisan jwt:secret -f
    - create database : bugarsehat
    - setting database env :
        DB_CONNECTION=mysql
        DB_HOST=127.0.0.1
        DB_PORT=3306
        DB_DATABASE=bugarsehat
        DB_USERNAME=sesuaikan dengan mysql yg telah di install di local
        DB_PASSWORD=sesuaikan dengan mysql yg telah di install di local
    - php artisan migrate
    - php artisan db:seed

2. Create Migrations -> DDL 
3. Create Seeder [Credential, Master, dll]
4. Authentication
5. Create Modul -> Bisnis Proses

Hasil
------------
1. Dashboard Owner
<img width="1917" height="981" alt="image" src="https://github.com/user-attachments/assets/7c4ab81b-5518-4faa-886b-4a38f2bf94a9" />

2. Scan Code QR Staff
<img width="1912" height="968" alt="image" src="https://github.com/user-attachments/assets/af1b9f69-0576-4efe-88a3-96f28b4c07fa" />

3. Laporan Transaksi
<img width="1918" height="977" alt="image" src="https://github.com/user-attachments/assets/c641c319-fcb6-4951-b9bf-80187c5428f7" />

