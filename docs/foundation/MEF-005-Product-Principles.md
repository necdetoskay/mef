# MEF-005 — Product Principles

| Alan | Değer |
|------|--------|
| Belge Kodu | MEF-005 |
| Belge Adı | Product Principles |
| Durum | Approved |
| Sürüm | 1.0.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | MEF-000, MEF-001, MEF-002, MEF-003, MEF-004 |

---

# 1. Amaç

Bu belge, MEF geliştirilirken alınacak ürün kararlarının temel ilkelerini tanımlar.

Her yeni özellik, tasarım kararı veya teknik geliştirme bu ilkeler doğrultusunda değerlendirilmelidir.

---

# 2. Karar Verme İlkesi

MEF'te her özellik şu soruyla değerlendirilir:

> **Bu özellik kullanıcının daha iyi öğrenmesini sağlıyor mu?**

Eğer cevap net bir "Evet" değilse, özellik yeniden değerlendirilmelidir.

---

# 3. Temel Ürün İlkeleri

## 3.1 Öğrenme Önceliklidir

MEF içerik üretme platformu değildir.

MEF öğrenme platformudur.

---

## 3.2 Kullanıcı Merkezlidir

Kullanıcı sisteme uyum sağlamaz.

Sistem kullanıcıya uyum sağlar.

---

## 3.3 Basitlik

Her ekran, her özellik ve her akış mümkün olduğunca sade olmalıdır.

Karmaşıklık, kullanıcıya değil sisteme ait olmalıdır.

---

## 3.4 Kişiselleştirme

Aynı içerik herkese sunulmaz.

Her kullanıcı için farklı öğrenme yolu oluşturulur.

---

## 3.5 Ölçülebilirlik

Her öğrenme hedefinin başarı kriteri olmalıdır.

Sistem, öğrenmenin gerçekleştiğini kanıtlayabilmelidir.

---

## 3.6 Geri Bildirim

Kullanıcı yalnızca doğru veya yanlış cevabı görmez.

Neden doğru, neden yanlış olduğunu da öğrenir.

---

## 3.7 Süreklilik

Öğrenme bir oturumla bitmez.

Platform, kullanıcının uzun vadeli gelişimini destekler.

---

# 4. Teknik İlkeler

Ürün geliştirilirken aşağıdaki prensipler korunacaktır:

- Modüler mimari
- API First yaklaşımı
- AI bağımsız çekirdek mimari
- Ölçeklenebilir altyapı
- Güvenlik önceliği
- Test edilebilir bileşenler

---

# 5. Kullanıcı Deneyimi İlkeleri

MEF'in kullanıcı deneyimi şu hedefleri taşımalıdır:

- İlk kullanımdan itibaren anlaşılır olmak
- Gereksiz adımları azaltmak
- Kullanıcıyı motive etmek
- Başarı hissini görünür kılmak
- Hataları öğretme fırsatına dönüştürmek

---

# 6. Yapay Zekâ İlkeleri

Yapay zekâ;

- Karar verici değil, rehberdir.
- Açıklanabilir olmalıdır.
- Kullanıcının yerine öğrenmez.
- Kullanıcıyı bağımlı hâle getirmemelidir.
- Öğrenme sürecini desteklemelidir.

---

# 7. Ürün Red Kriterleri

Aşağıdaki özellikler reddedilmelidir:

- Öğrenmeye katkısı olmayan özellikler
- Sadece gösteriş amacı taşıyan geliştirmeler
- Gereksiz karmaşıklık oluşturan tasarımlar
- Ölçülemeyen başarı hedefleri

---

# 8. Sonuç

MEF'in başarısı, eklenen özellik sayısıyla değil; kullanıcıların kazandığı bilgi, beceri ve özgüven ile ölçülür.

Bu belge, gelecekte alınacak tüm ürün kararları için temel referans olacaktır.

---

## Sonraki Belge

**PRD-000 — Product Requirements Document**
