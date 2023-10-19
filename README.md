# NBA-Forecasting-Machine-Learning

Bu projemde, NBA takımlarının gelecekteki maçlarında toplam kaç sayı atılacağını tahmin etmek amacıyla bir veri analizi yaklaşımı kullanıyorum. Projem, veri çekme, veri işleme ve makine öğrenimi analizlerini içeriyor.

### Veri Çekme:
NBA takımlarının gelecekteki ve geçmişteki maç verilerini elde etmek için, <a href= "basketball-reference.com">  "Basketball Reference" </a> adlı web sitesinden veri çekme işlemi gerçekleştiriyorum. Bu veriler, her iki takımın gelecekteki maç tarihleri ve takımların geçmiş maçlarının sonuçları gibi bilgileri içermektedir.

### Veri İşleme:
Elde edilen verileri işlemek için Python dilinde popüler veri işleme kütüphaneleri olan <a href="https://numpy.org">NumPy</a> ve <a href="https://pandas.pydata.org">Pandas</a>' kütüphanelerini kullanıyorum. Verileri düzenliyorum ve özellik mühendisliği yapıyorum. Özellikle, her iki takımın geçmiş maçlarına dayalı istatistikleri çıkararak tahmin modeli için girdi verilerini oluşturuyorum.

### Makine Öğrenimi Analizi:
Tahmin yapmak için makine öğrenimi tekniklerini kullanıyorum. <a href="https://scikit-learn.org">Sklearn</a> kütüphanesinde bulunan <a href="https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html">LinearRegression</a> algoritması ile verileri analiz ediyorum. Bu algoritma, iki takım arasındaki geçmiş maçlara dayalı istatistikleri kullanarak gelecekteki maçlarda toplam kaç sayı atılacağını tahmin etmek için kullanıyorum.

### Proje Adımları:
1) İlk olarak, mevcut tarih, ay ve saati datetime modülü kullanılarak alınır.

2) Ardından, NBA takımlarının istatistiklerini ve oynadıkları maçları içeren bir web sitesinden veri çekmek için requests_html ve HTMLSession kullanılır.

3) Veriler çekildikten sonra, her bir takım için istatistikler ayrı ayrı çekilir ve uygun listelere eklenir.

4) Gelecekteki maçların programını içeren bir web sayfası da çekilir ve maçların tarihleri, saatleri, ev sahibi ve deplasman takımları gibi bilgiler alınır.

5) Daha sonra, geçmiş maçlara dayalı olarak bir tahmin modeli oluşturmak için istatistikler ve maç sonuçları bir araya getirilir. Bu model, sklearn kütüphanesinde bulunan LinearRegression ile eğitilir.

6) Gelecekteki maçların tahminleri yapılır ve sonuçlar predicted_matches adlı bir liste içinde saklanır.

7) Tahmin modeli bir .sav dosyasına kaydedilir, böylece gelecekte kullanılabilir.

8) Son olarak, tahmin sonuçları ve modelin katsayıları ve intercept değeri ekrana yazdırılır.

![Ekran görüntüsü 2023-10-18 012940](https://github.com/KaganMuslu/NBA-Forecasting-Machine-Learning/assets/71410113/4195245c-4a3e-48de-8e64-286e3c8f7525)

