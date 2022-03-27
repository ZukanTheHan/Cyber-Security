# Tehdit, Zafiyet ve Risk

Tehdit (Threat) ⇒ Veriler veya ağın kendisi gibi varlıklar için potansiyel tehlikedir. 

Zafiyet (Vulnerability) ⇒ Bir tehdit tarafından istismar edilebilecek bir sistemdeki veya tasarımındaki bir zayıflık.

Saldırı Yüzeyi (Attack surface) ⇒ Saldırı yüzeyi, belirli bir sistemdeki bir saldırganın erişebildiği güvenlik açıklarının toplamıdır. Saldırı yüzeyi, bir saldırganın sisteme girebileceği ve sistemden verileri alabileceği farklı noktaları tanımlar. Örneğin, işletim sisteminiz ve web tarayıcınız güvenlik  Birlikte, tehdit aktörünün yararlanabileceği bir saldırı yüzeyi oluştururlar.

İstismar (Exploit) ⇒ Bir varlığın güvenlik açığından yararlanmak için kullanılan mekanizma. İstismarlar uzak veya yerel olabilir. Uzaktan istismar, hedef sisteme önceden erişim olmadan ağ üzerinden çalışan bir istismardır. Saldırganın bu güvenlik açığından yararlanabilmesi için son sistemde bir hesaba ihtiyacı yoktur. Yerel bir istismarda, tehdit aktörünün son sisteme bir tür kullanıcı veya yönetici erişimi vardır. Yerel güvenlik açıklarından yararlanma, saldırganın son sisteme fiziksel erişimi olduğu anlamına gelmez.

Risk ⇒ Belirli bir tehdidin, bir varlığın belirli bir güvenlik açığından yararlanma ve istenmeyen bir sonuçla sonuçlanma olasılığı.

Risk yönetimi, varlığın korunmasıyla elde edilen kazanımlar ile koruyucu önlemlerin sağlanmasının operasyonel maliyetlerini dengeleyen süreçtir.

Riski kabul etme (Risk acceptance) ⇒ Bu, risk yönetimi seçeneklerinin maliyetinin riskin kendi maliyetinden daha ağır basmasıdır. Risk kabul edilir ve herhangi bir işlem yapılmaz.

Riskten kaçma (Risk avoidance) ⇒ Bu, riski taşıyan faaliyeti veya cihazı ortadan kaldırarak riske maruz kalmaktan kaçınmak anlamına gelir. Riskten kaçınmak için bir faaliyetin ortadan kaldırılmasıyla, faaliyetten elde edilebilecek tüm faydalar da kaybedilir.

Risk azaltma (Risk reduction) ⇒ Bu, riski azaltmak için harekete geçerek riske maruz kalmayı azaltır veya riskin etkisini azaltır. Bu strateji, zarar maliyetlerinin, hafifletme stratejisinin ve risk altındaki operasyon veya faaliyetten elde edilen faydaların dikkatli bir şekilde değerlendirilmesini gerektirir.

Risk transferi ⇒ Riskin bir kısmı veya tamamı, sigorta şirketi gibi istekli bir üçüncü şahsa devredilir.

## Tehdit Aktörlerinin Kullandığı Araçlar

Pek çok araç ağın ve sistemin güvenliğini sınamak için geliştirilmiştir ama tehdit aktörleri tarafından da saldırı amacıyla kullanılabilir. Tehdit aktörlerinin de bilgisayara korsanlığı için geliştirdiği pek çok araç mevcuttur. 

**Şifre kırıcılar** ⇒ Parola kırma araçları genellikle parola kurtarma araçları olarak adlandırılır ve parolayı kırmak veya kurtarmak için kullanılabilir. Bu, ya veri şifrelemesini atladıktan sonra orijinal parolayı kaldırarak ya da parolanın doğrudan keşfedilmesiyle gerçekleştirilir. Şifre kırıcılar, şifreyi kırmak ve sisteme erişmek için defalarca tahminlerde bulunur. Parola kırma araçlarına örnek olarak John the Ripper, Ophcrack, L0phtCrack, THC Hydra, RainbowCrack ve Medusa verilebilir.

**Kablosuz bilgisayar korsanlığı araçları** ⇒ Kablosuz ağlar, ağ güvenliği tehditlerine karşı daha hassastır. Kablosuz bilgisayar korsanlığı araçları, güvenlik açıklarını tespit etmek için bir kablosuz ağa kasıtlı olarak girmek için kullanılır. Kablosuz bilgisayar korsanlığı araçlarına örnek olarak Aircrack-ng, Kismet, InSSIDer, KisMAC, Firesheep ve NetStumbler verilebilir.

**Ağ tarama ve bilgisayar korsanlığı araçları** ⇒ Ağ tarama araçları, açık TCP veya UDP bağlantı noktaları için ağ cihazlarını, sunucuları ve bilgisayarları araştırmak için kullanılır. Tarama araçlarına örnek olarak Nmap, SuperScan, Angry IP Scanner ve NetScanTools verilebilir.

**Paket hazırlama araçları** ⇒ Paket oluşturma araçları, özel olarak hazırlanmış sahte paketleri kullanarak bir güvenlik duvarının sağlamlığını test etmek için kullanılır. Bu tür araçların örnekleri arasında Hping, Scapy, Socat, Yersinia, Netcat, Nping ve Nemesis bulunur.

**Paket koklayıcılar** ⇒ Paket koklayıcı araçları, geleneksel Ethernet LAN'lar veya WLAN'lar içindeki paketleri yakalamak ve analiz etmek için kullanılır. Araçlar arasında Wireshark, Tcpdump, Ettercap, Dsniff, EtherApe, Paros, Fiddler, Ratproxy ve SSLstrip bulunur.

**Rootkit dedektörleri** ⇒ Bir rootkit algılayıcısı, beyaz şapkalar tarafından kurulu kök kitleri tespit etmek için kullanılan bir dizin ve dosya bütünlüğü denetleyicisidir. Örnek araçlar arasında AIDE, Netfilter ve PF: OpenBSD Packet Filter bulunur.

**Güvenlik açıklarını aramak için fuzzers** ⇒ Fuzzers, bir bilgisayar sisteminin güvenlik açıklarını keşfetmeye çalışırken tehdit aktörleri tarafından kullanılan araçlardır. Fuzzers örnekleri arasında Skipfish, Wapiti ve W3af bulunur.

**Adli aletler (Forensic tools)** ⇒ Adli bilişim uzmanları, belirli bir bilgisayar sisteminde var olan herhangi bir kanıtı bulmak için adli araçlar kullanır. Araçlara örnek olarak Sleuth Kit, Helix, Maltego ve Encase dahildir.

**Hata ayıklayıcılar (Debugger)** ⇒ Hata ayıklayıcı araçları, istismar (exploit) yazarken ikili dosyalarda tersine mühendislik (reverse engineering) uygulamak için saldırganlar tarafından kullanılır. Kötü amaçlı yazılımları analiz ederken güvenlik uzamanları tarafından da kullanılırlar. Hata ayıklama araçları arasında GDB, WinDbg, IDA Pro ve Bağışıklık Hata Ayıklayıcı bulunur.

**İşletim sistemleri** ⇒ Bilgisayar korsanlığı işletim sistemleri, bilgisayar korsanlığı için optimize edilmiş araçlar ve teknolojilerle önceden yüklenmiş özel olarak tasarlanmış işletim sistemleridir. Özel olarak tasarlanmış bilgisayar korsanlığı işletim sistemlerine örnek olarak Kali Linux, SELinux, Knoppix, Parrot OS ve BackBox Linux verilebilir.

**Şifreleme araçları** ⇒ Bu araçlar, depolandığında veya iletildiğinde bir kuruluşun verilerinin içeriğini korur. Şifreleme araçları, verilere yetkisiz erişimi önlemek için algoritma şemaları kullanır. Bu araçlara örnek olarak VeraCrypt, CipherShed, Open SSH, OpenSSL, OpenVPN ve Stunnel verilebilir.

**Güvenlik açığı istismar araçları** ⇒ Bu araçlar, uzaktaki bir bilgisayarın bir güvenlik saldırısına açık olup olmadığını belirler. Güvenlik açığı istismar araçlarına örnek olarak Metasploit, Core Impact, Sqlmap, Social Engineer Tool Kit ve Netsparker verilebilir.

**Güvenlik açığı tarayıcıları** ⇒ Bu araçlar, açık bağlantı noktalarını belirlemek için bir ağı veya sistemi tarar. Ayrıca bilinen güvenlik açıklarını taramak ve VM'leri, BYOD cihazlarını ve istemci veritabanlarını taramak için de kullanılabilirler. Bu araçların örnekleri arasında Nipper, Securia PSI, Core Impact, Nessus, SAINT ve Open VAS bulunur.

## IOC ve IOA 
Pek çok ağ saldırısı, güvenlik ihlali göstergeleri (IOC) hakkında bilgi paylaşılarak önlenebilir. Her saldırının benzersiz tanımlanabilir nitelikleri vardır. Güvenlik ihlali göstergeleri, bir saldırının gerçekleştiğinin kanıtıdır. IOC'ler, diğerlerinin yanı sıra kötü amaçlı yazılım dosyalarını, saldırılarda kullanılan sunucuların IP adreslerini, dosya adlarını ve sistem yazılımını sonlandırmak için yapılan karakteristik değişiklikleri tanımlayan özellikler olabilir. IOC'ler, siber güvenlik personelinin bir saldırıda ne olduğunu belirlemesine ve saldırıya karşı savunma geliştirmesine yardımcı olur. 

Saldırı göstergeleri (IOA), bir saldırının arkasındaki motivasyona ve varlıklara erişim elde etmek için hangi tehdit aktörlerinin güvenlik açıklarından yararlanabileceği potansiyeline daha fazla odaklanır. IOA'lar saldırganlar tarafından kullanılan stratejilerle ilgilenir. Bu nedenle, tek bir tehdide yanıtı bildirmek yerine, IOA'lar proaktif bir güvenlik yaklaşımı oluşturmaya yardımcı olabilir. Bunun nedeni, stratejilerin birden çok bağlamda ve birden çok saldırıda yeniden kullanılabilmesidir. Bu nedenle, bir stratejiye karşı savunma, aynı veya benzer stratejiyi kullanan gelecekteki saldırıları önleyebilir. 

