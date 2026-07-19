# LFS-004 — Teaching Strategy Engine

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-004 |
| Belge Adı | Teaching Strategy Engine |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-001, LFS-002, LFS-003 |

---

# 1. Amaç

Teaching Strategy Engine (TSE), bir konunun kullanıcıya hangi yöntemle sunulacağına karar veren bileşendir.

MEF aynı bilgiyi tek bir biçimde sunmaz.

Sistem, kullanıcının önceki öğrenme performansını analiz ederek en uygun öğretim stratejisini seçer ve gerektiğinde değiştirir.

---

# 2. Temel İlke

Her bilgi birden fazla yöntemle öğretilebilir.

Başarısız olan yöntem tekrar edilmek zorunda değildir.

Sistem alternatif stratejiler deneyebilir.

---

# 3. Öğretim Stratejileri

Her Knowledge Node aşağıdaki stratejilerden biri veya birkaçıyla anlatılabilir.

### TS-001

Klasik açıklama

---

### TS-002

Adım adım anlatım

---

### TS-003

Günlük yaşam benzetmeleri

---

### TS-004

Hikâyeleştirme

---

### TS-005

Sokratik yöntem

---

### TS-006

Görsel anlatım

---

### TS-007

İnteraktif uygulama

---

### TS-008

Mini proje

---

### TS-009

Gerçek hayat senaryosu

---

### TS-010

Soru-cevap oturumu

---

### TS-011

Öğrencinin öğretmesi ("Teach Back")

Kullanıcıdan konuyu kendi cümleleriyle anlatması istenir.

---

# 4. Strateji Seçimi

Sistem aşağıdaki sinyalleri değerlendirir:

- Assessment sonuçları
- Öğrenme süresi
- Tekrar sayısı
- İpucu kullanımı
- Kullanıcının geri bildirimi
- Reflection cevapları
- Uzun dönem hatırlama başarısı

Bu sinyaller tek başına kesin karar vermez; birlikte değerlendirilir.

---

# 5. Strateji Değiştirme Kuralları

Aşağıdaki durumlarda strateji değişikliği önerilebilir:

- Aynı konuda art arda başarısızlık
- Çok düşük ilerleme
- Kullanıcının "anlamadım" geri bildirimi
- Uzun süre aynı noktada kalma
- Tekrarlara rağmen düşük kalıcılık

---

# 6. Teach Back

Teach Back, MEF'in temel doğrulama yöntemlerinden biridir.

Kullanıcıdan;

- konuyu açıklaması,
- örnek vermesi,
- problemi çözmesi,
- başka birine anlatıyormuş gibi anlatması

istenebilir.

Bu yöntem, anlamayı ezberden ayırmaya yardımcı olur.

---

# 7. Strateji Performansı

Her strateji anonim ve toplu kullanım verileri üzerinden değerlendirilebilir.

Örneğin:

- Ortalama başarı oranı
- Ortalama tamamlanma süresi
- Uzun dönem hatırlama başarısı

Bu veriler yeni stratejilerin geliştirilmesine yardımcı olur.

---

# 8. AI'nin Rolü

AI;

- seçilen stratejiye uygun içerik üretir,
- örnekleri kişiselleştirir,
- farklı açıklamalar oluşturur,
- kullanıcıya uygun görevler hazırlar.

AI öğretim yöntemini tek başına belirlemez; Teaching Strategy Engine'in kararlarını uygular.

---

# 9. Başarı Ölçütü

Bir strateji başarılı kabul edilir, eğer:

- Mastery seviyesi artıyorsa,
- tekrar ihtiyacı azalıyorsa,
- uzun dönem hatırlama güçleniyorsa,
- kullanıcı hedefe daha verimli ulaşıyorsa.

---

# 10. Sonuç

Teaching Strategy Engine, MEF'in adaptif öğretim mekanizmasının merkezidir.

Aynı bilgi, farklı kullanıcılar için farklı yollarla sunulabilir.

Sistem zamanla hangi stratejilerin hangi durumlarda daha etkili olduğunu öğrenerek sürekli gelişir.
