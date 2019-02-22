# spring-hello-zipkin

====
必要なもの
* Localhost:9411で上がってくるZipkinのDockerコンテナ(デフォルトでDocker runする）

----
使い方
1.localhost:8080/へアクセスする  
2.localhost:9411のZipkinGUIでドリルダウンしてみる  
⇒ただし、画面に対してリクエストを投げていて、内部呼び出しではないので、IDは別となるので改善が必要
