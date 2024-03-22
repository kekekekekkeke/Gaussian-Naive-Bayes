# Naive-Bayes
# Giriş

Bu çalışmanın amacı Naive Bayesin teorik alt yapsını anlamak ve bununla ilgili bir uygulama yapmaktır.
# Metot
# Naive Bayes
Naive bayes bir makine öğrenimi ve olasılık teorisi yöntemidir. Temel olarak, bir sınıflandırma algoritmasıdır ve özellikle metin sınıflandırması gibi birçok uygulama alanında kullanılır.
Naive Bayes algoritması, Bayes teoremi üzerine kuruludur. Bayes teoremi, bir olayın meydana gelme olasılığını, bu olayın gerçekleştiği koşullarda belirlemek için kullanılır. Naive Bayes algoritması ise "naif" ya da "saf" olarak adlandırılan bir varsayıma dayanır bu da tüm özelliklerin birbirinden bağımsız olduğunu varsaymasıdır. Bu, özellikler arasında herhangi bir ilişki olmadığı anlamına gelir.
Gaussian naive bayes bunlarlar birlikte özelliklerin normal dağılıma(Gaussian Distiribution) sahip olduğunu varsayar.
# Gridsearch
Grid Search, bir makine öğrenimi modelinin en verimli hiperparametrelerini belirlemek için kullanılan bir yöntemdir. Makine öğrenimi modellerinde, hiperparametreler modelin performansını etkileyen ve kullanıcı tarafından belirlenmesi gereken parametrelerdir.Grid Search yöntemi, önceden belirlenmiş bir hiperparametre uzayını belirler ve bu uzay içinde belirli bir adımla hiperparametreleri dener. Her bir kombinasyon için modeli eğitir ve belirlenen bir performans metriği (doğruluk, hassasiyet, vb.) kullanarak her bir modelin performansını değerlendirir.Sonunda en iyi performansı veren hiperparametre kombinasyonunu seçer.
# Normalizasyon
Bir veri tabanının, veri tekrarını en aza indirgemek ve her tabloda yalnızca ilgili verilerin depolandığından emin olmak için normalleştirilmesi önemlidir. Bir tablo ideal olarak belirli bir konu hakkında olmalı ve sadece destekleyici konular içermelir.
# Sonuçlar ve Yorum
![Screenshot_882](https://github.com/kekekekekkeke/Gaussian-Naive-Bayes/assets/110430637/dbf33938-385f-4ae2-8522-530dd38d967d)
![Screenshot_883](https://github.com/kekekekekkeke/Gaussian-Naive-Bayes/assets/110430637/2ad3bad0-c71e-458c-ae25-c0c525df265e)
![Screenshot_884](https://github.com/kekekekekkeke/Gaussian-Naive-Bayes/assets/110430637/ee654695-f02f-435a-810a-5d323abc90ee)


Varsayılan hiperparametreler ile 0.7337662337662337

Hiperparametreleri optimize edildikten sonra  0.7727272727272727

Normalizasyon uygulandıktan sonra ise 0.7597402597402597 accuracy değerini aldık.

Normalizasyon sonrası da hiperparametre optimizasyonu sonrası da daha iyi sonuç aldığmızı görüyoruz.En iyi sonucu hiperparametreler optimize edildiğinde verdiğini görüyoruz ancak yine de optimize edilmemiş haline oldukça yakındır.Burdan Naive Bayes'in verinin eksik değerlere sahip olması rağmen yeterince iyi sonuç verebildiğini hatta varsayılan hiperparametrelerle bile bu veriseti gibi küçük ve özellikler arası bağlantı çok olmayan verisetlerinde iyi sonuçlar verdiğini görüyoruz.Ancak çok fazla özelliğe ya da bibirine aşırı bağlı özelliklerin olduğu setlerde yaptığı birbirinden bağımsız olma varsayımından dolayı aynı kalitede sonuç veremeyecektir.
