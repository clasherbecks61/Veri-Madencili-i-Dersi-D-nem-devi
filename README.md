# Veri-Madenciligi-Dersi-Donem-Odevi

Verilerimizin ilk ve ham hali
![Ham Veri Tablosu](images/ekran1.png)

Sözleşme tipine göre müşteri kaybının grafik ile gösterimi


Grafiği incelendiğimizde en yüksek müşteri kaybının 'Month-to-month'sözleşme tipine sahip müşterilerde yaşandığı görülmektedir. Uzun vadeli sözleşmeler müşteri sadakatini artırarak ayrılma oranını istatistiksel olarak belirgin bir şekilde düşürmüştür. 
![Bkz. Month-to Month sözleşme tipi ile Uzun Vadeli sözleşmelerin karşılaştırıldığı bir grafik örneği](images/ekran2.png)


Müşteri sadakati ile aylık ödeme ilişkisi


Bu serpilme (dağılım) grafiği, müşterinin şirkette geçirdiği süre, ödediği aylık fatura ve ayrılma durumu arasındaki üçlü ilişkiyi aynı anda incelememizi sağlıyor.
![Bkz. Bu serpilme grafiği, müşterinin şirkette geçirdiği süre, ödediği aylık fatura ve ayrılma durumu arasındaki üçlü ilişkiyi aynı anda incelememizi sağlıyor ](images/ekran3.png)


NaN değerlerin (Boş veya eksik olan veriler) doldurulması ve modelleme için anlamsız olan `customerID` sütununun çıkartılmasından sonraki verinin son hali:
![Final Veri Tablosu](images/ekran4.png)

Bu iki analizimiz, şirketin en büyük yarasının "yüksek fatura ödeyen, taahhütsüz (aylık) yeni müşteriler" olduğunu açıkça ortaya koymaktadır.


Ödevin 2.ci Kısmı
1. Tamamlanmış Orange Proje Dosyası
donemodevi2.ows dosyası projeye eklendi.

2.Model Karşılaştırma Tablosu

![Bkz.Modellerin hızlarının karşılaştırıldığı oran tablosu](images/ekran5.png)


3. Hata analiz tablosu

Bu sonuçlara göre; gerçekte şirkette kalmasına rağmen model tarafından yanlışlıkla
"ayrılacak" olarak tahmin edilen (False Positive) müşteri sayısı 150'dir.

![Bkz.Seçilen en başarılı modelin Karmaşıklık Matrisi sonucu](images/ekran6.png)

4. Şirket için en riskli müşteri profili
   
Karar Ağacı algoritmasının oluşturduğu dallanmalar incelendiğinde, şirket için en yüksek ayrılma riskine sahip müşteri profili şunlardır:
Aylık sözleşmesi (Month-to-month) bulunan, Fiber optik internet servisi kullanan ve şirketteki kalma süresi henüz çok düşük olan yeni müşterilerdir.
