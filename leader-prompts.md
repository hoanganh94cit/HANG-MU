# Ảnh ban chủ nhiệm Fanclub

Ba người đứng trước bàn thờ trên overlay live. Lưu vào `assets/` đúng tên file, tải lại overlay là thấy. Chưa có ảnh nào thì người đó tạm dùng ảnh Fan nam đứng.

| Vai trò | Tên trên overlay | Vị trí | File |
|---|---|---|---|
| Chủ nhiệm Fanclub | Chủ nhiệm Carrick | Giữa, có vòng sáng | `leader_chairman.png` |
| Phó Fanclub | Phó Fanclub | Bên trái | `leader_vice.png` |
| Admin | Admin Hang | Bên phải | `leader_admin.png` |

## Cách làm trong Flow

- Đính kèm `assets/pose_man_stand.png` làm mẫu nét vẽ, để ba người này khớp với đám đông.
- Dán prompt của từng người (tiếng Anh, giữ nguyên).
- Xuất PNG **nền trong suốt**. Không được thì để nền xanh lá #00FF00, Claude sẽ tách nền.
- Ba người này **quay mặt về phía khán giả** (nhìn thẳng), khác với fan nhìn từ sau lưng, vì họ đứng trên bục dẫn dắt buổi live.
- Kích thước tùy ý, code tự co giãn cho bằng cỡ người đứng.

## Chủ nhiệm Fanclub · Michael Carrick → `leader_chairman.png`

Michael Carrick là người thật. Flow có thể từ chối vẽ khuôn mặt giống người thật. Nếu bị từ chối, dùng **phương án B** (nhìn từ sau lưng, nhận ra nhờ tên và số áo).

### Phương án A: nhìn thẳng

```text
The reference image shows the illustration style to match: a cartoon sticker-style Manchester United fan with clean dark outlines and soft cel shading. In exactly this style, draw a friendly cartoon caricature of a tall, slim Englishman in his forties inspired by former Manchester United midfielder Michael Carrick: short neat dark-brown hair, light stubble, calm confident smile. He wears a smart black Manchester United club jacket with a small red club crest on the chest over a red Manchester United shirt, a red-and-white Manchester United scarf around the neck, dark trousers and black shoes. Full body, standing upright and facing the viewer, as the chairman of a fan club welcoming the crowd: one hand raised in a warm wave, the other holding a small gold trophy. Single character only, centered, full body visible. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than the club crest.
```

### Phương án B: nhìn từ sau lưng

```text
The reference image shows the illustration style to match: a cartoon sticker-style Manchester United fan seen from behind, with clean dark outlines and soft cel shading. In exactly this style, draw a tall, slim man with short neat dark-brown hair seen from behind, wearing a red Manchester United home jersey with "CARRICK" and the number 16 on the back, white shorts, red-and-white socks and black boots, a red-and-white Manchester United scarf over one shoulder. He stands upright like a captain leading the fans, holding a gold trophy high above his head with one hand. Back view, full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

## Phó Fanclub → `leader_vice.png`

```text
The reference image shows the illustration style to match: a cartoon sticker-style Manchester United fan with clean dark outlines and soft cel shading. In exactly this style, draw a cheerful young Vietnamese woman, the vice-chair of a Manchester United fan club: short black bob haircut, bright smile. She wears a red Manchester United home jersey, white shorts, red-and-white socks and white sneakers, a red-and-white Manchester United scarf around the neck. Full body, standing upright and facing the viewer, holding a red megaphone to her mouth with one hand and raising the other fist to lead the crowd's chant. Single character only, centered, full body visible. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than the club crest on the jersey.
```

## Admin → `leader_admin.png`

```text
The reference image shows the illustration style to match: a cartoon sticker-style Manchester United fan with clean dark outlines and soft cel shading. In exactly this style, draw a friendly young Vietnamese man, the admin of a Manchester United fan club livestream: short spiky black hair, round black glasses, a gaming headset with a microphone around his neck. He wears a black Manchester United training jacket over a red Manchester United jersey, dark jeans and white sneakers. Full body, standing upright and facing the viewer, holding a smartphone on a small selfie stick in one hand and giving a thumbs-up with the other. Single character only, centered, full body visible. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than the club crest.
```

## Lưu ý

Ghi tên "Chủ nhiệm Carrick" trên live có thể khiến người xem nghĩ Michael Carrick thật sự tham gia hoặc ủng hộ kênh. Nên coi đây là ảnh fan vẽ cho vui, không dùng tên và hình của anh ấy để quảng cáo hay kêu gọi donate.
