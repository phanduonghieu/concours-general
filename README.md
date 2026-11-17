# Concours Général des Lycées — Mathématiques (1990–2025)

Tuyển tập đầy đủ đề thi Concours Général de mathématiques, tải từ APMEP :
https://www.apmep.fr/Annales-Concours-General-des-lycees

**36 năm, 1990 → 2025** — mỗi năm đều có cả mã nguồn LaTeX và bản PDF.

## Nội dung thư mục

| Mục | Mô tả |
|-----|-------|
| `tex/CG_<année>.tex` | Mã nguồn LaTeX gốc của từng đề (36 file) |
| `pdf/CG_<année>.pdf` | Bản PDF từng đề (36 file) |
| `Concours_General_Maths_1990-2025.pdf` | **Tuyển tập gộp** — 84 trang, có bookmark theo năm. Mở là đọc được ngay. |
| `Recueil_master.tex` | File LaTeX chủ (dùng `pdfpages`) để tự dựng lại tuyển tập có mục lục + bookmark |
| `index.html` | **Trang web đọc đề**: mục lục theo năm (nhóm thập niên), xem PDF ngay trong trang, nút Trước/Sau, tải `.pdf`/`.tex`. Mở bằng trình duyệt. |

## Dùng ngay

- Chỉ muốn đọc/in → mở `Concours_General_Maths_1990-2025.pdf`.
- Muốn chỉnh/soạn lại → sửa các file trong `tex/`, hoặc biên dịch `Recueil_master.tex` :
  ```
  pdflatex Recueil_master.tex
  pdflatex Recueil_master.tex   # chạy 2 lần để có mục lục
  ```
  (cần có `pdflatex` và gói `pdfpages`.)

## Ghi chú kỹ thuật

- Các file `.tex` gốc **không đồng nhất**: khác documentclass (article/report,
  có bản landscape/twocolumn), nhiều bản dùng **PSTricks** (phải biên dịch bằng
  `latex`→`dvips`→`ps2pdf` hoặc `pdflatex` kèm `auto-pst-pdf`). Vì vậy tuyển tập
  được gộp ở mức **PDF** (chắc chắn chạy) thay vì ghép mã nguồn.
- Bản 2002–2021 lấy từ kho lưu trữ `C_G_2002_2022.zip` của APMEP; 1990–2001 và
  2022–2025 tải riêng từng năm. Tên file đã được chuẩn hoá thành `CG_<année>`.
- Nguồn: APMEP (Association des professeurs de mathématiques de l'enseignement public).