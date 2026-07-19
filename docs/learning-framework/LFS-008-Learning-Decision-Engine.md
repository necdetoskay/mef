# LFS-008 — Learning Decision Engine

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-008 |
| Belge Adı | Learning Decision Engine |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-002, LFS-003, LFS-004, LFS-005, LFS-006, LFS-007 |

---

# 1. Amaç

Learning Decision Engine (LDE), MEF'in merkezi karar verme bileşenidir.

LDE'nin görevi, mevcut öğrenme kanıtlarını analiz ederek kullanıcı için en uygun bir sonraki öğrenme adımını belirlemektir.

---

# 2. Temel İlkeler

- Kararlar tek bir veriye dayanmaz.
- Birden fazla öğrenme kanıtı birlikte değerlendirilir.
- Kararlar açıklanabilir olmalıdır.
- Kullanıcı öneriyi kabul veya reddedebilir.
- Her karar yeniden değerlendirilebilir.

---

# 3. Girdi Kaynakları

LDE aşağıdaki sistemlerden veri alır:

- Knowledge Graph
- Learning Path
- Teaching Strategy Engine
- Learning Validation Engine
- Memory Engine
- Reflection Engine
- Learner Profile

---

# 4. Üretebileceği Kararlar

LDE aşağıdaki önerileri oluşturabilir:

- Bir sonraki konuya geç.
- Aynı konuyu farklı yöntemle tekrar et.
- Ön koşul konusuna geri dön.
- Mini proje yap.
- Kısa tekrar planla.
- Değerlendirme uygula.
- Dinlenme öner.
- Öğrenme hızını değiştir.
- Yeni öğrenme hedefi öner.

---

# 5. Karar Akışı

```text
Assessment
      │
Memory Engine
      │
Reflection
      │
Teaching Strategy
      │
Knowledge Graph
      │
Learner Profile
      │
      ▼
Learning Decision Engine
      │
      ▼
Next Best Learning Action
```

---

# 6. Karar Açıklanabilirliği

Her öneri kullanıcıya açıklanabilir olmalıdır.

Örnek:

"Son iki değerlendirmede Docker Volume konusunda zorlandığın ve son tekrarının üzerinden 18 gün geçtiği için önce kısa bir uygulama öneriyorum."

Bu sayede kullanıcı sistemin neden bu öneriyi yaptığını anlayabilir.

---

# 7. Önceliklendirme

Birden fazla öneri mümkün olduğunda LDE;

1. Kritik eksikleri,
2. Yaklaşan unutma riskini,
3. Öğrenme hedeflerini,
4. Kullanıcının zamanını,
5. Motivasyon durumunu

birlikte değerlendirerek öncelik sıralaması oluşturur.

---

# 8. AI'nin Rolü

AI;

- karar için gerekli analizleri destekleyebilir,
- alternatif öğrenme yolları önerebilir,
- açıklamaları kişiselleştirebilir.

Nihai karar, LDE'nin tanımlı kuralları ve öğrenme kanıtları doğrultusunda verilir.

---

# 9. Başarı Ölçütü

LDE başarılıdır, eğer:

- kullanıcı gereksiz tekrar yapmıyorsa,
- öğrenme süresi verimli kullanılıyorsa,
- Mastery artıyorsa,
- uzun dönem bilgi kalıcılığı iyileşiyorsa,
- öneriler kullanıcı tarafından anlamlı bulunuyorsa.

---

# 10. Sonuç

Learning Decision Engine, MEF'in merkezi karar mekanizmasıdır.

Platformun diğer bileşenlerinden gelen verileri birleştirerek kişiselleştirilmiş, açıklanabilir ve sürekli güncellenen öğrenme kararları üretir.
