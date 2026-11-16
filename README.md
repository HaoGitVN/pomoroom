# 🍅 PomoRoom: Cozy Study

Ứng dụng web **Pomodoro 3D thư giãn** chạy hoàn toàn trên trình duyệt, chỉ cần một file `index.html`. Bạn học bài trong một căn phòng low-poly ấm cúng, có nhân vật gõ phím theo phiên tập trung và nghỉ ngơi theo phiên giải lao. Lấy cảm hứng từ phong cách của *Spirit City: Lofi Sessions* (không liên kết với game này).

## ✨ Tính năng

- **Phòng học 3D** dựng bằng Three.js: đổ bóng mềm, đèn bàn bấm để bật/tắt, laptop, bảng ghim, giá sách, sofa, thảm, đồng hồ treo tường.
- **Nhân vật** có hoạt họa theo trạng thái: gõ phím khi tập trung, ngả lưng/vươn vai/uống nước khi giải lao. Lúc nhàn rỗi nhân vật tự đi lại, ngồi sofa đọc sách, nằm nghỉ, vươn vai, hít đất, ra giá sách tìm sách. Có thể thay bằng model `.glb` của bạn.
- **Pomodoro**: các gói có sẵn (Chuẩn 25/5, Deep Work 50/10, Học Nhanh 15/3, Demo 10s/10s) và **giờ tự chọn**. Cứ 4 phiên thì được nghỉ dài 15 phút. Hoàn thành phiên được thưởng Xu.
- **Bảng việc cần làm 3D**: giấy nhớ dán trên bảng ghim, chọn việc ưu tiên cho phiên, hoàn thành việc được +10 Xu.
- **Học tập sinh động**: trong phiên tập trung nhân vật luân phiên gõ phím, xem bài giảng video trên laptop (màn hình phát video giả lập), ghi chép bằng bút vào vở, đọc sách. Bàn học có sẵn vở, bút và sách.
- **Laptop chi tiết**: bàn phím đầy đủ (53 phím, phím lún xuống khi gõ), touchpad, chuột không dây trên bàn di chuột. Màn hình chạy các trang học tập giả lập: soạn ghi chú gõ từng chữ, bài giảng video, và trang thư viện online với 24 tài liệu nhiều môn đại học: nhân vật kéo thanh cuộn tìm tài liệu, có xác suất tìm thấy rồi bấm Tải về và mở đọc.
- **Bàn học nâng cấp** (lấy cảm hứng từ góc học tập thực tế): máy tính bảng hiển thị đồng hồ Pomodoro với chiếc cốc đầy dần, heo đất chấm bi (có xu rơi vào khi bạn kiếm Xu, bấm để chọc), hàng bút dạ quang cầu vồng, cốc bút, giấy note, chồng sách và giấy tờ có highlight.
- **Phong cảnh Thành phố hoàng hôn**: đường chân trời có cửa sổ nhà sáng đèn nhấp nháy và xe chạy.
- **Thời đại AI**: màn hình laptop còn có trình soạn code kiểu VS Code (gõ code từng ký tự, chạy ra kết quả) và trợ lý AI dạng chat (gõ câu hỏi, gửi, câu trả lời hiện dần). Phím trên laptop lún theo từng nhịp gõ.
- **Ghi chép tự nhiên**: cuốn tập đặt giữa bàn, ngay dưới laptop; một tay giữ trang, tay kia viết, thỉnh thoảng nhân vật ngước nhìn màn hình rồi ghi tiếp.
- **Ăn uống**: nếu đã mua đồ uống/bánh, thỉnh thoảng nhân vật cầm ly lên nhấp một ngụm hoặc cắn bánh rồi đặt lại.
- **Cửa hàng**: mua cà phê, matcha, croissant, xương rồng, đèn lava rồi sắp xếp trên bàn. Dữ liệu lưu bằng `localStorage`.
- **Phong cảnh**: Nắng ban mai, Đêm mưa, Rừng thông tuyết rơi, Hoàng hôn tím.
- **Âm thanh**: tiếng mưa, lửa trại, chuông (tạo bằng Web Audio API), 4 bài nhạc Lofi tự tạo, và trình phát YouTube. Âm lượng chỉnh riêng từng loại trong ⚙️ Cài đặt.
- **Giao diện thích ứng** điện thoại dọc/ngang, chế độ toàn màn hình, tự ẩn giao diện sau 10 giây (chạm vào khoảng trống trong phòng để ẩn/hiện).

## 🕹️ Cách dùng nhanh

1. Bấm vào **laptop** (hoặc nút 💻) để chọn thời gian, phong cảnh, âm thanh, rồi bấm **Bắt đầu tập trung**.
2. Bấm **bảng ghim** để quản lý việc cần làm. Bấm **đèn bàn** để bật/tắt.
3. Mở **Cửa hàng**, mua đồ rồi bấm vào đồ trên bàn và bấm chỗ trống để dời.
4. Kéo chuột/ngón tay để xoay phòng, cuộn/chụm để phóng to.

## 🚀 Chạy thử trên máy

Mở thẳng `index.html` bằng trình duyệt, hoặc chạy server tĩnh:

```bash
python3 -m http.server 8080
# mở http://localhost:8080
```

Cần có Internet để tải Three.js từ CDN (jsDelivr).

## 🌐 Đưa lên GitHub Pages

1. Tạo repo mới trên GitHub và tải các file trong thư mục này lên (giữ `index.html` ở thư mục gốc).
2. Vào **Settings → Pages**, mục *Build and deployment* chọn **Deploy from a branch**, branch `main`, thư mục `/ (root)`, rồi **Save**.
3. Đợi khoảng 1 phút, trang chạy tại `https://<tên-bạn>.github.io/<tên-repo>/`.

## 📝 Lưu ý

- **YouTube:** một số video cấm nhúng hoặc trình duyệt chặn tự phát. Khi đó dùng liên kết "Mở trên YouTube" hoặc chọn nhạc Lofi có sẵn. Thanh trượt Nhạc chỉ chỉnh được nhạc có sẵn.
- **Model nhân vật:** nên dùng file `.glb` (đóng gói sẵn). File `.gltf` có kèm file ngoài có thể không đọc được.
- **Toàn màn hình** có thể không dùng được trên iPhone Safari.

## 📁 Cấu trúc dự án

```
├── index.html   # toàn bộ ứng dụng (HTML + CSS + JS)
├── README.md
├── LICENSE      # MIT
├── .gitignore
└── .nojekyll    # để GitHub Pages phục vụ file trực tiếp
```

## 🤝 Đóng góp

Mở Issue hoặc Pull Request đều được. Ý tưởng tiếp theo: thêm vật phẩm mới, thêm nhạc Lofi, thêm phong cảnh, lưu tiến độ theo tuần.

## 🧱 Công nghệ

Three.js r128 (`OrbitControls`, `GLTFLoader`), Web Audio API, HTML/CSS/JS thuần, không cần build.

## 📄 Giấy phép

MIT, xem file `LICENSE`. Dự án được tạo cùng Claude (Anthropic).
