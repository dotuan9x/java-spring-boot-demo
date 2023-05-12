# Java for children

## Install

Sử dụng maven để cài các packages sử dụng trong project

```shell
./mvnw install
```

**Trong project sử dụng docker để cài đặt các service cần thiết như:**
- **MySQL**

Tạo file `.env` chứa các cấu hình với nội dung sau:

```text
MYSQL_VERSION=latest
MYSQL_HOST=localhost
MYSQL_DATABASE=tuando
MYSQL_ROOT_PASSWORD=tuando
MYSQL_USER=tuando
MYSQL_PASSWORD=tuando
```

Tạo thư mục `data` để chứa dữ liệu `mysql` sau khi start.

Lưu ý: chmod thư mục data có quyền ghi dữ liệu.

```shell
chmod -R 777 data
```

Sau đó, start docker container, sử dụng command line sau:

```shell
docker-compose up -d
```

## Start 
Start project bằng câu lệnh sau

```shell
./mvnw spring-boot:run
```