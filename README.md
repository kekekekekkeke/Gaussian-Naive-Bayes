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
![Screenshot_879](https://github.com/kekekekekkeke/Gaussian-Naive-Bayes/assets/110430637/800b0fd8-0838-4ef2-9f98-ed840c1a7767)

![Screenshot_880](https://github.com/kekekekekkeke/Gaussian-Naive-Bayes/assets/110430637/b776f9c4-a338-4702-9264-157d48878f4d)

![Screenshot_881](https://github.com/kekekekekkeke/Gaussian-Naive-Bayes/assets/110430637/1faf28e0-2c2c-4eaa-95a9-bec49e57aedc)

Varsayılan hiperparametreler ile 0.7727272727272727

Hiperparametreleri optimize edildikten sonra 0.7857142857142857

Normalizasyon uygulandıktan sonra ise  0.7467532467532467 accuracy değerini aldık.

Veri normalleştirildiğinde daha kötü sonuç vermesi, içindeki eksik değerler ve var olan değerlerin de zaten birbirine yakın olmasından kaynaklanabilir.Hiper parametreler optimize edildiğinde ise daha iyi sonuç vermektedir ancak yine de optimize edilmemiş haline oldukça yakındır.Burdan Naive Bayes'in verinin eksik değerlere sahip olması rağmen yeterince iyi sonuç verebildiğini hatta varsayılan hiperparametrelerle bile bu veriseti gibi küçük verisetlerinde iyi sonuçlar verdiğini görüyoruz.Ancak çok fazla özelliğe ya da bibirine aşırı bağlı özelliklerin olduğu setlerde yaptığı birbirinden bağımsız olma varsayımından dolayı aynı kalitede sonuç veremeyecektir.
