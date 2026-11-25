<p align="center">
  <img src="https://raw.githubusercontent.com/SIU-Sirocco-2026/.github/main/profile/assets/sirocco-logo.png" width="96" height="96" alt="Logo đội SIU Sirocco">
</p>

<h1 align="center">SIU Sirocco</h1>

<p align="center">Đội sinh viên Trường Đại học Quốc tế Sài Gòn. Chúng tôi phát triển Sirocco Core và tích hợp các dịch vụ dùng chung qua API vào ứng dụng thực tế.</p>

## Các dự án

```mermaid
flowchart TB
    accTitle: Core và hai ứng dụng
    accDescr: SchoolOps và bản EcoTrack tích hợp gọi API của Sirocco Core. Mỗi ứng dụng có giao diện và nghiệp vụ riêng.
    school["SchoolOps<br/>Vận hành trường học"] --> core["Sirocco Core<br/>Dịch vụ dùng chung qua API"]
    eco["EcoTrack tích hợp<br/>Chất lượng không khí"] --> core
    classDef platform fill:#07304a,stroke:#16869a,color:#ffffff
    class core platform
```

| Dự án | Bài toán |
| --- | --- |
| **Sirocco Core** | Cung cấp đăng nhập, workflow, bản ghi và lưu trữ tệp có kiểm dịch cho backend ứng dụng. |
| **EcoTrack** | Theo dõi chất lượng không khí. Bản tích hợp với Core hỗ trợ xác minh nguồn dữ liệu PM2.5 và theo dõi phản ánh. |

## Khám phá mã nguồn

[EcoTrack 2025](https://github.com/SIU-Sirocco-2025/Eco-Track) là bản độc lập công khai của đội. Bản EcoTrack trong sơ đồ là phiên bản tích hợp Sirocco Core. Xem [các bản phát hành EcoTrack 2025](https://github.com/SIU-Sirocco-2025/Eco-Track/releases) hoặc mở [danh sách kho SIU Sirocco](https://github.com/orgs/SIU-Sirocco-2026/repositories) để xem các kho tài khoản của bạn có quyền truy cập.
