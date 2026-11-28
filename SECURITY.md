<!-- SPDX-License-Identifier: Apache-2.0 -->

# Chính sách bảo mật hệ sinh thái SIU Sirocco

Tài liệu áp dụng chung cho các kho thuộc tổ chức **SIU Sirocco** (`sirocco-core`, `sirocco-schoolops` và kho liên kết `Eco-Track`).

## Báo cáo lỗ hổng bảo mật

- **Không tạo Issue công khai** cho lỗ hổng bảo mật, rò rỉ khóa xác thực, vượt quyền ACL (như G03) hoặc lỗi bỏ qua kiểm dịch ClamAV.
- Dùng mục **Security → Report a vulnerability** trên GitHub của kho tương ứng, hoặc liên hệ riêng trực tiếp cho nhóm duy trì.
- Khi báo cáo, vui lòng đính kèm:
  - Phiên bản/tag hoặc commit SHA bị ảnh hưởng.
  - Bước tái hiện ngắn gọn (đã che toàn bộ token, mật khẩu và dữ liệu cá nhân).
  - Mức độ ảnh hưởng dự kiến.

## Phạm vi ưu tiên xử lý

- Cô lập quyền Connector v2 (`Client ID`, scope) và ngăn đọc chéo dữ liệu giữa các ứng dụng qua APISIX Gateway.
- Đường ống cách ly SeaweedFS, quét ClamAV và đối chiếu `VerifiedScanReceipt`.
- Cơ chế đăng nhập OIDC PKCE S256 trên Keycloak và bảo vệ phiên trên từng ứng dụng.
