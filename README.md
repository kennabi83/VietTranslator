# Viet Translator — FFXIV tiếng Việt

Plugin [Dalamud](https://github.com/goatcorp/Dalamud) hiển thị **phụ đề tiếng Việt** cho thoại
Final Fantasy XIV: overlay ImGui, chữ có dấu chuẩn (font BeVietnam Pro), giữ nguyên tên riêng
tiếng Anh để dễ tra cứu cùng cộng đồng. Bản dịch làm sẵn ngoại tuyến — **không sửa dữ liệu game**.

> **Mới nhất — v1.6.0:** trọn bộ **Endwalker**, và lần đầu có **thoại boss trong dungeon/trial/raid** từ A Realm Reborn tới Endwalker.

## Cài đặt

1. Trong game, gõ `/xlsettings` → mở tab **Experimental**.
2. Ở mục **Custom Plugin Repositories**, dán đường dẫn dưới đây, bấm **+** rồi **Save & Close**:

   ```
   https://raw.githubusercontent.com/kennabi83/VietTranslator/main/repo.json
   ```

3. Gõ `/xlplugins`, tìm **Viet Translator**, bấm **Install**.
4. Vào chơi — cốt truyện sẽ hiện phụ đề tiếng Việt. Gõ `/viettl` để bật/tắt overlay.

## Phạm vi bản dịch

Năm bản mở rộng đầu đã có phụ đề tiếng Việt: **2.629 nhiệm vụ · hơn 135.000 dòng thoại**, cộng
**7.800 dòng thoại boss** trong dungeon, trial và raid.

| Bản mở rộng | Nhiệm vụ | Dòng thoại |
|---|---|---|
| A Realm Reborn (2.0–2.55) | 987 | ~39.000 |
| Heavensward (3.0–3.5) | 448 | ~22.200 |
| Stormblood (4.0–4.5) | 397 | ~24.700 |
| Shadowbringers (5.0–5.5) | 366 | ~22.100 |
| Endwalker (6.0–6.5) | 431 | ~27.000 |

Mỗi bản mở rộng gồm:

- **Cốt truyện chính (MSQ)** kèm các mạch hậu-expansion.
- **Nhiệm vụ Nghề & Job**, và từ Shadowbringers có thêm **nhiệm vụ vai trò (Role)**.
- **Nhiệm vụ mở khóa Duty**: dungeon, trial, raid, alliance raid.
- **Nhiệm vụ mở khóa tính năng**: nhà ở, retainer, Gold Saucer, Hildibrand, Resistance Weapons, Studium…
- **Nhiệm vụ bộ tộc (beast tribe)** của ARR, Heavensward và Stormblood: đủ 12 bộ tộc.
- **Thoại giữa trận** trong nhiệm vụ, và **thoại boss** bên trong dungeon/trial/raid (mới ở v1.6.0).

> **Ngoài phạm vi:** side quest (nhiệm vụ phụ) và Dawntrail. Những dòng chưa dịch sẽ hiển thị
> nguyên bản tiếng Anh — plugin không gây lỗi hay chặn nội dung nào.

## Lịch sử phiên bản

- **v1.6.0** — **Endwalker hoàn chỉnh**: cốt truyện chính, Sage & Reaper, 5 tuyến nhiệm vụ vai trò, Studium Deliveries, mở khóa Duty và tính năng. **Thoại boss trong dungeon/trial/raid** từ ARR tới Endwalker (7.800 dòng) — nguồn dữ liệu trước đây chưa từng được khai thác. Bổ sung các nhiệm vụ trước đây chưa có: hai sự kiện Gold Saucer Festivities, *By the Time You Hear This*, *Akadaemia Anyder*. Sửa lỗi: người chơi có tên trùng một từ tiếng Anh (May, Will, Hope, Ruby…) bị lòi tiếng Anh ở hàng trăm câu; tên người nói trong ngoặc `(-…-)` lọt vào phụ đề; hàng trăm câu bị rơi mất bản dịch vì trùng khóa tra; câu người chơi phải gõ vào chat nay giữ nguyên tiếng Anh kèm chú nghĩa.
- **v1.5.2** — Thoại giữa trận Shadowbringers (316 dòng, 11 nhiệm vụ). Sửa 4 dòng đại từ cố định một giới.
- **v1.5.1** — Nhiệm vụ bộ tộc của ARR, Heavensward, Stormblood: 69 nhiệm vụ, 12 bộ tộc.
- **v1.5.0** — **Shadowbringers hoàn chỉnh**: 364 nhiệm vụ, gồm Bozja, Werlyt, Eden, YoRHa. Bổ sung 26 nhiệm vụ ARR bị sót vì trùng tên (có *The Ultimate Weapon*, *Operation Archon*).
- **v1.4.1 – v1.4.8** — **Stormblood hoàn chỉnh**, thoại giữa trận (BattleTalk), và khung theo dõi nhiệm vụ tiếng Việt khi rê chuột.
- **v1.3.6** — Sửa lỗi khớp với câu chứa giá trị do game điền vào lúc chơi: cấp bậc Grand Company trong lời chào của NPC, tên chủng tộc, tên nghề và tên vật phẩm. Trước đây những câu này hiện nguyên tiếng Anh vì bản dịch không đoán trước được giá trị. Nay đã phủ 145 câu chào theo cấp bậc và toàn bộ tên chủng tộc/nghề/vật phẩm cố định.
- **v1.3.5** — Sửa lỗi khớp với câu chứa gạch nối đặc biệt. Dữ liệu gốc dùng gạch nối dài trong tên riêng ("Brother E–Sumi–Yan") còn game hiển thị gạch nối thường, khiến 490 đoạn thoại tra không ra bản dịch.
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
