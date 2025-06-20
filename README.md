# ETL Pipeline với Airflow, PostgreSQL và Docker

## Mô tả dự án

Dự án này xây dựng một pipeline ETL sử dụng Apache Airflow để tự động hóa quá trình:
- Trích xuất dữ liệu thu hồi sản phẩm từ file JSON (`output.json`)
- Làm sạch và chuyển đổi dữ liệu
- Nạp dữ liệu vào cơ sở dữ liệu PostgreSQL

Pipeline được đóng gói và triển khai bằng Docker, giúp dễ dàng cài đặt và mở rộng.

## Tải file dữ liệu nguồn:

### Do file quá lớn nên phải tải về chứ ko request trực tiếp: 
curl -o output.json https://recalls-rappels.canada.ca/sites/default/files/opendata-donneesouvertes/HCRSAMOpenData.json

### Chạy dự án:
docker-compose up -d
