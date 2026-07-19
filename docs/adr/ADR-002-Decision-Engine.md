# ADR-002 — Central Learning Decision Engine

Durum: Accepted

---

## Bağlam

Karar verme mantığı farklı modüllere dağıtıldığında sistemin davranışını yönetmek zorlaşmaktadır.

---

## Karar

Tüm öğrenme kararları merkezi Learning Decision Engine tarafından üretilecektir.

---

## Gerekçe

- Tek karar noktası
- Açıklanabilir öneriler
- Daha kolay test edilebilirlik
- Gelecekte AI modellerini değiştirebilme

---

## Sonuç

Teaching Strategy, Memory Engine ve Assessment modülleri öneriler üretir.

Nihai karar Learning Decision Engine tarafından verilir.
