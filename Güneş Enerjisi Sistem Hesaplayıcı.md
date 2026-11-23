# ☀️ Güneş Enerjisi Sistem Hesaplayıcı

Konuma göre güneşlenme, elektrik üretimi, maliyet (TL/m²) ve geri dönüş süresi. Ev tipi, bataryalı ve EV şarj istasyonlu sistemler.

## Girdiler

Sistem tipi Şehir

Enlem (°) Güneşlenme (kWh/m²/gün)

Çatı alanı (m²) Panel verimi (%)

Eğim (°) Yön

Performans oranı (PR) Aylık tüketim (kWh)

Batarya kapasitesi (kWh) [ ] EV şarj istasyonu ekle

Günlük yol (km) Tüketim (kWh/100 km)

Şarj zamanı

Birim fiyatlar ve varsayımlar (düzenlenebilir)

Panel (TL/Wp) İnvertör (TL/Wp)

Montaj + işçilik (TL/Wp) Batarya (TL/kWh)

EV şarj cihazı (TL) Diğer giderler (%)

Elektrik tarifesi (TL/kWh) Şebekeye satış (TL/kWh)

Yıllık panel kaybı (%) Yıllık tarife artışı (%)

Gelişmiş parametreler (sıcaklık, DC kablo, EV)

Ort. sıcaklık (°C)Sıcaklık katsayısı (%/°C)

[ ] PR’yi sıcaklığa göre aylık ayarla

Panel Voc (V)Panel Vmp (V)

Panel Imp (A)Seri panel sayısı

DC kablo uzunluğu (m, tek yön)Kablo kesiti (mm²)

EV şarj gücü (kW)Benzinli araç (L/100 km)

Benzin fiyatı (TL/L, örnek)

## Sonuçlar

## Aylık üretim ve tüketim (kWh)

ÜretimTüketim

## Maliyet dağılımı

## Yöntem ve notlar

Kurulu güç = alan × panel verimi (1 kW/m² STC). Yıllık üretim = kWp × günlük güneşlenme × eğim/yön katsayısı × PR × 365. Aylık dağılım enleme bağlı mevsimsel bir eğriyle yaklaşık olarak hesaplanır. Öz tüketim; gündüz yükü %35, gece yükü %65 ve batarya gidiş-dönüş verimi %90 varsayılarak bulunur.

Şehir güneşlenme değerleri yaklaşık yıllık ortalamalardır; tezde GEPA veya PVGIS verisiyle değiştirin. Fiyatlar örnek varsayımdır, güncel piyasa fiyatıyla güncelleyin. Batarya/invertör değişimi ve bakım hesaba katılmamıştır. LCOE = toplam maliyet / 25 yıllık toplam üretim; IRR 25 yıllık tasarruf akışından hesaplanır; AC akım 8 kW’a kadar tek faz (230 V), üstü üç faz (400 V) varsayılır. Sıcaklık kaybında hücre sıcaklığı ≈ ortam + 25 °C alınır, ortam sıcaklığı sinüs eğrisiyle modellenir. Saatlik simülasyon çan şeklinde üretim eğrisi ve tipik ev yük profili kullanır. DC kablo hesabı bakır iletken için ρ = 0,0225 Ω·mm²/m ile yapılır; EV sonuçları yaklaşıktır.

## Saatlik simülasyon (tipik gün)

Ay

ÜretimTüketimBatarya doluluğuŞebekeden çekilen

## Hassasiyet analizi (geri dönüş, yıl)

## Senaryo karşılaştırma