# LFS-010 — Learning Analytics & Insights

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-010 |
| Belge Adı | Learning Analytics & Insights |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-001 ... LFS-009 |

---

# 1. Amaç

Learning Analytics & Insights bileşeni, öğrenme sürecinden elde edilen verileri analiz ederek kullanıcıya, eğitmene ve sisteme anlamlı içgörüler sunar.

Amaç yalnızca geçmişi raporlamak değil, gelecekteki öğrenmeyi iyileştirecek öneriler üretmektir.

---

# 2. Temel İlkeler

- Analizler açıklanabilir olmalıdır.
- Kullanıcıya eyleme dönüştürülebilir öneriler sunulmalıdır.
- Analizler birden fazla veri kaynağına dayanmalıdır.
- Gizlilik ve veri güvenliği korunmalıdır.

---

# 3. Veri Kaynakları

Learning Analytics aşağıdaki kaynaklardan beslenebilir:

- Learning Path geçmişi
- Assessment sonuçları
- Multi-Dimensional Mastery profili
- Memory Engine verileri
- Reflection sonuçları
- Teaching Strategy performansı
- Öğrenme oturumu kayıtları
- Kullanıcının açık geri bildirimleri

---

# 4. Analiz Türleri

## LA-001 İlerleme Analizi

- Hedef tamamlama oranı
- Öğrenme hızı
- Tamamlanan Knowledge Node sayısı

---

## LA-002 Öğrenme Kalitesi

- Mastery gelişimi
- Bilgi Sağlığı eğilimi
- Uzun dönem kalıcılık

---

## LA-003 Risk Analizi

- Unutma riski yüksek konular
- Uzun süredir çalışılmayan alanlar
- Sürekli başarısız olunan düğümler

---

## LA-004 Verimlilik Analizi

- Hangi öğretim stratejileri daha başarılı?
- Hangi görev türleri daha etkili?
- Ortalama hedef tamamlama süresi

---

## LA-005 Hedef Analizi

- Hedefe kalan tahmini süre
- Kritik eksikler
- Öncelikli çalışma önerileri

---

# 5. İçgörü (Insight) Üretimi

Sistem yalnızca veri göstermez.

Örnek içgörüler:

- "Son üç haftada ağ teknolojileri konularında istikrarlı gelişim gösterdin."
- "Docker Compose konusunda tekrar yapılması öneriliyor."
- "Mini proje temelli çalışmalar sende daha yüksek başarı sağlıyor."

---

# 6. Tahmine Dayalı Analiz

Gelecek sürümlerde sistem aşağıdaki tahminleri üretebilir:

- Tahmini hedef tamamlama tarihi
- Beklenen unutma riski
- Muhtemel zorlanma noktaları
- Tekrar öncelikleri

Bu tahminler kullanıcıya kesin sonuç olarak değil, olasılık ve güven düzeyiyle sunulmalıdır.

---

# 7. Kullanıcıya Sunum

Analytics aşağıdaki biçimlerde gösterilebilir:

- Günlük özet
- Haftalık rapor
- Aylık gelişim raporu
- Knowledge Health haritası
- Mastery profili
- AI koç önerileri

---

# 8. AI'nin Rolü

AI;

- raporları sade bir dille açıklayabilir,
- önemli değişimleri özetleyebilir,
- önerileri kişiselleştirebilir.

AI, analiz sonuçlarını yorumlar; ham verileri değiştirmez.

---

# 9. Başarı Ölçütü

Learning Analytics başarılıdır, eğer:

- kullanıcı doğru öncelikleri belirleyebiliyorsa,
- öneriler öğrenme verimliliğini artırıyorsa,
- kullanıcı gelişimini açıkça takip edebiliyorsa,
- karar motoruna anlamlı veri sağlıyorsa.

---

# 10. Sonuç

Learning Analytics & Insights, MEF'in öğrenme verilerini anlamlı bilgiye dönüştüren katmanıdır.

Bu bileşen, kullanıcıların daha bilinçli öğrenme kararları almasını ve sistemin zaman içinde gelişmesini destekler.
