1. Öncelikle application.properties dosyasından sizde kullanılacak postgresql veritabanın bilgileri girilmeli.
	(Normalde local denemelerde "jdbc:postgresql://localhost:5432/mydatabase"  şekilde kullanıyordum.
	Fakat proje docker a attığımda veritabanına bağlanamadı. Bu yüzden localhost yerine kendi ip adresimi yazdım.)

	spring.datasource.url=jdbc:postgresql://host:port/db  
	spring.datasource.username=username
	spring.datasource.password=password
 
	şeklinde. (db'yi ben mydatabase şeklinde bir db oluşturmuştum.)


2. > cd projeninBulunduğuDizin  (C:\Users\kanko\Spring_İndirmeleri\rehber gibi)

3. > docker build -t rehber .

4. > docker run -d -p 8888:8080 -it e36376273b2c

5. > docker ps

6. Proje docker'da ayağa kalktıktan sonra "localhost:8888/swagger-ui.html" adresinden denemeleri yapabiliriz.

