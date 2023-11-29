# Spring-MongoDb
I explain to connection Spring with MongoDb

<span style="color:blue; font-size:18px;">Gerekli olan Dependencyler</span>
<span style="color:blue; font-size:18px;">Lombok : Getter ve setter metotlarını ayrı ayrı yazmaya gerek bırakmadan , anatosyonlar </span>yardımıyla oluşturmamıza olanak sağlar.    </span>
																																													</span>
<span style="color:blue; font-size:18px;">Spring Data MongoDB : Veritabanı işlemlerimiz için gerekli implementleri sağlayacak.                                                      </span>
																																													</span>
<span style="color:blue; font-size:18px;">Spring Boot DevTools : Ben uygulama da değişikliklerden sonra otomatik deploy etme özelliğini kullanıyorum . Bunun haricin de işlevsel    </span>birçok özelliği bulunmakta.
																																													</span>
																																													</span>
<span style="color:blue; font-size:18px;">Projenin ilk ayağında sadece veri ekleyip gösterme yapacağımız için bu paketler işimizi görecektir. API paketinde http isteklerinin       </span>karşılandığı controller ımız , DAL paketindeki bu isteklerin yönlendirildiği sınıflar , Repositories paketi altında veriye temas ettiğimiz repository ler bulunacak .
																																													</span>
<span style="color:blue; font-size:18px;">Biz proje de mongo database ini kullanacağımız için ,veri tabanı işlemleri için Mongo Repository extend ini yaptığımız repository mizi    </span>kullanıyor olacağız.
																																													</span>
<span style="color:blue; font-size:18px;">RDBMS(ilişkisel veri tabanları) sistemlerde kullandığımız tablolar , nosql veri tabanlarında collection olarak saklanır. Collectionlar da </span>veriler (key/value) olarak tutulur. Veriler aralarında ilişki olmadığından oldukça hızlıdır. Document ler ise satırlarımızı temsil eder.
																																													</span>
<span style="color:blue; font-size:18px;">BookRepository MongoRepository interface ini extend ediyor . MongoRepository extendi sayesinde CRUD operasyonlarının yanında bir çok veri tabanı operasyonunu kullanabiliriz.</span>
																																													</span>
<span style="color:blue; font-size:18px;">HTTP isteklerinin cevaplanacağı controller ı da ekledikten sonra kullanacağımız veri tabanı bağlantımız kalıyor.                          </span>
																																																																																							
<span style="color:blue; font-size:18px;">spring.data.mongodb.host=localhost                                                                                                        </span>
<span style="color:blue; font-size:18px;">spring.data.mongodb.port=27017                                                                                                            </span>
<span style="color:blue; font-size:18px;">spring.data.mongodb.database=BookStore                                                                                                    </span>
																																													</span>
<span style="color:blue; font-size:18px;">Mongo Db kullanabilmek için Mongo Db Server , verileri görebilmek için grafiksel arayüz sağlayan Mongo Compass uygulamasını kurmamız gerekiyor.     </span>
