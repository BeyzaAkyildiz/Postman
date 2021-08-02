<h1>Postman Nedir?</h1>


--------------
<ul>
<li>Postman, Chrome uzantısı olarak kullanabileceğimiz veya direct indirip bilgisayarımıza yükleyebileceğimiz bir uygulamadır. Rest Client olarak da tanımlanabilir.</li>
<li>API(Application Programming Interface) farklı uygulama yazılımlarının birbirleri ile etkileşim sağlamasına olanak sağlar. Client(Android) ve Backend(java) yazılımlarının Restfull Api ile iletişim kurması buna örnek verilebilir.</li>
<li>Postman sayesinde uzun uzun kodlar yazmak yerine API’lerimizi kolayca test edebiliriz. Birçok özelliği sayesinde kolay bir şekilde istek hazırlayıp gelen cevap değerlerini kullanabiliriz</li>
</ul>
<br><br><br>
<h2>POST-GET-PUT-DELETE</h2>
 
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
<p>API(Application Programming Interface) bizim dilimizde “Uygulama Programlama Arayüzü”, bir uygulamanın işlevlerine dışarıdan veya uzaktan erişilip bu işlevlerin kullanılmasını sağlayan arayüzdür. API, bir sunucunun üzerindeki uygulamaya farklı platformlardan ulaşılmasını ve response dönmesine olanak sağlar. Web API’lerinin tamamı REST(REpresentational State Transfer) mimarisi üzerinde dizayn edilir. Bundan dolayı platform bağımsız çalışır. Bu mimari GET, POST, PUT, DELETE metotlarının hepsini desteklemektedir. Web API çıktıları talebe göre JSON, XML gibi çeşitli çıktıları olabilir.</p>