# DOMAIN-002 — Bounded Contexts

| Alan | Değer |
|------|--------|
| Belge Kodu | DOMAIN-002 |
| Belge Adı | Bounded Contexts |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | DOMAIN-000, DOMAIN-001 |

---

# 1. Amaç

Bu belge, MEF'in iş alanını bağımsız sorumluluk bölgelerine (Bounded Contexts) ayırır.

Her Context;

- kendi kurallarına,
- kendi veri modeline,
- kendi servislerine,
- kendi API'lerine

sahiptir.

Bir Context, başka bir Context'in iç mantığını bilmez; yalnızca tanımlı arayüzler üzerinden iletişim kurar.

---

# 2. Context Haritası

```text
                           +----------------------+
                           |   Identity Context   |
                           +----------+-----------+
                                      |
                                      v
+------------------+        +----------------------+       +----------------------+
| Learner Context  |<------>| Learning Context     |<----->| Knowledge Context    |
+------------------+        +----------------------+       +----------------------+
           |                          |
           |                          |
           v                          v
+------------------+        +----------------------+
| Assessment       |<------>| Memory Context       |
| Context          |        +----------------------+
+------------------+                 |
                                     |
                                     v
                          +----------------------+
                          | Analytics Context    |
                          +----------------------+
                                     |
                                     v
                          +----------------------+
                          | AI Context           |
                          +----------------------+
```

---

# 3. Context Tanımları

## Identity Context

Sorumlulukları:

- Kimlik doğrulama
- Yetkilendirme
- Roller
- Organizasyon yapısı
- Oturum yönetimi

---

## Learner Context

Sorumlulukları:

- Kullanıcı profili
- Öğrenme tercihleri
- Hedefler
- İlerleme özeti

Bu Context, kullanıcının kim olduğunu değil; nasıl öğrendiğini bilir.

---

## Knowledge Context

Sorumlulukları:

- Bilgi düğümleri
- Ön koşullar
- Bilgi ilişkileri
- Bilgi grafı
- Kavram haritası

Bu Context içerik üretmez; bilgi yapısını yönetir.

---

## Learning Context

MEF'in çekirdeğidir.

Sorumlulukları:

- Learning Path oluşturmak
- Öğrenme oturumlarını yönetmek
- Adaptif öğrenme kararları almak
- Öğretim stratejisini belirlemek

---

## Assessment Context

Sorumlulukları:

- Quiz
- Açık uçlu değerlendirme
- Kod değerlendirme
- Proje değerlendirme
- Puanlama
- Mastery hesaplama

---

## Memory Context

Sorumlulukları:

- Tekrar planları
- Unutma tahmini
- Hatırlatma zamanlaması
- Bilgi kalıcılığı

---

## Analytics Context

Sorumlulukları:

- Öğrenme analitiği
- Performans raporları
- Gelişim grafikleri
- Sistem metrikleri

---

## AI Context

Sorumlulukları:

- AI Teacher
- AI Mentor
- AI Reviewer
- İçerik üretimi
- Geri bildirim üretimi
- Model yönetimi

Bu Context, öğrenme kararlarını tek başına vermez; Learning Context ile birlikte çalışır.

---

# 4. Context İletişim Kuralları

- Context'ler doğrudan veritabanı paylaşmaz.
- Her Context kendi veri bütünlüğünden sorumludur.
- İletişim API veya olaylar (events) üzerinden yapılır.
- İç mantık başka Context'lere açılmaz.

---

# 5. Gelecek Genişlemeler

İlerleyen sürümlerde aşağıdaki Context'ler eklenebilir:

- Collaboration Context
- Gamification Context
- Marketplace Context
- Notification Context
- Institution Context
- Certification Context
- Content Management Context

---

# 6. Tasarım İlkeleri

- Düşük bağımlılık (Low Coupling)
- Yüksek uyum (High Cohesion)
- Açık sorumluluk sınırları
- Genişletilebilir yapı
- Test edilebilir servisler

---

# 7. Sonuç

Bu belge, MEF'in iş alanını mantıksal parçalara ayırır.

Tüm mimari, servis tasarımı ve veri modeli bu sınırlar dikkate alınarak geliştirilecektir.
