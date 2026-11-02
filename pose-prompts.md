# Ảnh hành động cổ động viên

2 nhân vật × 5 hành động = 10 ảnh. Lưu vào `assets/` đúng tên file, tải lại trang là thấy. Ảnh nào chưa có thì nhân vật đó tạm dùng ảnh ngồi cũ.

## Danh sách

| Nhân vật | Đứng | Ngồi | Nằm | Khóc | Chửi lớn |
|---|---|---|---|---|---|
| Fan nam | ✅ `pose_man_stand.png` | ✅ `pose_man_sit.png` | ✅ `pose_man_lie.png` | ✅ `pose_man_cry.png` | ✅ `pose_man_shout.png` |
| Fan nữ | ✅ `pose_woman_stand.png` | ✅ `pose_woman_sit.png` | ✅ `pose_woman_lie.png` | ✅ `pose_woman_cry.png` | `pose_woman_shout.png` |

✅ = đã có trong `assets/`.

## Cách làm trong Flow

- Đính kèm **2 ảnh mẫu**: ảnh nhân vật (cột "Ảnh mẫu" bên dưới) để giữ đúng người, và `assets/pose_man_stand.png` để giữ đúng nét vẽ.
- Dán prompt của ảnh cần làm (tiếng Anh, giữ nguyên).
- Xuất PNG **nền trong suốt**. Không được thì để nền xanh lá #00FF00, Claude sẽ tách nền.
- Kích thước tùy ý, càng lớn càng nét. Code tự co giãn: các hành động đứng (đứng, khóc, chửi lớn) cao gấp khoảng 1,5 lần ngồi.
- Lưu xong báo Claude để cắt viền thừa và kiểm tra.

## Fan nam · ảnh mẫu `assets/c_man.png`

### Đứng → `pose_man_stand.png` ✅ đã có

```text
The first reference image shows the character: a young man with short messy dark brown hair, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: standing upright, cheering with both arms raised high, holding a red-and-white Manchester United scarf stretched above the head with both hands. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Ngồi → `pose_man_sit.png` ✅ đã có

```text
The first reference image shows the character: a young man with short messy dark brown hair, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: sitting on the floor with knees bent, one fist raised in the air cheering, a red Manchester United scarf around the neck. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Nằm → `pose_man_lie.png` ✅ đã có

```text
The first reference image shows the character: a young man with short messy dark brown hair, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: lying relaxed on their side on a small red fan blanket on the floor, propped up on one elbow, waving a small red flag with the other hand; the body is horizontal. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Khóc → `pose_man_cry.png` ✅ đã có

```text
The first reference image shows the character: a young man with short messy dark brown hair, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: standing with shoulders slumped and head bowed, crying after a lost match: tears streaming down the cheek (visible in the three-quarter back view), wiping the eyes with a red Manchester United scarf held in one hand. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Chửi lớn → `pose_man_shout.png` ✅ đã có

```text
The first reference image shows the character: a young man with short messy dark brown hair, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: standing and leaning forward, shouting loudly in frustration at the pitch with the mouth wide open (visible in the three-quarter back view), one fist raised and shaking in the air, the other hand cupped beside the mouth; angry and intense, but no rude hand gestures, no speech bubbles and no written words. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

## Fan nữ · ảnh mẫu `assets/c_woman.png`

### Đứng → `pose_woman_stand.png` ✅ đã có

```text
The first reference image shows the character: a young woman with very long straight black hair down to her waist, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: standing upright, cheering with both arms raised high, holding a red-and-white Manchester United scarf stretched above the head with both hands. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Ngồi → `pose_woman_sit.png` ✅ đã có

```text
The first reference image shows the character: a young woman with very long straight black hair down to her waist, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: sitting on the floor with knees bent, one fist raised in the air cheering, a red Manchester United scarf around the neck. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Nằm → `pose_woman_lie.png` ✅ đã có

```text
The first reference image shows the character: a young woman with very long straight black hair down to her waist, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: lying relaxed on their side on a small red fan blanket on the floor, propped up on one elbow, waving a small red flag with the other hand; the body is horizontal. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Khóc → `pose_woman_cry.png` ✅ đã có

```text
The first reference image shows the character: a young woman with very long straight black hair down to her waist, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: standing with shoulders slumped and head bowed, crying after a lost match: tears streaming down the cheek (visible in the three-quarter back view), wiping the eyes with a red Manchester United scarf held in one hand. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```

### Chửi lớn → `pose_woman_shout.png`

```text
The first reference image shows the character: a young woman with very long straight black hair down to her waist, slim build, a Manchester United fan seen from behind, wearing a red Manchester United home jersey with "B.FERNANDES" and the number 8 on the back, white shorts and red-and-white socks. The second reference image shows the illustration style to match. Draw THE SAME character in the same style (clean dark outlines, soft cel shading, cartoon sticker look) in this pose: standing and leaning forward, shouting loudly in frustration at the pitch with the mouth wide open (visible in the three-quarter back view), one fist raised and shaking in the air, the other hand cupped beside the mouth; angry and intense, but no rude hand gestures, no speech bubbles and no written words. Back view or three-quarter back view, as if the viewer stands behind them in a stadium crowd facing a stage. No book, no cushion. Full body visible, single character only, centered. Transparent background (or plain solid green #00FF00 if transparency is not possible), no floor, no shadow, no text other than on the jersey.
```
