# DOMAIN-004 — Domain Events

| Alan | Değer |
|------|--------|
| Belge Kodu | DOMAIN-004 |
| Belge Adı | Domain Events |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | DOMAIN-000, DOMAIN-001, DOMAIN-002, DOMAIN-003 |

---

# 1. Amaç

Bu belge, MEF içerisinde gerçekleşen önemli iş olaylarını (Domain Events) tanımlar.

Domain Event'ler, sistemin iş açısından anlamlı değişikliklerini temsil eder.

Teknik olaylardan (ör. HTTP isteği veya veritabanı güncellemesi) farklı olarak, Domain Event'ler iş dilini kullanır.

---

# 2. Event Tasarım İlkeleri

Bir Domain Event:

- Geçmiş zamanda isimlendirilir.
- İş açısından anlamlıdır.
- Değiştirilemez (Immutable).
- Gerçekleşmiş bir olayı temsil eder.

Örnek:

✅ `LearningGoalCreated`

❌ `CreateLearningGoal`

---

# 3. Learner Event'leri

### LearnerRegistered

Yeni bir kullanıcı sisteme kaydoldu.

---

### LearnerProfileUpdated

Kullanıcının profil bilgileri güncellendi.

---

### LearningPreferencesUpdated

Öğrenme tercihleri değiştirildi.

---

# 4. Learning Goal Event'leri

### LearningGoalCreated

Yeni bir öğrenme hedefi oluşturuldu.

---

### LearningGoalStarted

Öğrenme hedefi aktif hâle geldi.

---

### LearningGoalPaused

Öğrenme hedefi geçici olarak durduruldu.

---

### LearningGoalCompleted

Hedef başarıyla tamamlandı.

---

### LearningGoalCancelled

Hedef kullanıcı tarafından iptal edildi.

---

# 5. Learning Event'leri

### LearningPathGenerated

Kişiselleştirilmiş öğrenme yolu oluşturuldu.

---

### LearningSessionStarted

Yeni bir öğrenme oturumu başladı.

---

### LearningSessionCompleted

Öğrenme oturumu tamamlandı.

---

### LearnerStuckDetected

Sistem, kullanıcının ilerlemekte zorlandığını tespit etti.

---

### LearningStrategyChanged

Sistem, öğretim yöntemini değiştirdi.

Örnek:

- metin → görsel
- teori → uygulama
- açıklama → benzetme

---

# 6. Assessment Event'leri

### AssessmentStarted

Değerlendirme başlatıldı.

---

### AssessmentCompleted

Değerlendirme tamamlandı.

---

### AssessmentFailed

Başarı kriteri sağlanamadı.

---

### AssessmentPassed

Başarı kriteri sağlandı.

---

### MasteryLevelChanged

Yeterlilik seviyesi güncellendi.

---

### MasteryAchieved

Belirlenen yeterlilik seviyesine ulaşıldı.

---

# 7. Memory Event'leri

### ReviewScheduled

Tekrar planı oluşturuldu.

---

### ReviewCompleted

Tekrar tamamlandı.

---

### RetentionScoreUpdated

Bilgi kalıcılığı puanı güncellendi.

---

### ForgettingRiskDetected

Sistem unutma riskini tespit etti.

---

# 8. AI Event'leri

### AIExplanationRequested

Kullanıcı yeni bir açıklama istedi.

---

### AIExplanationGenerated

Yeni anlatım oluşturuldu.

---

### AIFeedbackGenerated

Yapay zekâ kişiselleştirilmiş geri bildirim hazırladı.

---

### AIRecommendationGenerated

Yeni öğrenme önerisi üretildi.

---

# 9. Analytics Event'leri

### ProgressUpdated

İlerleme bilgisi güncellendi.

---

### LearningMilestoneReached

Önemli bir öğrenme kilometre taşı tamamlandı.

---

### LearningReportGenerated

Rapor oluşturuldu.

---

# 10. Event Zinciri Örneği

```text
LearningGoalCreated
        │
        ▼
LearningPathGenerated
        │
        ▼
LearningSessionStarted
        │
        ▼
AssessmentCompleted
        │
        ▼
AssessmentPassed
        │
        ▼
MasteryLevelChanged
        │
        ▼
ReviewScheduled
```

Bu zincir, tek bir öğrenme döngüsünün örnek akışını gösterir.

---

# 11. Gelecekte Eklenebilecek Event'ler

- MissionAssigned
- MissionCompleted
- ReflectionSubmitted
- BadgeEarned
- CertificateIssued
- CollaborationStarted
- MentorRequested
- StudyGroupJoined
- ContentUpdated
- KnowledgeGraphExpanded

---

# 12. Sonuç

Domain Event'ler, MEF'in iş süreçlerinin ortak dilidir.

Application Service'ler, Workflow'lar, bildirim sistemi, analitik altyapısı ve AI ajanları bu olayları referans alarak çalışacaktır.
