# DOMAIN-005 — Business Rules

| Alan | Değer |
|------|--------|
| Belge Kodu | DOMAIN-005 |
| Belge Adı | Business Rules |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | DOMAIN-000, DOMAIN-001, DOMAIN-002, DOMAIN-003, DOMAIN-004 |

---

# 1. Amaç

Bu belge, MEF'in değişmez iş kurallarını tanımlar.

İş kuralları teknolojiye, kullanıcı arayüzüne veya kullanılan yapay zekâ modeline bağlı değildir.

Platformun tüm katmanları bu kurallara uymak zorundadır.

---

# 2. Temel İlkeler

1. Öğrenme, içerik tüketmek değildir.
2. Öğrenme ölçülebilir olmalıdır.
3. Bilgi tek başına yeterli değildir; beceriye dönüşmelidir.
4. Her öğrenme hedefinin doğrulanabilir bir çıktısı olmalıdır.
5. Kullanıcının ilerlemesi kanıtlarla desteklenmelidir.

---

# 3. Learner Kuralları

### BR-001

Her Learner en az bir aktif veya tamamlanmış Learning Goal'a sahip olabilir.

---

### BR-002

Bir Learner aynı anda birden fazla Learning Goal yürütebilir.

---

### BR-003

Her Learner'ın ilerleme geçmişi silinmez; yalnızca arşivlenebilir.

---

# 4. Learning Goal Kuralları

### BR-004

Learning Goal açık ve ölçülebilir olmalıdır.

Yanlış örnek:

> Yazılım öğrenmek.

Doğru örnek:

> REST API geliştirebilecek seviyeye gelmek.

---

### BR-005

Her Learning Goal en az bir Knowledge Node ile ilişkilendirilmelidir.

---

### BR-006

Bir Learning Goal tamamlanmadan önce gerekli Assessment'lar başarıyla tamamlanmalıdır.

---

# 5. Knowledge Kuralları

### BR-007

Knowledge Node benzersizdir.

Aynı kavram sistemde iki kez oluşturulamaz.

---

### BR-008

Knowledge Node kendi ön koşullarını tanımlayabilir.

---

### BR-009

Döngüsel ön koşul oluşturulamaz.

Örnek:

A → B → C → A ❌

---

# 6. Assessment Kuralları

### BR-010

Her Assessment belirli bir Learning Goal ile ilişkilidir.

---

### BR-011

Assessment sonucu değiştirilemez.

İtiraz veya yeniden değerlendirme yeni bir Assessment oluşturur.

---

### BR-012

Assessment yalnızca puan üretmez; açıklayıcı geri bildirim de üretmelidir.

---

# 7. Mastery Kuralları

### BR-013

Mastery yalnızca başarılı Assessment sonuçlarıyla yükselir.

---

### BR-014

Uzun süre kullanılmayan becerilerde Mastery seviyesi yeniden değerlendirilebilir.

Bu değerlendirme otomatik düşüş yerine yeniden doğrulama gerektirebilir.

---

# 8. Memory Kuralları

### BR-015

Her önemli öğrenme çıktısı için tekrar planı oluşturulmalıdır.

---

### BR-016

Tekrar tamamlandığında Memory kaydı güncellenmelidir.

---

### BR-017

Tekrar planı kişiselleştirilmelidir.

Aynı plan tüm kullanıcılar için uygulanmaz.

---

# 9. Feedback Kuralları

### BR-018

Her Assessment sonrasında Feedback üretilmelidir.

---

### BR-019

Feedback yapıcı, açıklayıcı ve geliştirici olmalıdır.

---

### BR-020

Feedback yalnızca hata değil, güçlü yönleri de göstermelidir.

---

# 10. Learning Path Kuralları

### BR-021

Learning Path dinamiktir.

Kullanıcının performansına göre değişebilir.

---

### BR-022

Eksik ön koşullar tespit edilirse sistem yeni adımlar ekleyebilir.

---

### BR-023

Learning Path, kullanıcı hedefi değiştiğinde yeniden hesaplanmalıdır.

---

# 11. Genel Kurallar

### BR-024

Hiçbir kullanıcı öğrenmeye zorlanamaz.

Sistem öneride bulunur, karar kullanıcıya aittir.

---

### BR-025

Yapay zekâ tarafından üretilen içerikler gerektiğinde yeniden üretilebilir.

Sabit içerik zorunlu değildir.

---

### BR-026

Platformun temel başarı ölçütü içerik tüketimi değil, doğrulanmış öğrenmedir.

---

# 12. Sonuç

Bu iş kuralları, MEF'in değişmez davranışlarını tanımlar.

Application Service'ler, API'ler, kullanıcı arayüzü ve AI ajanları bu kuralları ihlal edemez.

Yeni kurallar eklendiğinde bu belge güncellenmeli ve ilgili mimari karar kayıtları (ADR) gözden geçirilmelidir.
