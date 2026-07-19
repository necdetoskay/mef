# LFS-006 — Memory Engine

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-006 |
| Belge Adı | Memory Engine |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-001, LFS-002, LFS-003, LFS-005 |

---

# 1. Amaç

Memory Engine, öğrenilen bilgilerin uzun süre korunmasını destekleyen sistemdir.

Amaç, kullanıcıya rastgele tekrar yaptırmak değil; doğru bilgiyi, doğru zamanda ve doğru yöntemle yeniden karşısına çıkarmaktır.

---

# 2. Temel İlkeler

- Unutmak öğrenmenin doğal bir parçasıdır.
- Tekrarlar kişiselleştirilmelidir.
- Her konu aynı sıklıkta tekrar edilmez.
- Tekrarın amacı ezber değil, geri çağırmadır (active recall).
- Kalıcılık zaman içinde yeniden değerlendirilmelidir.

---

# 3. Memory Döngüsü

Her Knowledge Node aşağıdaki yaşam döngüsünü izler:

```text
İlk Öğrenme
      │
      ▼
İlk Doğrulama
      │
      ▼
Tekrar Planı
      │
      ▼
Geri Çağırma (Recall)
      │
      ▼
Yeni Değerlendirme
      │
      ▼
Kalıcılık Güncellemesi
      │
      ▼
Yeni Tekrar Tarihi
```

Bu döngü, kullanıcı konuyu kalıcı biçimde öğrenene kadar devam eder.

---

# 4. Tekrar Tetikleyicileri

Sistem aşağıdaki durumlarda tekrar planlayabilir:

- Belirli bir süre geçtiğinde
- Unutma riski arttığında
- İlgili yeni bir konuya geçileceğinde
- Aynı bilgi başka bir bağlamda kullanılacağında
- Kullanıcı tekrar talep ettiğinde

---

# 5. Tekrar Türleri

Memory Engine farklı tekrar yöntemleri kullanabilir.

### MR-001

Kısa soru

---

### MR-002

Açık uçlu cevap

---

### MR-003

Teach Back

---

### MR-004

Mini görev

---

### MR-005

Gerçek hayat senaryosu

---

### MR-006

Problem çözme

---

### MR-007

Önceki hataları yeniden değerlendirme

---

# 6. Kalıcılık Göstergeleri

Her Knowledge Node için sistem aşağıdaki göstergeleri takip edebilir:

- Son doğrulama tarihi
- Son tekrar tarihi
- Başarı oranı
- Tekrar sayısı
- Tahmini unutma riski
- Geri çağırma başarısı
- Mastery seviyesi

Bu göstergeler birlikte değerlendirilir; tek bir metrik üzerinden karar verilmez.

---

# 7. Adaptif Tekrar

İki kullanıcı aynı tekrar planını almak zorunda değildir.

Sistem;

- öğrenme hızını,
- başarı geçmişini,
- unutma eğilimini,
- hedeflerini

dikkate alarak kişiselleştirilmiş tekrar planı oluşturur.

---

# 8. AI'nin Rolü

AI;

- yeni tekrar soruları oluşturabilir,
- farklı örnekler üretebilir,
- önceki hatalara göre içerik hazırlayabilir,
- tekrar görevlerini çeşitlendirebilir.

Tekrar zamanlaması ve iş kuralları Memory Engine tarafından yönetilir.

---

# 9. Başarı Ölçütü

Memory Engine başarılıdır, eğer:

- uzun dönem hatırlama oranı artıyorsa,
- gereksiz tekrarlar azalıyorsa,
- kullanıcı bilgiyi yeni durumlarda kullanabiliyorsa,
- unutma riski doğru tahmin edilebiliyorsa.

---

# 10. Gelecek Genişletmeler

İlerleyen sürümlerde Memory Engine;

- günlük çalışma planı,
- konu önceliklendirme,
- hedef bazlı tekrar,
- grup çalışmaları,
- AI destekli kişisel tekrar koçu

gibi özelliklerle genişletilebilir.

---

# 11. Sonuç

Memory Engine, MEF'in uzun dönem öğrenme stratejisinin temel bileşenidir.

Platformun amacı yalnızca bilgi sunmak değil, bilginin zaman içinde kullanılabilir kalmasını desteklemektir.
