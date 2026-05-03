# `lib/` — Thư viện 3D local

Thư mục này chứa các thư viện cần để chạy `masterplan_3d_v2.html` **100% offline** (không cần internet).

## File trong thư mục

| File | Kích thước | Vai trò |
|:---|---:|:---|
| `three.min.js` | 590 KB | Three.js r128 — core 3D engine |
| `OrbitControls.js` | 26 KB | Camera xoay/zoom mượt |
| `Water.js` | 12 KB | Mặt nước Sông Tắc + lagoon (shader) |
| `Sky.js` | 7 KB | Bầu trời atmospheric (Hosek-Wilkie) |
| **Tổng** | **~640 KB** | Tất cả MIT license, free |

## Nguồn gốc

Tải từ npm registry chính thức:
```
https://registry.npmjs.org/three/-/three-0.128.0.tgz
```

Ngày tải: 2026-05-03

## Lưu ý

- HTML sẽ tự **thử local trước**, nếu thiếu file mới fallback CDN
- KHÔNG xóa thư mục này trừ khi đã có internet ổn định
- Nếu muốn nâng cấp Three.js, tải bản mới về cùng tên file (giữ r128 vì r150+ bỏ `examples/js/`)

## ⚠️ Cleanup cần làm tay

Trong quá trình tải, em không xóa được thư mục `_tmp/` (do giới hạn quyền sandbox). Anh **vào folder `lib/` xóa tay thư mục `_tmp` này** — nó là source giải nén tạm, ~25 MB, không cần dùng nữa.

```
F:\VP_Holding\Demo_BOD\masterplan_300ha\lib\_tmp\   ← XÓA THỦ CÔNG
```
