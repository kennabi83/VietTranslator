# Viet Translator — FFXIV tiếng Việt

Plugin [Dalamud](https://github.com/goatcorp/Dalamud) hiển thị **phụ đề tiếng Việt** cho thoại
Final Fantasy XIV: overlay ImGui, chữ có dấu chuẩn (font BeVietnam Pro), giữ nguyên tên riêng
tiếng Anh để dễ tra cứu cùng cộng đồng. Bản dịch làm sẵn ngoại tuyến — **không sửa dữ liệu game**.

> **Mới nhất — v1.3.4:** Sửa nốt lỗi thoại lòi tiếng Anh — những đoạn thoại dài bị game chia thành nhiều trang giờ đã khớp được bản dịch.

## Cài đặt

1. Trong game, gõ `/xlsettings` → mở tab **Experimental**.
2. Ở mục **Custom Plugin Repositories**, dán đường dẫn dưới đây, bấm **+** rồi **Save & Close**:

   ```
   https://raw.githubusercontent.com/kennabi83/VietTranslator/main/repo.json
   ```

3. Gõ `/xlplugins`, tìm **Viet Translator**, bấm **Install**.
4. Vào chơi — cốt truyện sẽ hiện phụ đề tiếng Việt. Gõ `/viettl` để bật/tắt overlay.

## Phạm vi bản dịch

### A Realm Reborn (2.0–2.55) — đầy đủ
Trọn bộ ARR: **904 nhiệm vụ, hơn 30.000 dòng thoại.**

- Cốt truyện chính (MSQ) 2.0 + hậu-ARR 2.1–2.55, tới finale *The Steps of Faith*.
- Toàn bộ nhiệm vụ Nghề & Job (Class/Job).
- Nhiệm vụ mở khóa tính năng: nhà ở, chocobo, retainer, materia, glamour, Triple Triad, Palace of the Dead…
- Nhiệm vụ mở khóa Duty: dungeon, trial, raid (thường / Hard / Extreme).

### Heavensward (3.0–3.5) — đầy đủ
Trọn bộ HW: **425 nhiệm vụ, hơn 18.000 dòng thoại.**

- Cốt truyện chính (MSQ) 3.0 + hậu-Dragonsong 3.1–3.5, trọn 128 nhiệm vụ.
- Toàn bộ nhiệm vụ Nghề & Job (167 nhiệm vụ), gồm cả Dark Knight, Astrologian, Machinist.
- Nhiệm vụ mở khóa Duty: Alexander, Void Ark, Warring Triad, Dun Scaith…
- Nhiệm vụ mở khóa tính năng: Scholasticate, Hildibrand, Anima Weapons, Ishgardian Restoration…

> **Ngoài phạm vi:** side quest (nhiệm vụ phụ) tạm hoãn tới giai đoạn cuối. Những dòng chưa dịch
> sẽ hiển thị nguyên bản tiếng Anh — plugin không gây lỗi hay chặn nội dung nào.

## Lịch sử phiên bản

- **v1.3.4** — Sửa lỗi thoại dài hiện nguyên tiếng Anh. Khi một câu quá dài, game tự chia hộp thoại thành nhiều trang; plugin chỉ đọc được trang đầu nên tra không ra bản dịch. Nay đã khớp được qua bảng tra riêng cho hơn 3.400 đoạn thoại dài.
- **v1.3.3** — Sửa lỗi khớp bản dịch. Những câu thoại chứa phần thay đổi theo bối cảnh — lời chào theo giờ trong ngày ("Good morrow/day/evening"), câu đổi theo chủng tộc hoặc thành bang khởi đầu, xưng hô theo cấp bậc Grand Company — trước đây không khớp được nên hiện nguyên tiếng Anh; nay đã hiển thị tiếng Việt. Đồng thời chặn lỗi lộ mã thẻ ra khung phụ đề. Số câu khớp được tăng thêm khoảng 1.900.
- **v1.3.2** — Cập nhật nhỏ. Bổ sung 3 nhiệm vụ mở khóa trước đây bị bỏ sót vì Square Enix xếp nhầm vào nhóm side quest: *Rock the Castrum* (trọn cutscene mở màn Castrum Meridianum — diễn văn Chiến Dịch Archon và trận Livia sas Junius), *Earning Your Wings* (mở Rival Wings) và *Every Little Thing She Does Is Mahjong* (mở mạt chược Doma ở Gold Saucer).
- **v1.3.1** — Sửa lỗi hiển thị tên người nói: 60 đoạn thoại bị lặp tên trong hộp thoại (vd "(-Phó Vương-)(Phó vương)"), và một đoạn giữ nhầm "???" đúng lúc nhân vật tự xưng danh tính.
- **v1.3.0** — **Heavensward hoàn chỉnh**: thêm nhiệm vụ Nghề/Job (167), Duty (38) và mở khóa tính năng (92) — tổng 425 nhiệm vụ HW. Sửa lỗi bản dịch: khôi phục 254 chỗ mất tên người nói, 15 chỗ mất danh hiệu Grand Company, 20 chỗ mất nhấn mạnh; sửa 1 chỗ lộ mã chương trình ra hội thoại; dọn 88 thẻ điều kiện thừa.
- **v1.1.0** — Thêm trọn bộ cốt truyện chính Heavensward (MSQ, 128 nhiệm vụ). Vá 156 đoạn thoại ARR bị dịch thiếu phần sau (lỗi ngắt trang).
- **v1.0.1** — Sửa gạch nối ẩn, tách hộp thoại độc thoại dài, tinh chỉnh giọng nhân vật.
- **v1.0.0** — Phát hành đầu tiên: trọn bộ A Realm Reborn.

## Miễn trừ

Dalamud và mọi plugin là phần mềm bên thứ ba, về nguyên tắc nằm ngoài điều khoản dịch vụ của
Square Enix. Bạn tự cân nhắc khi sử dụng. Plugin chỉ hiển thị một lớp phụ đề, không can thiệp
hay chỉnh sửa dữ liệu/tiến trình game.

---

Tác giả: **Yu**. Đóng góp / báo lỗi: mở issue tại repo này.
