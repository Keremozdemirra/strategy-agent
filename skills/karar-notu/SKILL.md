---
name: "karar-notu"
description: "Bir karar için yapılandırılmış karar notu üretir — seçenekler, ödünleşimler, kriterler, tavsiye ve geri dönüş planı. \"Karar vermem lazım\", \"A mı B mi\", \"hangisini seçmeliyim\", \"artı eksi çıkar\", \"karar notu yaz\" dendiğinde kullan."
---

# Karar Notu

Amaç kararı **vermek** değil, doğru kararın kendiliğinden görünür olmasını sağlamak.

## 1. Kararı çerçevele — en önemli adım
- **Asıl soru ne?** Çoğu "A mı B mi" sorusunun altında yanlış çerçevelenmiş bir
  soru vardır. "Hangi CRM'i alalım" aslında "satış sürecimizde ne kırık" olabilir.
- Ne zamana kadar? Ertelemenin maliyeti ne?
- **Geri dönülebilir mi?** Geri dönülebilir kararlar hızlı verilir, uzun analiz
  israftır. Bunu açıkça söyle.
- Kim etkilenir, kim onaylamalı?

Bunlar netleşmeden seçeneklere geçme.

## 2. Kriterleri seçeneklerden ÖNCE belirle
3-5 kriter, ağırlıklı. Seçenekleri gördükten sonra kriter yazmak sonucu kendine
göre uydurmaktır. Sırayı bozma.

## 3. Seçenekleri çıkar
- En az 3. İkisi zaten konuşuluyorsa üçüncüyü sen bul.
- **"Hiçbir şey yapmama" her zaman bir seçenektir** — mutlaka değerlendir.
- Her biri için: ne gerektiriyor (para, zaman, kişi), ne kazandırır, riski ne,
  geri dönüşü ne kadar zor.

## 4. Dürüstçe tart
Her seçeneğin **en güçlü halini** yaz — kolay yenmek için zayıflatma.
Bilmediklerini işaretle. "Kararı tersine döndürecek bilgi ne olurdu?" — onu yaz.

## 5. Yaz

```markdown
# Karar: <tek cümle>
**Durum:** taslak | karar verildi
**Tarih:** | **Karar sahibi:** | **Geri dönülebilir mi:** | **Son tarih:**

## Bağlam  (neden şimdi? 3-5 cümle)

## Kriterler
| # | Kriter | Ağırlık | Neden önemli |

## Seçenekler
### A) <isim>
Ne demek: | Artı: | Eksi: | Maliyet: | Risk:
### B) ...
### C) Hiçbir şey yapmamak

## Karşılaştırma
| Kriter | A | B | C |

## Tavsiye
**<seçenek>** — çünkü <en belirleyici 1-2 gerekçe>.

## Bu tavsiyeyi ne değiştirirdi
## Bilmediklerimiz
## Geri dönüş planı  (yanlış çıkarsa ne yapacağız, hangi işaretle anlayacağız)
## Sonraki adımlar
- [ ] kim / ne / ne zaman
```

Uzunsa dosyaya yaz (`kararlar/YYYY-MM-DD-<konu>.md`), sohbete özet koy.

## Kurallar
- **Tavsiye vermekten kaçınma.** "Duruma göre değişir" işe yaramaz. Tavsiyeni ver,
  gerekçeni göster; kullanıcı reddedebilir.
- Kanıtın taşımadığı kesinlikte cümle kurma.
- Finansal/hukuki kararda: bilgi ver, karar verme, profesyonel danışmanlık
  gerektiğini not düş.
