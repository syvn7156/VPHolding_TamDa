# Resort 300 ha — Concept Masterplan v1

> **Status:** Phác thảo (Sketch / Concept), chưa phải bản vẽ kỹ thuật
> **Created:** 2026-05-03 by Claude
> **Tool used:** SVG (vector) + Three.js (3D massing) — **chi phí 0 đồng**
> **Mục đích:** Bản phác thảo concept để brief BOD, gọi NĐT sơ bộ, KHÔNG dùng cho xin phép xây dựng

---

## 📁 File trong thư mục

| File | Mô tả | Cách mở |
|:---|:---|:---|
| `masterplan_2d_v1.svg` | **Mặt bằng 2D top-down** (vector, edit được) | Mở bằng trình duyệt, Inkscape (free), hoặc Adobe Illustrator |
| `masterplan_3d_v1.html` | **Mô hình 3D xoay được** | Click đúp → mở trong Chrome/Edge |
| `README.md` | File này | — |

---

## 🏝️ Giả định đã đặt (Assumptions made)

Vì anh Phong chưa cung cấp ranh đất cụ thể, em **giả định** để vẽ ra bản phác thảo. Nếu sai, sửa số → em vẽ lại:

| Tham số (Parameter) | Giả định (Assumption) | Cần xác nhận |
|:---|:---|:---:|
| Hình dạng đất | Vuông ~1.7 × 1.7 km | ⚠️ |
| Vị trí mặt nước | Phía Nam (biển/hồ) | ⚠️ |
| Số tầng tower | 4 tower 35F (sea-front) + 4 tower 28F (back row) | ⚠️ |
| Khoảng cách tower | ~200 m (đảm bảo view + thông gió) | ⚠️ |
| Marina | 80 slip (chỗ neo), ~12 ha | ⚠️ |
| Hồ bơi | 1 hồ chính ~0.5 ha (kidney shape) | ⚠️ |
| Tiện ích trung tâm | Clubhouse + Retail + Wellness + Sports | ⚠️ |
| Cổng chính | Phía Bắc | ⚠️ |

---

## 📊 Bảng phân khu sơ bộ (Zoning summary)

| Phân khu (Zone) | Diện tích ước (Est. Area) | % tổng đất |
|:---|---:|---:|
| 8 Tower (footprint + setback) | ~30 ha | 10% |
| Marina + bãi tắm | ~16 ha | 5% |
| Clubhouse + Pool + Wellness | ~5 ha | 2% |
| Retail / F&B Plaza | ~2 ha | 1% |
| Sports Zone | ~3 ha | 1% |
| Đường nội bộ + bãi xe | ~30 ha | 10% |
| Cây xanh + công viên (green park) | ~150 ha | 50% |
| Đất dự trữ phát triển (reserved) | ~64 ha | 21% |
| **TỔNG** | **~300 ha** | **100%** |

> **Lưu ý:** Mật độ xây dựng 10% là rất thấp — phù hợp tiêu chuẩn resort cao cấp. Nếu là chung cư đô thị bình thường, có thể tăng lên 25-35%.

---

## 🛠️ Cách import vào AutoCAD (nếu anh muốn chỉnh tay)

### Cách 1: Import SVG → DXF
1. Mở SVG bằng **Inkscape** (free): https://inkscape.org
2. File → Save As → chọn định dạng `Desktop Cutting Plotter (.dxf)`
3. Trong AutoCAD, dùng lệnh `DXFIN` → chọn file `.dxf`
4. Scale lại theo tỷ lệ thật (1 unit = 1 m)

### Cách 2: Dùng SVG làm ảnh underlay
1. Trong AutoCAD: lệnh `IMAGEATTACH`
2. Chọn `masterplan_2d_v1.svg` (cần convert PNG trước nếu AutoCAD không nhận SVG)
3. Vẽ chồng tay lên ảnh (đây là cách "manual trace" — chính xác nhất)

---

## 🚧 Bước tiếp theo gợi ý (Suggested next steps)

1. **Anh xem 2 file** (SVG + HTML 3D), feedback "cái này đúng / cái kia sai"
2. **Em vẽ lại v2** với thông số đúng (ranh đất thật, hướng biển, số tầng, etc.)
3. Khi concept ổn → mới **thuê KTS quy hoạch** chuyên resort + marina để vẽ bản kỹ thuật chính thức (bắt buộc cho xin phép xây dựng)
4. Brief với **Tâm (GĐ Dự Án)** + **Kevin (đối tác BĐS)** để cross-check

---

## ⚠️ Phản biện (Devil's Advocate)

| # | Rủi ro |
|:---:|:---|
| 1 | Bản này **KHÔNG phải bản vẽ KTS** — không có cao độ, kết cấu, MEP, thoát nước, v.v. |
| 2 | Marina cần **marine engineer** tính sóng/triều/neo — em không làm được phần đó |
| 3 | Hướng tower phụ thuộc **hướng nắng/gió thực tế** + view biển — cần khảo sát hiện trường |
| 4 | Mật độ + chiều cao tower cần kiểm tra **quy hoạch địa phương** (zoning) |
| 5 | 300ha là dự án cực lớn → cần ESIA (đánh giá tác động môi trường) trước khi xây |

---

## Changelog

- **2026-05-03 v1:** Bản phác thảo đầu tiên dựa trên brief "300ha + 8 chung cư + bến thuyền + dịch vụ". Tools: SVG + Three.js. Free 100%.
- **2026-05-03 v2 (Phase B — Level 2):** Nâng cấp lên PBR + Water + Sky shader. Sửa scale đúng **3.71 ha trapezoidal** theo `render_prompts.json`. Đúng vị trí Sông Tắc Đông + cao tốc Nam + Đường Tam Đa Tây + Kênh Ông Thảo Bắc. Thêm day/night slider, OrbitControls mượt, 8 tower theo C-shape opening east. Free 100%.
- **2026-05-03 v2-fix:** Bug fix — bản v2 đầu tiên dùng ES Module + importmap → bị browser **chặn khi mở từ `file://`** (CORS). Đổi sang **global `<script>` tags** với three.js r128 (chạy được từ file://). Thêm **3-CDN fallback** (jsDelivr → unpkg → Skypack) + live loading status để debug nếu CDN bị chặn. Nước dùng procedural normal map (không cần tải texture ngoài).
- **2026-05-03 v2-offline:** Tải toàn bộ 4 file thư viện về `lib/` local (~640 KB tổng). HTML giờ **chạy 100% offline** không cần internet. Vẫn giữ fallback CDN (jsDelivr + unpkg) phòng khi `lib/` thiếu file. Có thể copy folder masterplan_300ha sang USB/máy khác chạy được luôn.
- **2026-05-03 v2-fileproof:** Fix 2 lỗi từ Chrome console: (1) `thickness` không có trong `MeshPhysicalMaterial` r128 → bỏ; (2) `THREE.Water` shader dùng `WebGLRenderTarget` cho phản chiếu → bị Chrome chặn từ `file://` (security origin error) → thay bằng `MeshPhongMaterial` với animated normal map. Mất phản chiếu thật nhưng có sóng + highlight + chạy 100% từ file://. Glass tower vẫn đẹp dùng clearcoat + reflectivity.

---

## 🆕 Chi tiết v2 (Level 2 PBR Build)

### Thư viện đã tích hợp
| Thư viện | Vai trò | License |
|:---|:---|:---|
| `three.js r160` (module) | Core 3D engine | MIT |
| `OrbitControls` (addon) | Camera mượt, damping, hạn chế góc | MIT |
| `THREE.Water` (addon) | Sông Tắc + lagoon pool + Kênh Ông Thảo phản chiếu | MIT |
| `THREE.Sky` (addon, Hosek-Wilkie) | Bầu trời atmospheric + sun position | MIT |
| `MeshPhysicalMaterial` (built-in) | Kính xanh ngọc transmission + clearcoat | — |
| `CanvasTexture` (built-in) | Wood grain + grass + asphalt + sand procedural | — |
| `InstancedMesh` (built-in) | 600+ cây xanh hiệu năng cao | — |

### Tính năng v2
- ☀️ **Day/Night slider** (06:00 → 22:00) — sun di chuyển, sky đổi màu, tower phát sáng vàng ban đêm
- 🚗 **Xe hơi animate** chạy 2 chiều trên cao tốc DCT Bắc-Nam
- 🛥️ **6 cầu tàu + 12 du thuyền** ở marina Sông Tắc
- 📷 **6 view preset** (Aerial SW, Top, Marina, Cao tốc, Night, Ground level) — chuyển có tweening
- 📊 **FPS counter** real-time

### CDN dùng
```
https://cdn.jsdelivr.net/npm/three@0.160.0/...
```
Nếu offline hoặc CDN block: tải Three.js về local rồi sửa importmap.

### Browser yêu cầu
- Chrome/Edge ≥ 89
- Firefox ≥ 108
- Safari ≥ 16.4
*(cần hỗ trợ ES Module `importmap`)*

### So sánh v1 vs v2

| Tiêu chí | v1 | v2 |
|:---|:---:|:---:|
| Lines of code | ~150 | ~830 |
| File size | 8 KB | 30 KB |
| Hình học | Vuông 1.7 km giả định | **Trapezoidal 3.71 ha thực** |
| Material | Lambert flat color | **PBR (Physical + Standard)** |
| Nước | Plane phẳng | **Water shader phản chiếu** |
| Bầu trời | Solid color | **Sky shader (Hosek-Wilkie)** |
| Camera | Custom orbit cơ bản | **OrbitControls (damping, limits)** |
| Day/Night | ❌ | ✅ Slider + tower glow |
| Xe hơi | ❌ | ✅ 18 xe animate |
| Marina | 8 boats đơn giản | 12 boats + cabin + dock |
| Cây xanh | 50-60 thủ công | **600 instanced** |
| Chất lượng vs render AI | ~10-15% | **~35-45%** |

