# CLAUDE.md – Quy tắc quản lý task

Repo này dùng **GitHub Issues** để quản lý task của team. Claude đọc file này mỗi khi bắt đầu phiên làm việc và làm theo các quy tắc dưới đây.

## Format của một task (issue)

Mỗi task có:
- **Tiêu đề:** ngắn gọn, bắt đầu bằng động từ (ví dụ: "Đăng ký Brand Registry").
- **Bảng PIC / Deadline** ở đầu nội dung:

  | PIC | Deadline |
  |---|---|
  | TBD | TBD |

- **Mục tiêu:** 1–2 câu, task này để đạt được gì.
- **Checklist:** các bước cụ thể, dạng `- [ ]`.

Quy ước:
- Deadline ghi dạng `DD/MM/YYYY`. Chưa biết thì ghi `TBD`.
- PIC ghi tên người. Nếu người đó có tài khoản GitHub trong repo thì gán vào mục **Assignees**. Chưa có người thì ghi `TBD`.
- Viết bằng tiếng Việt.

## Label

| Label | Dùng khi |
|---|---|
| `product` | Task liên quan đến product |
| `account` | Task liên quan đến tài khoản, setup |
| `brand registry` | Task đăng ký / quản lý brand |
| `way of working` | Quy trình làm việc, công cụ, platform |
| `priority: high` | Task quan trọng, cần làm trước |
| `tracker` | Issue tổng hợp, không phải task |

Chỉ dùng label trong bảng trên. Muốn thêm label mới thì hỏi lại trước.

## Trạng thái

- ⬜ **Todo:** chưa bắt đầu
- 🟡 **In progress:** đang làm
- 🔴 **Blocked:** bị kẹt, phải ghi lý do trong comment
- ✅ **Done:** đóng issue (state reason = completed)

## Claude cần làm gì

- Khi được nhờ tạo task: dùng đúng format và label ở trên. Thiếu PIC hoặc deadline thì ghi `TBD` và nhắc lại cho người dùng.
- Khi được nhờ cập nhật task: sửa nội dung issue và để lại một comment ngắn ghi rõ đã thay đổi gì.
- Trước khi tạo task mới: kiểm tra xem đã có task trùng chưa.
- Không xoá hoặc đóng task nếu người dùng chưa đồng ý.
- Khi tổng hợp / báo cáo: chia nhóm theo trạng thái, nêu rõ task trễ hạn và task chưa có PIC hoặc deadline.

## Câu lệnh nhanh

- `thêm task: <nội dung> | PIC: <tên> | hạn: <ngày>`
- `cập nhật #<số>: <đang làm / xong / bị kẹt vì …>`
- `tổng hợp tuần này`
- `từ biên bản họp này tạo task: <nội dung>`
