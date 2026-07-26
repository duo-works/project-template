# <PROJE ADI>

> <Bir cümlelik proje açıklaması.>

> ### 🤖 AI ajanıysan buradan başla
>
> **Bu repoda herhangi bir iş yapmadan önce [`AGENTS.md`](AGENTS.md) dosyasını oku — zorunludur.**
>
> İçinde: oturum protokolü (çakışma kontrolü, devir kayıtları), kesin kurallar, hazır komutlar ve Notion referansları. Projeyi tanımak için oradaki **"İlk kez buradaysan — okuma sırası"** bölümünü izle; repo ve Notion'u birlikte kapsıyor.
>
> Bu org'da iki geliştirici **dört ayrı ajanla** çalışıyor. Protokolü atlarsan başkasının açık işinin üzerine yazabilirsin.

<!--
  YENİ PROJE KURUYORSANIZ — doldurulacaklar:
    1. Yukarıdaki başlık ve tek cümlelik açıklama
    2. "Bu proje şu an nerede" bölümü
    3. Aşağıdaki tabloda <PRD LİNKİ> — Notion → 📚 Bilgi Bankası'nda proje PRD'sini açıp linkini koyun
    4. Kurulum bölümündeki <PROJE> adı

  Diğer Notion linkleri org geneli, her projede aynı — dokunmayın.
-->

---

## Bu proje şu an nerede

<!--
  Kısa tutun. Durum bilgisi burada tutulursa eskir; canlı durum Notion → 📋 Görevler'de.
  Buraya yalnızca yavaş değişen gerçekler yazın: kod var mı, yığın seçildi mi, ne bloke ediyor.
-->

- **Kapsam** — <PRD durumu>
- **Teknoloji yığını** — <seçildi mi?>

Canlı durum için **[📋 Görevler](https://app.notion.com/p/93190546ef3941c88ab1d2bd0d1fface)**'e bakın.

---

## Bu repo nasıl çalışır

| İhtiyacınız | Nereye bakacaksınız |
|---|---|
| Ne yapacağım? Görev listesi? | **[📋 Görevler](https://app.notion.com/p/93190546ef3941c88ab1d2bd0d1fface)** — bu repo'da Issues kapalıdır |
| Nasıl çalışıyoruz? Branch, commit, PR kuralları | [`CONTRIBUTING.md`](CONTRIBUTING.md) |
| Neden böyle yapılmış? Mimari kararlar | [`docs/decisions/`](docs/decisions/) · **[🧭 Kararlar](https://app.notion.com/p/79735f2d234744bca1c73ebc62d20788)** |
| Proje ne yapacak? Kapsam ne? | **<PRD LİNKİ>** |
| PRD, mimari doküman, API notları | **[📚 Bilgi Bankası](https://app.notion.com/p/6c92e82ed17c427ba0d515c827fac07e)** |
| AI ajanı ile çalışırken konvansiyonlar | [`AGENTS.md`](AGENTS.md) — Claude Code ve Codex için tek kaynak |
| Kim şu an neye dokunuyor? Devir notları | **[📓 Oturum Kaydı](https://app.notion.com/p/cb1df32162934baba379c8733813893f)** |

🔗 **Notion çalışma alanı:** [🛠️ duo-works](https://app.notion.com/p/3a79bfc93b2e81048f7ddf02d3de4a38)

---

## Yeni katılıyorsanız

1. **[🚪 Onboarding](https://app.notion.com/p/3a79bfc93b2e81b589e6fe2918e64a00)** — 30 dakikada devreye girme rehberi
2. **[🤖 Ajan Kurulumu](https://app.notion.com/p/3a89bfc93b2e8125b9d5e6a99682d706)** — Claude Code ve Codex'i koordinasyon sistemine bağlama

İkinci adımı atlamayın. Ajanınız Notion'a yazamıyorsa karşı tarafın ajanı "aktif kayıt yok" görüp aynı dosyaya girer.

---

## Kurulum

```bash
gh repo clone duo-works/<PROJE>
cd <PROJE>
cp .env.example .env    # gerçek değerleri parola yöneticisinden alın
```

<!-- Stack seçildikten sonra buraya bağımlılık kurulum ve çalıştırma adımları eklenir. -->

---

## Katkı

Kod yazmaya başlamadan önce [`CONTRIBUTING.md`](CONTRIBUTING.md) dosyasını okuyun. Özet:

1. Notion'da görevi **Yapılıyor**'a alın
2. `main`'den branch açın: `feat/DW-42-kisa-aciklama`
3. PR başlığı: `feat(kapsam): açıklama [DW-42]`
4. Onay + yeşil CI → squash merge
5. Notion'da görevi **Bitti**'ye alın

`main`'e doğrudan push kapalıdır. Branch adı, commit mesajı ve PR gövdesi CI tarafından doğrulanır.
