# Spring-MongoDb
I explain to connection Spring with MongoDb

Gerekli olan Dependencyler</span>
Lombok : Getter ve setter metotlarını ayrı ayrı yazmaya gerek bırakmadan , anatosyonlar </span>yardımıyla oluşturmamıza olanak sağlar. Detaylı bilgi için bkz.

Spring Data MongoDB : Veritabanı işlemlerimiz için gerekli implementleri sağlayacak.

Spring Boot DevTools : Ben uygulama da değişikliklerden sonra otomatik deploy etme özelliğini kullanıyorum . Bunun haricin de işlevsel bir çok özelliği bulunmakta.


Projenin ilk ayağında sadece veri ekleyip gösterme yapacağımız için bu paketler işimizi görecektir. API paketinde http isteklerinin karşılandığı controller ımız , DAL paketindeki bu isteklerin yönlendirildiği sınıflar , Repositories paketi altında veriye temas ettiğimiz repository ler bulunacak .

Biz proje de mongo database ini kullanacağımız için ,veri tabanı işlemleri için Mongo Repository extend ini yaptığımız repository mizi kullanıyor olacağız.

RDBMS(ilişkisel veri tabanları) sistemlerde kullandığımız tablolar , nosql veri tabanlarında collection olarak saklanır. Collectionlar da veriler (key/value) olarak tutulur. Veriler aralarında ilişki olmadığından oldukça hızlıdır. Document ler ise satırlarımızı temsil eder.

BookRepository MongoRepository interface ini extend ediyor . MongoRepository extendi sayesinde CRUD operasyonlarının yanında bir çok veri tabanı operasyonunu kullanabiliriz.

HTTP isteklerinin cevaplanacağı controller ı da ekledikten sonra kullanacağımız veri tabanı bağlantımız kalıyor.


spring.data.mongodb.host=localhost
spring.data.mongodb.port=27017
spring.data.mongodb.database=BookStore

Mongo Db kullanabilmek için Mongo Db Server , verileri görebilmek için grafiksel arayüz sağlayan Mongo Compass uygulamasını kurmamız gerekiyor.
