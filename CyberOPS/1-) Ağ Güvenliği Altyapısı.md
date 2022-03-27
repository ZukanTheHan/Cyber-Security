# Ağ Güvenliği Altyapısı

![image](https://user-images.githubusercontent.com/70758694/159547619-2964c04c-d561-473d-99f5-efab2dd570f0.png)

Ağ güvenliğinde temelde iki tür ağ vardır, iç ağ (private - güvenilir) ve dış ağ (public - güvenilmeyen). Temel prensib iç ağın dış ağa çıkışına izin vermek ve dış ağdan gelebilecek doğrudan bağlantıları engellemektir. Yukarıdaki görselde bu temel prensip anlatılmıştır. 

## Demilitarized zone (DMZ)

![image](https://user-images.githubusercontent.com/70758694/159548508-ea0b7d39-63c0-4b7a-9ce2-b73b0d0abebc.png)

DMZ, şekilde görüldüğü gibi bir iç ağ, dış ağ ve DMZ biriminin bulunduğu bir firewall tasarımdır. Bu tasarımı genellikle dış ağa açılmak istenen servisler olduğunda tercih edilir. Örnek olarak bir web suncucusu verilebilir. 

- İç ağdan DMZ veya dış ağa yapılan trafik denetlenir ve buna çoğu zaman izin verilir. 
- DMZ veya dış ağdan iç ağa cevap olarak trafikte denetlendikten sonra iletilir. 
- DMZ ağından kaynaklanan trafik iç ağa yöneliyorsa bu engellenir. Aynı şekilde doğrudan dış ağdan iç ağa doğru başlatılan bir trafik yine firewall tarafından engellenir. 
- DMZ ağından başlatılan ve dış ağa doğru gönderilen trafikse hizmet gereksinimlerine göre seçici olarak izin verilir. Dış ağdan DMZ ağına başlatılan trafik denetlenir ve izin verilir. 

Buradaki asıl amaç güvenilmeyen dış ağdan gelen bir tehdit eğer DMZ bölgesinde bulunan bir cihaza saldırır ve onu geliçirirse iç ağa bulaşıp daha fazla zarar vermesini engellemektir. 

## Zone-based policy firewalls

![image](https://user-images.githubusercontent.com/70758694/159550606-9e434cb5-4584-4399-aa55-0595993adf6c.png)

Bölge tabanlı ilke güvenlik duvarları (ZPF'ler), ek esneklik sağlamak için bölge kavramını kullanır. Bölge, benzer işlevlere veya özelliklere sahip bir veya daha fazla arabirim grubudur. Varsayılan olarak, aynı bölgedeki arayüzler arasındaki trafik herhangi bir politikaya tabi değildir ve serbestçe geçer. Ancak, bölgeden bölgeye tüm trafik engellenir. Bölgeler arasındaki trafiğe izin vermek için, trafiğe izin veren veya trafiği denetleyen bir ilke yapılandırılmalıdır.

Bu varsayılan olarak hepsini reddetme ilkesinin tek istisnası, yönlendiricinin (router) kendi bölgesidir. Self zone, yönlendiricinin kendisidir ve yönlendiricinin tüm  arabirim IP adreslerini içerir. Self zone içeren ilke yapılandırmaları, yönlendiriciye yönlendirilen ve yönlendiriciden kaynaklanan trafiğe uygulanır. Varsayılan olarak, bu tür trafik için bir politika yoktur. Self zone için bir politika tasarlarken dikkate alınması gereken trafikler, SSH, SNMP ve yönlendirme protokolleri gibi yönetim ve kontrol trafikleridir.
