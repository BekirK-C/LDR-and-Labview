# LDR-and-Labview

Arduino ile LDR sensörden alınan verilere göre LabVIEW programında ışık şiddetine göre LED yakmak.


## Labview_Project Dosyası Hakkında

Arduino kodlarını içeren dosyadır. Serial portla haberleşme sağlanıp Arduino'nun A0 bacağına bağlanan pinden analog okuma yapılır ve Serial olarak yazdırılır.

## LDR Sensor ile LED Kontrolu Dosyası Hakkında

Projenin VI dosyasını içerir. Front panelde Gauge gösterge paneli, 3 tane gösterge ledi, 2 tane  numerik kontrol paneli, 1 tane port kontrol paneli ve stop durdurma düğmesi bulunmaktadır. Back panelde gerekli VISA haberleşmesi yapılıp döngü içinde daha önceden belirlenen referans değerlere göre karşılaştırma yapılmaktadır.

## Images Hakkında

Projenin 3 ayrı haldeki (Düşük, Normal ve Yüksek ışıkta) fotoğrafını içerir. 

## Nasıl Çalışır

Öncelikle Yazdığımız Arduino kodlarını Arduino'ya yüklüyoruz. Ardından yine Serial olarak Arduino ile haberleşme sağlayıp oluşturduğumuz LabVIEW dosyasını açıyoruz. Açılan projede serial port panelinden Arduino'yu bağladığımız COM'u seçmeli ve 'Normal' ve 'Yüksek' olarak adlandırılan referans değerlerini belirlemeliyiz. 
Arduino'nun A0 pinine bağlı olan LDR sensörden okunan değerler VI'daki Gauge göstergesinden okunabilir. Önceden belirlenen referans değerlerine göre ışık şiddetini ledlerle düşük, normal veya yüksek olarak görebiliriz.

## NOT

LabVIEW projesini çalıştırmadan önce Serial portta Arduinonun bağlı olduğu COM seçilmeli ve ışık şiddeti referans değerleri yazılmalıdır.
