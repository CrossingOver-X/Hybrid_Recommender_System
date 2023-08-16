# Hybrid Recommender System
Bu proje, öneri sistemleri alanında kullanılan iki farklı yöntem olan "User-Based Collaborative Filtering" ve "Item-Based Collaborative Filtering" yöntemlerini kullanarak bir hibrid öneri sistemi geliştirmeyi amaçlamaktadır. Bu hibrid sistem, kullanıcının daha iyi ve kişiselleştirilmiş öneriler almasını sağlamak için iki farklı yöntemin avantajlarını birleştirir.

# Verinin Hazırlanması
Bu adımda, "movie" ve "rating" veri setleri kullanılarak bir kullanıcı-film matrisi oluşturulmaktadır. Bu matris, her bir kullanıcının hangi filmlere hangi puanları verdiğini içermektedir. Eksik veya nadiren puanlanan filmler çıkartılmaktadır.

# Öneri Yapılacak Kullanıcının İzlediği Filmlerin Belirlenmesi

Öneri yapılacak olan kullanıcı rastgele bir şekilde seçilir. Seçilen kullanıcının izlediği filmler belirlenir ve bu filmler üzerinden benzer kullanıcılar tespit edilir.

# Aynı Filmleri İzleyen Diğer Kullanıcıların Verisine ve Id'lerine Erişmek

Seçilen kullanıcının izlediği filmler, diğer kullanıcıların izlediği filmler ile korelasyonları kullanılarak benzer kullanıcılar belirlenir. Bu benzer kullanıcıların id'leri ve izledikleri filmler elde edilir.

# Öneri Yapılacak Kullanıcı ile En Benzer Kullanıcıların Belirlenmesi

Seçilen kullanıcı ile yüksek korelasyona sahip kullanıcılar belirlenir ve bu kullanıcılar arasından en benzer olanlar seçilir. Bu kullanıcılar öneri yapılacak kullanıcının ilgilenebileceği filmleri belirlemek için kullanılır.

# Weighted Average Recommendation Score'un Hesaplanması ve İlk 5 Filmin Tutulması

Benzer kullanıcıların puanlarını kullanarak, kullanıcıların verdiği puanlarla ağırlıklandırılmış bir ortalama skor hesaplanır. Bu skorlar, filmlerin öneri skorlarını oluşturmak için kullanılır ve en iyi 5 film önerisi elde edilir.

# Item-Based Recommendation

Kullanıcının en son izlediği ve en yüksek puan verdiği film temel alınarak, "Item-Based Collaborative Filtering" yöntemi kullanılarak öneri yapılır. Kullanıcının izlediği film ile diğer filmlerin korelasyonları hesaplanarak, en benzer filmler belirlenir ve öneri yapılır.

# Sonuçlar

Bu proje, farklı öneri sistemleri yöntemlerinin birleştirilerek daha iyi ve kişiselleştirilmiş öneriler sunan bir hibrid öneri sistemi oluşturmayı amaçlamaktadır. Adım adım kodlarla sunulan bu proje, öneri sistemlerinin temel mantığını ve yöntemlerini anlamak isteyenler için faydalı bir kaynak olabilir.

Bu projenin detaylı kodları ve açıklamaları "HYBRID_RECOMMENDER_PROJE.py" dosyasında bulunmaktadır. Projeyi daha iyi anlamak için bu kodları inceleyebilirsiniz.
