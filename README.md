
<h1>Postman</h1>
<br><br>
<h2>Postman Nedir?</h2>
--------------
<ul>
<li>Postman, Chrome uzantısı olarak kullanabileceğimiz veya direct indirip bilgisayarımıza yükleyebileceğimiz bir uygulamadır. Rest Client olarak da tanımlanabilir.</li>
<li>API(Application Programming Interface) farklı uygulama yazılımlarının birbirleri ile etkileşim sağlamasına olanak sağlar. Client(Android) ve Backend(java) yazılımlarının Restfull Api ile iletişim kurması buna örnek verilebilir.</li>
<li>Postman sayesinde uzun uzun kodlar yazmak yerine API’lerimizi kolayca test edebiliriz. Birçok özelliği sayesinde kolay bir şekilde istek hazırlayıp gelen cevap değerlerini kullanabiliriz</li>
</ul>
<br><br><br>
<h3>POST-GET-PUT-DELETE</h3>
 <br>
<p>İstek metod türlerimiz bulunmaktadır, en çok kullanılanları ise GET, POST, PUT, DELETE metodlarıdır.
<br> Not: CRUD operasyonları Create, Read, Update, Delete olarak adlandırılmaktadır.</p>

<ol>
<li><strong><em>GET:</em></strong> Sunucudan sadece veri çekmek(okuma) istiyorsak yani veri üzerinde herhangi bir değişiklik(ekleme, slime, modifiye) yapılmayacaksa GET metodunu kullanmamız tavsiye ediliyor.
<br><br>
CRUD operasyonlarından Read’e karşılık geldiğini söyleyebiliriz.
<br><br>
Ör: GET /students kullandığımızda bize öğrenciler listesini dönmesi.</li>
<br><br><br>
<li><strong><em>POST:</em></strong> Server Api’e body kısmını doldurarak ve veri üzerinde değişiklik yapmak istediğimizde kullanabiliriz
 <br><br>
Değişilik yapmak ile kastedilen CRUD operasyonlarından Create ve Update kısımlarını kapsar.
<br><br>
Ör: Post /createUser ile body kısmına kullanıcı bilgileri girip veritabanında bir kullanıcı oluşturulması istenmesi
</li>
<br><br><br>
<li><strong><em>PUT:</em></strong> Post isteğinin özelliklerine sahiptir. Yani CRUD operasyonlarından Create ve Update operasyonlarını yapmak istediğimizde kullanıyoruz. 
<br><br>
Post’dan ayrılan tarafı Put isteğinin idempotent ve not cacheable olarak tanımlanması
</li>
<br><br><br>
<li><strong><em>DELETE:</em></strong> CRUD operasyonlarından Delete’e karşılık gelir. Bir veriyi silmek istediğimizde kullanılması tavsiye ediliyor
 </li>
</ol>
<br><br>
<h2>API Nedir?</h2>
<br>
<p>API(Application Programming Interface) bizim dilimizde “Uygulama Programlama Arayüzü”, bir uygulamanın işlevlerine dışarıdan veya uzaktan erişilip bu işlevlerin kullanılmasını sağlayan arayüzdür. API, bir sunucunun üzerindeki uygulamaya farklı platformlardan ulaşılmasını ve response dönmesine olanak sağlar. Web API’lerinin tamamı REST(REpresentational State Transfer) mimarisi üzerinde dizayn edilir. Bundan dolayı platform bağımsız çalışır. Bu mimari GET, POST, PUT, DELETE metotlarının hepsini desteklemektedir. Web API çıktıları talebe göre JSON, XML gibi çeşitli çıktıları olabilir.</p>
<h2>API Kullanımı</h2>
<br>
<p>Amacı bir uygulamanın bütün veya bazı metotlarını diğer uygulamalara kullanıma açarak uzaktan gelecek veri ve bilgi taleplerini kolayca ve hızlıca karşılamaktadır. Böylelikle tek bir uygulamada gerçekleşen işlemlerden izin verilen uzak kullanıcılar belirli parametreler sayesinde faydalanabileceklerdir. API genel olarak gerçek zamanlı veriyi tek tek işlemeye yarar. Sunucunun API üzerinden gönderdiği parametre içeren veya içermeyen girdiyi sunucu işler ve geriye bir sonuç kümesi veya sadece başarı bildirimi döner. Verinin sadece belli bir kısmında yapılacak güncellemeler bir parametre gerektirir. API ise bu işlemlerin hem hızlı hemde pratik olmasını sağlar.</p>
<h2>Entegrasyonu Nasıl Yapılır?</h2>
<p>Karşıdaki sunucunun API üzerinden izin verdiği fonksiyonları kullanabilmek için istemciyi tanıtacak bir key gereklidir. Daha sonra bu key ile kullanılabilecek erişimi onaylayacak olan bir şifre almak gerekir. API hizmeti veren sunucu tarafındaki kurum, ilk olarak istemcinin başvurusunda key ve şifreyi ister. İstenen fonksiyonlar kullanılır ve istenen bilgiler karşı uygulamadan API’lerin döndüğü response’lar vasıtasıyla alınır. API’lara erişim ile ilgili kısıt konulabilir.</p>
<br>
<h2>API'nin Türleri Nelerdir?</h2>
<br>
<ul>
<li>Open API (diğer adıyla Public API) : Minimum kısıtlama ile geliştiriciler ve diğer kullanıcılar tarafından herkesin kullanımına açık API'lerdir.</li>
<li>Internal API (diğer adıyla Private API) : Harici kullanıcılardan gizlenir ve yalnızca dahili sistemler tarafından açığa çıkarılır. </li>
<li>Partner API : Stratejik iş ortaklarına veya stratejik iş ortakları tarafından sunulan API'lerdir. Herkese açık değildir ve bunlara erişmek için özel yetkilere ihtiyaçlar vardır. </li>
<li>Composite API : Composite API'ler birden çok veri veya hizmet API'sini birleştiren API'lerdir. </li>
</ul>
<br>
<h2>REST API ve SOAP API Nedir?</h2>
<br>
<p>API, programların birbirleriyle nasıl iletişim kurduğunu belirleyen belirli bir dizi kural iken, REST ve SOAP API'ler, API'nin nasıl sunulacağını tanımlar.</p>
<br>
<p>Her biri işlevsellik açısından benzerdir ancak birkaç temel farklılıklarla birbirlerinden ayrılırlar.</p>
<h2>SOAP API (Simple Access Protocol)</h2>
<ul>
<li>SOAP web servis çağrılarında RPC (Remote Procedure Call) modelini kullanan, istemci/sunucu mantığına dayalı bir protokol olarak ifade edilir</li>
<li>SOAP mesajları XML formatındadırlar ve genellikle HTTP(Hyper Text Transfer Protocol) protokolu(bazende TCP/IP) kullanılarak gönderilirler.</li>
<li>SOAP ,XML tabanlı kullanıma mecbur bırakır. Bu konuda esnek değildir.</li>

</ul>
<br>
<h2>REST API (Representational State Transfer)</h2>
<ul>
<li>HTTP metotlarını kullanan, esnek bir yapıya sahip, istemci – sunucu arasındaki basit bir veri iletişim yoludur. </li>
<li>Katı kurallara sahip bir protokolden ziyade bir mimari stildir.</li>
<li>Durumsuzdur (stateless), yani o anki kullanıcı durumu ya da geçmişinden habersizdir. </li>
<li>Servis yönelimli uygulamalarda REST bize lightweight bir çözüm yapısı sunar.</li>
<li>REST mimarisi kullanılan dil ve format bakımından gayet esnektir. JSON, XML hatta TEXT dosyasıyla bile veri alışverişi yapabilmemizi sağlar.</li>
<li>JSON ile aynı veriyi çok daha düşük boyutla taşıyabilir.</li>
<li>Web serviste çalışacak metot URI (Uniform Resource Identifier) yani Tekdüzen Kaynak Tanımlayıcısı ile HTTP üzerinden çağırılır.</li>
</ul>
<br>
<h2>Rest ile Soap Farkı</h2>
<p><strong>Güvenlik:</strong>SOAP üzerinde güvenlik(security) sağlamak daha kolay ve hızlı iken, bu durum REST için karmaşık olabiliyor.</p>
<p><strong>Data Yapısı:</strong>REST ile JSON, XML hatta TEXT ile çalışabiliyorken, SOAP ile XML kullanmalıyız. REST bu sayede daha kullanışlı olabiliyor.</p>
<p><strong>Uygulama Hızı:</strong>REST kullanımı, SOAP'a göre Uygulamanın daha hızlı çalışmasını sağlar</p>
<p><strong>Destek:</strong>SOAP için geliştirici araçları daha iyidir, yardımcı olacak daha çok kaynak bulabiliriz. REST’in dökümantasyonu SOAP’a göre daha azdır.</p>

<h2>RESTful API</h2>
<ul>
<li>Rest de temelinde HTTP protokolü üzerinden haberleşen bir mimari yaklaşımdır. Bu mimari yaklaşımı kullanan API'lara da Restful API olarak adlandırıyoruz. </li>
<li>Restful standardı daha eski ve katı kuralları olan SOAP servislere bir çözüm olarak geliştirilmiş ve tercih edilmiştir.</li>
<li>Restful olarak geliştirilmiş bir API üzerinden genellikle JSON tipinde dönüş yapılması tercih edilir fakat amaca ve isteğe göre XML, CSV, HTML veya düz bir metin olarak dönüş alabilirsiniz.</li>
<li>Restul API üzerinde HTTP protokünde yer alan çeşitli tipleri(GET,PUT,POST,DELETE) de etkin bir şekilde kullanıyoruz. Bu şekilde anlamlı URL'ler oluşturup göze ve programcıya hoş gelen linkler kolaylıkla oluşturuyoruz.</li>
</ul>


<P></P>
<P></P>

