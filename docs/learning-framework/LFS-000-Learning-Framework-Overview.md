# LFS-000 — Learning Framework Overview

| Alan | Değer |
|------|--------|
| Belge Kodu | LFS-000 |
| Belge Adı | Learning Framework Overview |
| Durum | Draft |
| Sürüm | 0.1.0 |
| Son Güncelleme | 2026-07-19 |
| Bağımlılıklar | Foundation, Domain |

---

# 1. Amaç

Learning Framework Specification (LFS), MEF'in çekirdek öğrenme modelini tanımlar.

Bu belge, sistemin kullanıcıya nasıl öğreteceğini, nasıl değerlendireceğini ve öğrenmeyi nasıl kalıcı hâle getireceğini açıklayan en üst düzey teknik referanstır.

Bu belge teknoloji bağımsızdır.

Web, mobil veya gelecekte geliştirilecek farklı platformlar aynı Learning Framework'ü kullanacaktır.

---

# 2. Vizyon

MEF'in amacı bilgi sunmak değildir.

MEF'in amacı, her kullanıcı için kişiselleştirilmiş, ölçülebilir ve sürdürülebilir bir öğrenme süreci oluşturmaktır.

Her kullanıcı farklıdır.

Bu nedenle her öğrenme yolculuğu da farklı olacaktır.

---

# 3. Learning Framework'ün Temel Bileşenleri

Framework aşağıdaki ana bileşenlerden oluşur:

- Learning Goal Management
- Knowledge Graph
- Prerequisite Analysis
- Learning Path Generation
- Adaptive Teaching
- Assessment
- Feedback
- Mastery Evaluation
- Memory Engine
- Reflection
- Learning Analytics

Bu bileşenler birlikte çalışarak tam bir öğrenme döngüsü oluşturur.

---

# 4. Öğrenme Döngüsü

Her öğrenme hedefi aşağıdaki yaşam döngüsünü izler:

```text
Learning Goal
      │
      ▼
Knowledge Analysis
      │
      ▼
Prerequisite Analysis
      │
      ▼
Learning Path Generation
      │
      ▼
Learning Session
      │
      ▼
Assessment
      │
      ▼
Feedback
      │
      ▼
Mastery Evaluation
      │
      ▼
Memory Planning
      │
      ▼
Reflection
      │
      ▼
Continuous Improvement
```

Bu döngü, kullanıcı hedefe ulaşana kadar devam eder.

---

# 5. Temel İlkeler

Framework aşağıdaki ilkelere bağlıdır:

- Öğrenme kişiselleştirilmelidir.
- Öğrenme doğrulanmalıdır.
- Eksikler görünür olmalıdır.
- Hatalar öğrenme fırsatıdır.
- Tekrar öğrenmenin doğal bir parçasıdır.
- Öğrenme sürekli gelişen bir süreçtir.

---

# 6. Öğrenme Başarı Kriterleri

Bir konu yalnızca okunmuş veya izlenmiş olduğu için öğrenilmiş kabul edilmez.

Bir öğrenme hedefi tamamlanmış sayılabilmesi için kullanıcı:

- Kavramı açıklayabilmeli,
- Gerçek bir problem çözebilmeli,
- Bilgiyi farklı senaryolarda kullanabilmeli,
- Gerekirse başkasına öğretebilmelidir.

---

# 7. Framework'ün Kapsamı

Bu belge aşağıdaki alt spesifikasyonların giriş noktasıdır:

- LFS-001 Learning Goal Model
- LFS-002 Knowledge Graph
- LFS-003 Learning Path
- LFS-004 Adaptive Teaching
- LFS-005 Assessment
- LFS-006 Feedback
- LFS-007 Mastery Model
- LFS-008 Memory Engine
- LFS-009 Reflection Model
- LFS-010 Learning Analytics

Her belge, ilgili bileşenin ayrıntılı davranışını tanımlar.

---

# 8. Sonuç

Learning Framework, MEF'in en önemli bileşenidir.

Ürün, kullanıcı arayüzü veya yapay zekâ modelleri zamanla değişebilir.

Ancak Learning Framework, sistemin değişmeyen çekirdeğini oluşturur.

Bu nedenle MEF'in tüm teknik ve ürün kararları bu spesifikasyona uygun olmalıdır.
