---
title: TT426 — Kısa Kesim Sonrası Baskılar
lang: tr
pdf: tt426-short-cut-clamps-tr.pdf
---

# TT426 — Kısa Kesim Sonrası Baskılar

<div class="document-tools" markdown="1">
[English](short_cut_clamps_en.md) · **[PDF indir](downloads/tt426-short-cut-clamps-tr.pdf)**
</div>

Bu rehber, TT426'da **kısa kesim** yapıldıktan sonra baskıların (profil baskı silindirleri) nasıl açıldığını anlatır.

Geçerli sürüm: **PLC V27.1 ve sonrası.**

## Davranış

Kısa kesim modunda yapılan bir kesimden sonra:

| Parça boyu | Kesimden sonra baskılar |
| --- | --- |
| **Short Cut Clamp Length** parametresine eşit ya da daha uzun | **Kapalı kalır.** Ana ekrandaki **Baskıları Aç** tuşuna basılınca açılır. |
| Parametreden kısa | Önceki gibi kendiliğinden açılır. |

- Baskılar açılmadan makine bir sonraki kesime geçmez. Baskılar yukarı konuma gelince döngü devam eder.
- Bu kural, sıradaki parça normal (kısa olmayan) bir kesim olsa da geçerlidir. Karar, **yapılan kesime** göre verilir.
- Acil stopta baskılar her zaman açılır.

## Kullanım

1. Kısa kesim tamamlanır; baskılar parçayı tutmaya devam eder.
2. Parçayı alın ya da kontrol edin.
3. Ana ekranın alt kısmındaki **Baskıları Aç** tuşuna basın.
4. Baskılar açılır, makine sıradaki kesim için devam eder.

## Parametre

| Parametre | Yer | Fabrika değeri |
| --- | --- | --- |
| Short Cut Clamp Length | Servis ekranı → İşleme parametreleri | 431,8 mm (17") |

Değer kaydedilir; makine kapanıp açıldığında korunur.

## Önceki sürümler

PLC V27.1 öncesinde baskıların bekletilmesi **sıradaki parçanın** kesim moduna göre belirleniyordu: kısa kesimden sonra gelen parça normal kesimse baskılar kendiliğinden açılıyordu.
