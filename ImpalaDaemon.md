 # Impala Daemon
Çekirdek Impala bileşeni, kümenin her DataNode'unda çalışan ve fiziksel olarak işlenen süreçle temsil edilen bir süreçtir. Veri dosyalarını okur ve yazar; Impala-shell komutu, Hue, JDBC veya ODBC'den iletilen sorguları kabul eder; Sorguları paralelleştirir ve kümelenme boyunca dağıtır; ve ara sorgu sonuçlarını merkezi koordinatör düğüme geri gönderir.Herhangi bir DataNode üzerinde çalışan Impala daemon'a bir sorgu gönderebilir ve bu daemonun o örneği bu sorgu için koordinatör düğümü olarak hizmet verir. Diğer düğümler kısmi sonuçları bir sorgu için belirlenen nihai sonucu oluşturan koordinatöre geri gönderir. Impala-shell komutuyla işlevsellikli deneyler çalıştırırken, kolaylık sağlamak için her zaman aynı Impala servisine bağlanabilirsiniz. Üretim işyüklerini çalıştıran kümeler için, JDBC veya ODBC arabirimlerini kullanarak, her bir sorguyu yuvarlak bir dize tarzında farklı bir Impala arka planına göndererek denge yükleyebilirsiniz.