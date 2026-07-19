# LFS-001 — Adaptive Mastery Learning Model (AMLM)

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-001 |
| Belge Adı | Adaptive Mastery Learning Model |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-000, DOMAIN-000 |

---

# 1. Amaç

Adaptive Mastery Learning Model (AMLM), MEF'in temel öğrenme modelidir.

Modelin amacı, her kullanıcının aynı hedefe kendi hızında, kendi öğrenme biçimine uygun ve doğrulanabilir şekilde ulaşmasını sağlamaktır.

---

# 2. Temel Varsayımlar

AMLM aşağıdaki varsayımlara dayanır:

- Her bireyin öğrenme hızı farklıdır.
- Anlamak ile ezberlemek aynı değildir.
- Öğrenme doğrulanabilir olmalıdır.
- Tekrar, öğrenmenin ayrılmaz bir parçasıdır.
- Hata yapmak öğrenme sürecinin doğal bir bileşenidir.
- Öğrenme doğrusal değil, döngüsel bir süreçtir.

---

# 3. AMLM Döngüsü

Her konu aşağıdaki döngü ile işlenir:

```text
1. Hedef Belirleme
        │
2. Ön Bilgi Analizi
        │
3. İçerik Sunumu
        │
4. Aktif Uygulama
        │
5. Değerlendirme
        │
6. Geri Bildirim
        │
7. Eksik Analizi
        │
8. Adaptasyon
        │
9. Tekrar Planı
        │
10. Yansıtma (Reflection)
        │
        └────────► Gerekirse döngü yeniden başlar
```

---

# 4. Adaptasyon İlkesi

Sistem her kullanıcı için aşağıdaki unsurları uyarlayabilir:

- Anlatım biçimi
- Örnek sayısı
- Zorluk seviyesi
- Öğrenme sırası
- Tekrar aralığı
- Görev türü

Amaç, tek tip eğitim yerine kişiye uygun öğrenme deneyimi sunmaktır.

---

# 5. Ustalık (Mastery)

Bir konu yalnızca tamamlanmış olduğu için öğrenilmiş sayılmaz.

Ustalık için kullanıcı;

- Kavramı açıklayabilmeli,
- Bilgiyi uygulayabilmeli,
- Yeni bir probleme aktarabilmeli,
- Hatalarını düzeltebilmeli,
- Bilgiyi belirli bir süre sonra tekrar gösterebilmelidir.

---

# 6. Başarısızlık Yaklaşımı

Başarısızlık bir son değildir.

Sistem başarısızlık durumunda:

1. Eksik kavramları belirler.
2. Ön koşulları yeniden değerlendirir.
3. Alternatif anlatım yöntemi seçer.
4. Yeni uygulama görevi oluşturur.
5. Gerekirse öğrenme yolunu yeniden düzenler.

---

# 7. Öğrenme Kanıtları

Bir kullanıcının ilerlemesi aşağıdaki kanıtlarla desteklenir:

- Tamamlanan görevler
- Değerlendirme sonuçları
- Proje çalışmaları
- Kod örnekleri
- Açık uçlu cevaplar
- Tekrar performansı
- Uzun dönem hatırlama başarısı

---

# 8. Başarı Ölçütü

MEF için başarı;

- kaç video izlendiği,
- kaç sayfa okunduğu,
- kaç dakika sistemde kalındığı

değil,

kullanıcının hedeflediği bilgi ve beceriyi gerçekten kazanmasıdır.

---

# 9. Sonuç

Adaptive Mastery Learning Model, MEF'in bütün öğrenme kararlarının temelini oluşturur.

Learning Path, Assessment, Memory Engine ve AI destekli öğretim stratejileri bu modele uygun çalışmalıdır.
