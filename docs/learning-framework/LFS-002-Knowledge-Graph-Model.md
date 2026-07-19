# LFS-002 — Knowledge Graph Model

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-002 |
| Belge Adı | Knowledge Graph Model |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | LFS-000, LFS-001, DOMAIN-000 |

---

# 1. Amaç

Knowledge Graph Model, öğrenilecek bilgilerin düğümler (Knowledge Nodes) ve bu düğümler arasındaki ilişkiler olarak modellenmesini tanımlar.

Bu model sayesinde sistem;

- hangi konunun önce öğrenilmesi gerektiğini,
- hangi bilgilerin birbirine bağlı olduğunu,
- kullanıcının hangi noktada eksik olduğunu

hesaplayabilir.

---

# 2. Temel Kavram

Her bilgi bir **Knowledge Node** olarak temsil edilir.

Örnek:

- Değişkenler
- Fonksiyonlar
- Döngüler
- TCP/IP
- SQL JOIN
- Fotosentez

Her düğüm bağımsızdır ancak diğer düğümlerle ilişkilidir.

---

# 3. Knowledge Node Yapısı

Her Knowledge Node aşağıdaki alanlara sahiptir:

- Benzersiz Kimlik (ID)
- Başlık
- Açıklama
- Zorluk Seviyesi
- Tahmini Öğrenme Süresi
- Öğrenme Çıktıları
- Ön Koşullar
- İlişkili Konular
- Örnekler
- Uygulama Görevleri
- Değerlendirme Türleri

---

# 4. İlişki Türleri

Knowledge Node'lar arasında aşağıdaki ilişkiler tanımlanabilir:

## Prerequisite

Bir konunun öğrenilebilmesi için önce öğrenilmesi gereken konu.

Örnek:

```
Fonksiyonlar
    ▲
    │ prerequisite
Değişkenler
```

---

## Builds On

Bir bilgi başka bir bilginin üzerine inşa edilir.

---

## Related To

Konular arasında doğrudan bağımlılık olmasa da anlamlı bir ilişki vardır.

---

## Part Of

Bir konu daha büyük bir konunun parçasıdır.

---

## Reinforces

İki konu birbirini pekiştirir.

---

# 5. Graph Kuralları

- Döngüsel ön koşullar oluşturulamaz.
- Her düğüm en az bir öğrenme çıktısına sahip olmalıdır.
- Her düğüm en az bir Assessment ile doğrulanmalıdır.
- Her düğüm en az bir örnek içermelidir.
- Her düğüm zaman içinde güncellenebilir.

---

# 6. Kullanım Alanları

Knowledge Graph aşağıdaki bileşenler tarafından kullanılır:

- Learning Path Generator
- Prerequisite Analyzer
- Assessment Engine
- Memory Engine
- AI Teacher
- AI Mentor
- Analytics

---

# 7. Eksik Bilgi Analizi

Sistem yeni bir Learning Goal aldığında:

1. İlgili Knowledge Node'ları belirler.
2. Ön koşulları çıkarır.
3. Kullanıcının mevcut bilgisini değerlendirir.
4. Eksik düğümleri işaretler.
5. Kişiselleştirilmiş öğrenme yolu oluşturur.

---

# 8. Örnek

Hedef:

> REST API geliştirmek

Sistem aşağıdaki bilgi ağını oluşturabilir:

```text
HTTP
 │
 ├── Request / Response
 │
 ├── JSON
 │
 ├── REST Prensipleri
 │
 ├── Status Codes
 │
 ├── Authentication
 │
 └── API Design
```

Kullanıcının yalnızca "JSON" konusunda eksik olduğu tespit edilirse, sistem doğrudan bu düğümden başlayabilir.

---

# 9. Gelecek Genişletmeler

İlerleyen sürümlerde Knowledge Graph;

- kullanıcı geri bildirimleri,
- uzman katkıları,
- AI önerileri,
- kullanım verileri

ile sürekli geliştirilebilir.

---

# 10. Sonuç

Knowledge Graph, MEF'in bilgi modelidir.

Learning Path oluşturma, adaptif öğretim ve eksik bilgi analizi bu model üzerine kurulacaktır.

Bu yapı, kullanıcıya her zaman ihtiyacı olan bilgiyi doğru sırada sunmayı hedefler.
