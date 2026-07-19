# LFS-003 — Adaptive Learning Path

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-003 |
| Belge Adı | Adaptive Learning Path |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-000, LFS-001, LFS-002 |

---

# 1. Amaç

Adaptive Learning Path (ALP), her kullanıcı için dinamik olarak oluşturulan ve sürekli güncellenen kişiselleştirilmiş öğrenme yoludur.

MEF'te iki kullanıcı aynı hedefi seçse bile aynı yolu izlemek zorunda değildir.

---

# 2. Temel İlkeler

Learning Path;

- sabit değildir,
- kullanıcı davranışlarına göre değişir,
- başarı ve başarısızlıklardan öğrenir,
- gerektiğinde yeniden oluşturulur.

---

# 3. Learning Path Oluşturma Süreci

Bir kullanıcı yeni bir Learning Goal seçtiğinde sistem aşağıdaki adımları uygular.

### Aşama 1

Hedef Analizi

Örnek:

> "Docker öğrenmek"

---

### Aşama 2

Knowledge Graph Analizi

Hedef için gerekli bütün Knowledge Node'lar çıkarılır.

---

### Aşama 3

Ön Bilgi Analizi

Sistem kullanıcının mevcut bilgisini belirler.

Kaynaklar:

- Ön değerlendirme
- Geçmiş başarılar
- Tamamlanan görevler
- Kullanıcının beyanı

---

### Aşama 4

Eksik Bilgi Analizi

Eksik düğümler belirlenir.

Bu düğümler öncelik sırasına konur.

---

### Aşama 5

İlk Learning Path Oluşturulur.

---

# 4. Adaptasyon Mekanizması

Learning Path aşağıdaki durumlarda yeniden hesaplanabilir.

- Assessment başarısız oldu.
- Kullanıcı zorlandığını belirtti.
- Öğrenme hızı beklenenden düşük.
- Kullanıcı çok hızlı ilerledi.
- Yeni Learning Goal eklendi.
- Ön koşul eksik bulundu.

---

# 5. Öğretim Stratejileri

Bir konu tek yöntemle öğretilmez.

MEF gerektiğinde farklı stratejilere geçebilir.

Örneğin:

### Strateji 1

Klasik açıklama

---

### Strateji 2

Benzetmeler

---

### Strateji 3

Günlük yaşam örnekleri

---

### Strateji 4

Görsel anlatım

---

### Strateji 5

Adım adım uygulama

---

### Strateji 6

Sokratik yöntem

Kullanıcıya sorular sorarak sonuca ulaştırma.

---

### Strateji 7

Mini proje

---

### Strateji 8

Oyunlaştırılmış görev

---

# 6. Zorlanma Tespiti

Sistem aşağıdaki durumlarda kullanıcının zorlandığını varsayabilir.

- Aynı konuda art arda başarısız Assessment
- Uzun cevap süreleri
- Sürekli ipucu isteme
- Aynı içeriği tekrar açma
- Kullanıcının "Anlamadım." demesi

---

# 7. Adaptasyon Kararları

Sistem aşağıdaki kararları alabilir.

- Daha kolay örnekler sun.
- Konuyu farklı yöntemle anlat.
- Ön koşulları tekrar et.
- Daha fazla uygulama ekle.
- Öğrenme hızını düşür.
- Yeni değerlendirme oluştur.

---

# 8. Kullanıcı Kontrolü

Kullanıcı her zaman aşağıdaki haklara sahiptir.

- Learning Path'i görüntülemek
- Önerilen sırayı kabul etmek
- Alternatif yol istemek
- Konuyu tekrar etmek
- Öğrenme hızını değiştirmek

MEF öneri sunar; son karar kullanıcıya aittir.

---

# 9. Başarı Ölçütü

Adaptive Learning Path başarılı sayılırsa:

- Kullanıcı daha az tekrar ile öğrenir.
- Daha yüksek Mastery seviyesine ulaşır.
- Bilgiyi daha uzun süre hatırlar.
- Öğrenme motivasyonunu korur.

---

# 10. Sonuç

Adaptive Learning Path, MEF'in kişiselleştirme mekanizmasının merkezidir.

Knowledge Graph, Assessment, Memory Engine ve AI Teacher birlikte çalışarak her kullanıcı için sürekli gelişen bir öğrenme yolu oluşturur.
