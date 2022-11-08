## Cài đặt MS SQL Server trên Docker


Từ dòng lệnh vào thư mục MSSQL tải về, gõ lệnh 
sau để tạo và chạy container MS SQL Server (2017)

```
docker-compose up -d
```

MS SQL Server chạy với thông tin:

- container name: sqlserver-xtlab

- port: 1433

- user: sa

- password: Password123
- Địa chỉ Server kết nối là địa chỉ IP máy host:
```127.0.0.1``` hoặc ```localhost```

## Phục hồi dữ liệu mẫu
```
docker exec sqlserver-xtlab /var/opt/mssql/backup/restore.sh
```
Tên CSDL: xtlab
