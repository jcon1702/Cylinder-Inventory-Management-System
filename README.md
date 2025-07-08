# Cylinder Inventory Management System

## Background
TotalEnergies Việt Nam đang trong giai đoạn số hóa dữ liệu vận hành LPG (hơn 12 triệu bình gas/năm) và năng lượng mặt trời. Việc theo dõi serial numbers, đối chiếu cylinder reconciliation, và phân tích hiệu suất tồn kho là mắt xích quan trọng để đảm bảo an toàn, chất lượng dữ liệu và hỗ trợ báo cáo ESG.

## Objective
Xây dựng một **Excel‑based Inventory Management System** để:
1. Theo dõi và quản lý trạng thái của từng bình gas theo tuần.
2. Phát hiện anomalies (lost, damaged) và tạo cảnh báo tự động.
3. Trực quan hóa dữ liệu qua dashboard giúp PM & Ban Quản Trị ra quyết định nhanh chóng.
4. Tính toán vòng đời trung bình của cylinder và đề xuất cải tiến hoạt động.

## Dataset
- **`01_Input`**: 25 serial records (S/N, DateReceived, CylinderType, InitialStatus).  
- **`02_Tracking`**: Hơn 100 bản ghi tracking theo 4 tuần (Status, Location, Warning flag).  
- **`00_Dictionary`**: Giải thích chi tiết các field.

## Methodology
1. **Data Cleaning**: Loại bỏ duplicate, kiểm tra missing S/N, chuẩn hóa ngày tháng.  
2. **Reconciliation**: Dùng PivotTable & formulas để đếm và highlight anomalies.  
3. **Dashboard**: Tạo Stacked Column, Pie, Line charts, thêm Slicers để filter nhanh.  
4. **Analysis**:  
   - Tính Error Rate (%) theo tuần và theo loại cylinder.  
   - Đếm serial “lost signal” (>2 tuần không được cập nhật).  
   - Tính vòng đời trung bình (lifespan) cho mỗi cylinder.  

## Results & Visualizations
![Dashboard Preview](docs/images/dashboard_preview.png)

- **Error Rate over Time:** giảm từ 28% → 20% trong 4 tuần.  
- **Cylinder Type Distribution:** 52% 12 kg, 48% 45 kg.  
- **Average Lifespan:** 30 ngày.  
- **Lost Signal Alerts:** 3 cylinders missing >2 weeks.

## Conclusions
- Hệ thống Excel đã giúp **phát hiện nhanh anomalies**, cải thiện tỷ lệ tracking accuracy từ 75% → 90%.  
- Loại bình 12 kg có error rate cao hơn (38% vs. 17%) → cần xem xét quy trình kiểm định hoặc chất lượng.  
- Đề xuất gắn QR code & tự động email cảnh báo để nâng cao hiệu quả tracking.

## File Structure
├── data/ # File Excel nguồn

├── docs/ # Slide report & hình ảnh

└── README.md # Hướng dẫn & tóm tắt project
