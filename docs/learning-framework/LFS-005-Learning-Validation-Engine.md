# LFS-005 — Learning Validation Engine

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-005 |
| Belge Adı | Learning Validation Engine |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-001, LFS-002, LFS-003, LFS-004 |

---

# 1. Amaç

Learning Validation Engine (LVE), kullanıcının yalnızca içeriği tüketip tüketmediğini değil, gerçekten öğrenip öğrenmediğini değerlendiren sistemdir.

LVE'nin amacı puan üretmek değil, öğrenmeyi doğrulamaktır.

---

# 2. Temel İlkeler

Bir konu yalnızca okunduğu veya izlendiği için öğrenilmiş kabul edilmez.

Doğrulama;

- bilgi,
- kavrama,
- uygulama,
- analiz,
- üretim,
- uzun dönem hatırlama

boyutlarını kapsar.

---

# 3. Doğrulama Katmanları

## LV-1 — Hatırlama

Örnek:

> HTTP'nin açılımı nedir?

---

## LV-2 — Kavrama

Örnek:

> HTTP neden durum kodları kullanır?

---

## LV-3 — Uygulama

Örnek:

> Basit bir REST isteği oluştur.

---

## LV-4 — Analiz

Örnek:

> Bu API tasarımındaki problemi bul.

---

## LV-5 — Üretim

Örnek:

> Yeni bir REST servisi tasarla.

---

## LV-6 — Aktarım (Transfer)

Örnek:

> Aynı prensibi GraphQL için nasıl uygularsın?

---

# 4. Doğrulama Yöntemleri

Sistem farklı doğrulama yöntemleri kullanabilir:

- Çoktan seçmeli sorular
- Açık uçlu sorular
- Kod yazma
- Mini projeler
- Vaka analizi
- Simülasyon
- Eşleştirme
- Teach Back
- AI ile diyalog
- Gerçek hayat senaryoları

---

# 5. Dinamik Değerlendirme

Sistem tek bir sınav yerine çoklu kanıt toplar.

Örnek kanıtlar:

- Quiz sonucu
- Kod kalitesi
- Görev tamamlama
- Açık uçlu cevap
- Reflection
- Uzun dönem tekrar başarısı

---

# 6. Başarısızlık Yönetimi

Başarısızlık durumunda sistem:

1. Eksik Knowledge Node'ları belirler.
2. Ön koşulları yeniden kontrol eder.
3. Alternatif öğretim stratejisi seçer.
4. Yeni görevler oluşturur.
5. Gerekirse Learning Path'i günceller.

---

# 7. Mastery Kararı

Mastery tek bir sınava göre verilmez.

Karar aşağıdaki kanıtların birleşimine dayanır:

- Assessment sonuçları
- Teach Back başarısı
- Görev performansı
- Uzun dönem tekrar sonuçları
- Bilgiyi farklı bağlamlarda kullanabilme

---

# 8. AI'nin Rolü

AI;

- değerlendirme hazırlayabilir,
- açık uçlu cevapları analiz edebilir,
- kişiselleştirilmiş geri bildirim üretebilir,
- ek çalışma önerileri sunabilir.

Son Mastery kararı, tanımlı iş kuralları ve toplanan kanıtlar doğrultusunda verilir.

---

# 9. Başarı Ölçütü

Learning Validation Engine başarılıdır, eğer:

- yanlış pozitif (öğrenmediği hâlde öğrenmiş görünme) oranı azalır,
- kullanıcı eksiklerini doğru tespit ederse,
- öğrenme yolunu doğru güncellerse,
- uzun dönem öğrenmeyi desteklerse.

---

# 10. Sonuç

Learning Validation Engine, MEF'in kalite güvencesidir.

Platformun amacı sınav yapmak değil, öğrenmeyi güvenilir şekilde doğrulamaktır.
