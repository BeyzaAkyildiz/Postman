
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
<br><br><br>
<h2>API Nedir?</h2>
<br>
<p>API(Application Programming Interface) bizim dilimizde “Uygulama Programlama Arayüzü”, bir uygulamanın işlevlerine dışarıdan veya uzaktan erişilip bu işlevlerin kullanılmasını sağlayan arayüzdür. API, bir sunucunun üzerindeki uygulamaya farklı platformlardan ulaşılmasını ve response dönmesine olanak sağlar. Web API’lerinin tamamı REST(REpresentational State Transfer) mimarisi üzerinde dizayn edilir. Bundan dolayı platform bağımsız çalışır. Bu mimari GET, POST, PUT, DELETE metotlarının hepsini desteklemektedir. Web API çıktıları talebe göre JSON, XML gibi çeşitli çıktıları olabilir.</p>
<h2>API Kullanımı</h2>
<br>
<p>API kullanımın asıl amacı bir uygulamanın bütün veya bazı metotlarını diğer uygulamalara kullanıma açarak uzaktan gelecek veri ve bilgi taleplerini kolayca ve hızlıca karşılamaktadır. Böylelikle tek bir uygulamada gerçekleşen işlemlerden izin verilen uzak kullanıcılar belirli parametreler sayesinde faydalanabileceklerdir. API genel olarak gerçek zamanlı veriyi tek tek işlemeye yarar. Sunucunun API üzerinden gönderdiği parametre içeren veya içermeyen girdiyi sunucu işler ve geriye bir sonuç kümesi veya sadece başarı bildirimi döner. Verinin sadece belli bir kısmında yapılacak güncellemeler bir parametre gerektirir. API ise bu işlemlerin hem hızlı hemde pratik olmasını sağlar.</p>
<h2>Entegrasyonu Nasıl Yapılır?</h2>
<p>Entegrasyon tarafına gelecek olursak, karşıdaki sunucunun API üzerinden izin verdiği fonksiyonları kullanabilmek için öncelikle istemciyi tanıtacak bir key gereklidir. Daha sonra bu key ile kullanılabilecek erişimi onaylayacak olan bir şifre almak gerekir. API hizmeti veren sunucu tarafındaki kurum, ilk olarak istemcinin başvurusunda key ve şifreyi ister. İstenen fonksiyonlar kullanılır ve istenen bilgiler karşı uygulamadan API’lerin döndüğü response’lar vasıtasıyla alınır. İsteğe göre API’lara erişim ile ilgili kısıt konulabilir, bunun nedeni API’leri aşırı meşgul olmasını istememeden kaynaklıdır.</p>
<br>