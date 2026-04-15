# Skill dosyasının olduğu klasöre gir
cd /skill/dosyasının/olduğu/klasör

# Git başlat
git init

# Dosyaları ekle
git add .

# İlk commit
git commit -m "initial commit: ozgun tez duzeltici skill"

# Sonra senin yazdıkların:
git remote add origin https://github.com/Lancelot3939/ozgun-tez-duzeltici.git
git branch -M main
git push -u origin main

ozgun-tez-duzeltici/
├── README.md                    ← Bu dosya
├── SKILL.md                     ← Skill'in kalbi (Claude'un okuduğu talimatlar)
└── ozgun-tez-duzeltici.skill    ← Paketlenmiş, doğrudan yüklenebilir sürüm

Özgün Tez Düzeltici
Akademik tez, makale ve rapor metinlerini 4 katmanlı bir dönüşüm süreciyle yeniden yazan bir Claude Skill'i. Amaç: AI-üretimi metinlerin tipik imzalarını (cümle uzunluğu monotonluğu, aşırı geçiş ifadeleri, kesin-emin dil, tek-tip kaynak atfı) ortadan kaldırıp metni insan-yazımı doğallığına yaklaştırmak.
Anlam, argüman, kaynak ve jargon dokunulmazdır. Değişen yalnızca yüzey üslubudur.

Ne İşe Yarar?
Bir akademik metni Claude'a verdiğinde skill devreye girer ve metni 4 ardışık katmanda dönüştürür:
KatmanYaptığı1 — Ritim ve YapıCümle uzunluklarını çeşitlendirir (5–8 / 10–12 / 20–30 kelime), ardışık iki cümlenin aynı uzunlukta olmasına izin vermez2 — Geçiş Seyreltme"Bununla birlikte", "öte yandan", "dolayısıyla" gibi geçiş ifadelerinin yarısını siler, kalanları sadeleştirir3 — Hedging ve AtıfKesin yargıları yumuşatır ("göstermektedir" → "işaret edebileceği ileri sürülmektedir"); kaynak atıflarını 3 farklı formatta dağıtır4 — Mikro Doğallaştırma2–3 yere insan-izi ekler: gereksiz "aslında", özne inversiyonu, eliptik kısa cümle, uzun-tireli yan düşünce

Ne Zaman Kullanılır?
Skill şu durumlarda otomatik tetiklenir:

Akademik bir metin paylaşıp "düzenle / doğallaştır / özgünleştir" istediğinde
"AI gibi duruyor", "monoton", "robotik", "hep aynı ritim" şikayetlerinde
Turnitin, GPTZero, AI-detector endişesi dile getirildiğinde
"Benim üslubuma uyarla" talebi geldiğinde

Tetikleyici örnek ifadeler: "tezimi düzenle", "tezimi doğallaştır", "AI gibi durmasın", "katmanlı düzenle", "akademik metin redaksiyonu".

Ne Zaman Kullanılmaz?

Kısa mesaj, e-posta, yaratıcı yazı için (skill akademik kayda özgüdür)
Sadece imla/gramer kontrolü için (bunun için ayrı bir skill kullanılmalı)
Prosedürel içerik, tablo, madde listesi, diyalog, örnek kalıplar — bunlar akademik düzyazı değildir, dokunulmaz


Kurulum
Claude.ai Üzerinde

Bu repodaki ozgun-tez-duzeltici.skill dosyasını indir.
Claude.ai → Settings → Capabilities → Skills
Upload skill ile .skill dosyasını yükle.
Tetikleyici ifadeler geçen bir konuşmada otomatik devreye girer.

Manuel Kurulum
SKILL.md dosyasını kendi kurulumunda kullanmak istiyorsan, dosyayı bir klasöre koyup Claude'un skill yükleme yöntemine göre yerleştirebilirsin.
