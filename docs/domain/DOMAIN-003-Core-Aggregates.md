# DOMAIN-003 — Core Aggregates

| Alan | Değer |
|------|--------|
| Belge Kodu | DOMAIN-003 |
| Belge Adı | Core Aggregates |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | DOMAIN-000, DOMAIN-001, DOMAIN-002 |

---

# 1. Amaç

Bu belge, MEF Domain'inin temel Aggregate'lerini tanımlar.

Aggregate, birlikte yönetilen ve tutarlılığı (consistency) korunması gereken iş nesnelerinin sınırıdır.

Her Aggregate tek bir **Aggregate Root** tarafından yönetilir.

---

# 2. Aggregate Nedir?

Aggregate;

- iş kurallarının uygulandığı,
- veri bütünlüğünün korunduğu,
- tek bir yaşam döngüsüne sahip

bir nesne grubudur.

Dış sistemler yalnızca Aggregate Root ile iletişim kurabilir.

---

# 3. Learner Aggregate

## Aggregate Root

**Learner**

### İçerdiği Varlıklar

- Learner Profile
- Learning Preferences
- Learning Goals
- Progress Summary
- Achievement History

### Sorumlulukları

- Öğrenme hedeflerini yönetmek
- Tercihleri saklamak
- İlerlemeyi takip etmek
- Başarı geçmişini korumak

---

# 4. Knowledge Aggregate

## Aggregate Root

**Knowledge Node**

### İçerdiği Varlıklar

- Concept
- Prerequisites
- Related Knowledge
- Difficulty
- Learning Outcomes

### Sorumlulukları

- Bilgi düğümünü yönetmek
- Ön koşulları tanımlamak
- Bilgi ilişkilerini korumak

---

# 5. Learning Aggregate

## Aggregate Root

**Learning Journey**

### İçerdiği Varlıklar

- Learning Path
- Learning Session
- Current Stage
- Active Mission
- Learning History

### Sorumlulukları

- Öğrenme yolculuğunu yönetmek
- Aktif görevi belirlemek
- Öğrenme geçmişini tutmak

---

# 6. Assessment Aggregate

## Aggregate Root

**Assessment**

### İçerdiği Varlıklar

- Questions
- Answers
- Evaluation
- Feedback
- Mastery Result

### Sorumlulukları

- Değerlendirmeyi yürütmek
- Sonucu hesaplamak
- Geri bildirim üretmek

---

# 7. Memory Aggregate

## Aggregate Root

**Memory Profile**

### İçerdiği Varlıklar

- Review Schedule
- Retention Score
- Forgetting Risk
- Review History

### Sorumlulukları

- Tekrar planı oluşturmak
- Bilgi kalıcılığını takip etmek
- Hatırlatma zamanlarını yönetmek

---

# 8. AI Aggregate

## Aggregate Root

**AI Learning Assistant**

### İçerdiği Bileşenler

- AI Teacher
- AI Mentor
- AI Reviewer
- AI Planner

### Sorumlulukları

- Öğretim stratejisini uygulamak
- Geri bildirim oluşturmak
- Kullanıcıya rehberlik etmek

Not: Bu Aggregate, iş kurallarını belirlemez; Learning Context tarafından alınan kararları uygular.

---

# 9. Aggregate İlişkileri

```text
Learner
   │
   ├── owns ─────────► Learning Journey
   │                      │
   │                      ├── uses ─────► Knowledge Node
   │                      │
   │                      ├── triggers ─► Assessment
   │                      │
   │                      └── updates ──► Memory Profile
   │
   └── interacts ────────► AI Learning Assistant
```

---

# 10. Aggregate Kuralları

1. Her Aggregate yalnızca kendi verisini değiştirir.
2. Aggregate'ler birbirlerinin iç nesnelerine doğrudan erişmez.
3. Aggregate'ler arası iletişim Domain Event veya Application Service üzerinden yapılır.
4. Her Aggregate bağımsız test edilebilir olmalıdır.

---

# 11. Sonuç

Bu belge, MEF'in temel iş nesnelerinin sınırlarını tanımlar.

Veritabanı modeli, API tasarımı ve servis mimarisi bu Aggregate yapısını referans alacaktır.
