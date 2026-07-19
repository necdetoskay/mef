# ADR-001 — Learning Operating System

| Alan | Değer |
|------|--------|
| Durum | Accepted |
| Tarih | 2026-07-19 |
| Karar Sahibi | MEF Architecture Team |

---

# Başlık

MEF, klasik bir LMS (Learning Management System) olarak değil, Learning Operating System (LOS) olarak tasarlanacaktır.

---

# Bağlam

Mevcut LMS platformları çoğunlukla:

- içerik sunar,
- sınav yapar,
- rapor üretir.

Öğrenme kararları büyük ölçüde kullanıcıya bırakılır.

MEF'in hedefi ise öğrenme sürecini aktif olarak yöneten bir sistem oluşturmaktır.

---

# Karar

MEF;

- öğrenme hedeflerini analiz eder,
- eksikleri belirler,
- öğrenme yolu oluşturur,
- öğretim stratejisini seçer,
- öğrenmeyi doğrular,
- tekrar planlar,
- bir sonraki adımı önerir.

Bu nedenle sistem "Learning Operating System" yaklaşımıyla geliştirilecektir.

---

# Sonuçlar

Avantajlar

- Modüler yapı
- Genişletilebilir mimari
- AI bağımsızlığı
- Karar odaklı tasarım

Riskler

- Daha karmaşık mimari
- Daha fazla entegrasyon ihtiyacı
- İlk geliştirme maliyetinin artması

---

# Durum

Bu karar, sistemin tüm mimari tasarımını etkileyen temel ilkedir.
