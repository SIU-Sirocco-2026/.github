<!-- SPDX-License-Identifier: Apache-2.0 -->

# Hướng dẫn đóng góp chung — SIU Sirocco

Cảm ơn bạn đã quan tâm đến hệ sinh thái nguồn mở **SIU Sirocco** (gồm [Sirocco Core](https://github.com/SIU-Sirocco-2026/sirocco-core), [Sirocco SchoolOps](https://github.com/SIU-Sirocco-2026/sirocco-schoolops) và [Eco-Track](https://github.com/SIU-Sirocco-2025/Eco-Track)).

## Cách bắt đầu

1. Kiểm tra mục lục kho tương ứng để xem hướng dẫn cài đặt và bộ kiểm thử bắt buộc:
   - `sirocco-core`: chạy `pnpm typecheck`, `pnpm build`, `pnpm test` và `node scripts/check-docs-links.mjs`.
   - `sirocco-schoolops`: chạy `pnpm typecheck`, `pnpm test`, `pnpm build` và `pnpm source:verify`.
   - `Eco-Track`: chạy `node --test test/sirocco-*.test.js` và kiểm cú pháp module tích hợp.
2. Giữ ngôn ngữ commit, mô tả PR, issue và bình luận bằng **tiếng Việt** (giữ nguyên tên API, biến môi trường và đường dẫn kỹ thuật).
3. Không commit `.env`, token, khóa bí mật hoặc cấu hình cá nhân.
4. Tuân thủ đúng giấy phép của từng kho (`Apache-2.0` cho Core & SchoolOps; `GPL-3.0-or-later` cho Eco-Track) và gắn header `SPDX-License-Identifier` khi tạo tệp nguồn mới.
