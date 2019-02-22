# spring-hello-zipkin


単に、SpringBootをローカルで稼働させて、ZipkinへID連携を確認するだけのアプリ。


必要なもの
----
* java11
* Localhost:9411で上がってくるZipkinのDockerコンテナ(デフォルトでDocker runする）


使い方  
----
    > ./mvnw clean package -DskipTests=true
    > java -jar .\target\hello-0.0.1-SNAPSHOT.jar
    > docker run -d -p 9411:9411 openzipkin/zipkin
    
localhost:8080/へアクセスする  
localhost:9411のZipkinGUIでドリルダウンしてみる  
⇒ただし、画面に対してリクエストを投げていて、内部呼び出しではないので、IDは別となるので改善が必要
