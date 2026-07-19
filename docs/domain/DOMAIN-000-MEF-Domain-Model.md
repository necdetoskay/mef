# DOMAIN-000 — MEF Domain Model

| Alan | Değer |
|------|--------|
| Belge Kodu | DOMAIN-000 |
| Belge Adı | MEF Domain Model |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Sahibi | Product & Architecture Team |

---

# 1. Amaç

Bu belge, MEF'in iş alanını (Domain) tanımlar.

Amaç; ürünün temel kavramlarını, bu kavramlar arasındaki ilişkileri ve sınırları belirlemektir.

Bu belge teknik mimari, veritabanı tasarımı veya API sözleşmesi değildir. Bunlar daha sonra bu modele dayanarak oluşturulacaktır.

---

# 2. Temel İlke

MEF'in merkezinde **öğrenme** vardır.

Yapay zekâ, kullanıcı arayüzü, veritabanı veya teknoloji seçimi bu amaca hizmet eden araçlardır.

Temel soru şudur:

> "Bir insanın gerçekten öğrendiğini nasıl anlayabilir ve bu süreci nasıl iyileştirebiliriz?"

---

# 3. Ana Domain Varlıkları

## Learner (Öğrenen)

Platformu kullanan kişidir.

Sahip olduğu bilgiler:

- Profil
- Hedefler
- Bilgi seviyesi
- Öğrenme geçmişi
- Tercihler
- İlerleme durumu

---

## Learning Goal

Kullanıcının ulaşmak istediği sonuçtur.

Örnekler:

- Docker öğrenmek
- İngilizce konuşabilmek
- Ağ yönetimini kavramak
- Yapay zekâ geliştirmek

Bir kullanıcının aynı anda birden fazla öğrenme hedefi olabilir.

---

## Knowledge

Öğrenilecek bilgi veya kavramdır.

Her bilgi;

- ön koşullara,
- ilişkili kavramlara,
- zorluk seviyesine,
- öğrenme çıktısına

sahiptir.

---

## Skill

Bilginin uygulanabilir hâlidir.

Bilmek ile yapabilmek aynı şey değildir.

MEF, bilgiyi beceriye dönüştürmeyi hedefler.

---

## Assessment

Öğrenmeyi doğrulayan değerlendirmedir.

Türleri:

- Quiz
- Açık uçlu soru
- Uygulamalı görev
- Kod yazma
- Senaryo çözümü
- Proje

---

## Mastery

Belirli bir konuda yeterlilik seviyesidir.

Önerilen seviyeler:

- Beginner
- Basic
- Intermediate
- Advanced
- Expert
- Mentor

---

## Memory

Öğrenilen bilgilerin zaman içindeki kalıcılığını temsil eder.

Bellek modeli;

- tekrar planı,
- unutma riski,
- tekrar geçmişi,
- güçlenme seviyesi

gibi verileri içerir.

---

## Feedback

Sistemin kullanıcıya sunduğu geri bildirimdir.

Geri bildirim yalnızca doğru/yanlış bilgisi değildir.

Aynı zamanda:

- neden,
- nasıl,
- hangi konuda eksik,
- nasıl gelişebilir

sorularını da cevaplar.

---

# 4. Domain İlişkileri

```text
Learner
   │
   ├── owns ─────────► Learning Goal
   │
   ├── learns ───────► Knowledge
   │                     │
   │                     └── develops ─► Skill
   │
   ├── completes ────► Assessment
   │
   ├── reaches ──────► Mastery
   │
   ├── stores ───────► Memory
   │
   └── receives ─────► Feedback
```

---

# 5. Domain Kuralları

1. Her Learning Goal en az bir Knowledge alanına bağlıdır.
2. Her Knowledge öğesinin sıfır veya daha fazla ön koşulu olabilir.
3. Assessment olmadan Mastery oluşmaz.
4. Mastery zaman içinde güncellenebilir.
5. Memory, tekrarlarla güçlenir; kullanılmadığında zayıflayabilir.
6. Feedback her Assessment sonrasında üretilmelidir.

---

# 6. Domain Dışı Unsurlar

Aşağıdakiler Domain'in parçası değildir:

- Web arayüzü
- Mobil uygulama
- Yapay zekâ sağlayıcıları
- Veritabanı teknolojisi
- API yapısı
- Kimlik doğrulama sistemi
- Bildirim altyapısı

Bunlar uygulama katmanında ele alınacaktır.

---

# 7. Açık Sorular

Bu belge ilerleyen sürümlerde aşağıdaki konularla genişletilecektir:

- Knowledge Graph modeli
- Learning Path yapısı
- Öğrenme oturumları (Learning Session)
- Görev sistemi (Mission)
- Motivasyon modeli
- Rozet ve başarı sistemi
- Sosyal öğrenme
- Grup öğrenme
- AI Agent rolleri

---

# 8. Sonuç

Bu belge, MEF'in ortak dilini tanımlar.

Bundan sonra oluşturulacak tüm PRD, mimari, veri modeli ve kod çalışmaları bu ortak dili kullanmalıdır.

Domain modeli değişirse, ilgili tüm belgeler gözden geçirilmelidir.
