# big_data_hf_2022
Ez a github repositoriy a BME Big Data elemzési módszerek nevű tantárgy beadandó házi feladatának fejlesztése céljából jött létre.
A projektben résztvevő hallgatók:
  1. Balog Marcell (D6W9SO)
  2. Lendvai Zsolt Dominik (KVBXU0)
  3. Móczó Árpád (F821WY)

Adatszótár:  
  - VendorID - a taxiszolgáltató kódja  
	○ 1= Creative Mobile Technologies, LLC; 2= VeriFone Inc.  
- tpep_pickup_datetime - Az taxióra bekapcsolásának dátuma és időpontja  
- tpep_dropoff_datetime - Az taxióra kikapcsolásának dátuma és időpontja  
- Passenger_count - A járműben lévő utasok száma  
- Trip_distance - A taxióra által jelentett megtett távolság mérföldben  
- PULocationID - TLC taxi zóna, amelyben a taxamétert bekapcsolták. (TLC = az adatokat szolgáltató társaság)  
- DOLocationID - TLC Taxi zóna, amelyben a taxamétert kikapcsolták.  
- RateCodeID - Az út végén érvényes végső díjszabási kód.  
	○ 1= Standard tarifa  
	○ 2=JFK  
	○ 3=Newark  
	○ 4=Nassau vagy Westchester  
	○ 5=Megegyezés alapú tarifa  
	○ 6=Csoportos utazás  
- Store_and_fwd_flag - Ez azt jelzi, hogy az utazási mérést a jármű memóriájában tartották-e, mielőtt elküldték volna a társaságnak, más néven "tárolás és továbbítás", mert a jármű nem kapcsolódott akkor a szerverhez.  
	○ Y= tárolás és továbbítás  
	○ N= nem tárolás és továbbítás  
- Payment_type Számkód, amely azt jelzi, hogy az utas hogyan fizetett az utazásért.  
	○ 1= Hitelkártya  
	○ 2= Készpénz  
	○ 3= Nincs díj  
	○ 4= Vitatott?  
	○ 5= Ismeretlen  
	○ 6= Törölt utazás  
- Fare_amount - A mérő által kiszámított idő- és távolsági viteldíj.  
- Extra - Különféle extrák és pótdíjak. Itt ez csak a 0,50 és az 1 dolláros csúcsforgalmi és éjszakai díjakat tartalmazza.  
- MTA_tax - $0.50 MTA-adó, amely automatikusan levonódik a mérőórák alapján.  
- Improvement_surcharge - $0,30 javítási pótdíj, amely aladíjként mindig fel van számolva.  
- Tip_amount - Borravaló összege - Csak hitelkártyás fizetés esetén, készpénzes fizetésnél nincs jegyezve.  
- Tolls_amount - Az utazás során fizetett összes útdíj (/autópályadíj) teljes összege.  
- Total_amount - Az utasoknak felszámított teljes összeg. Nem tartalmazza a készpénzes borravalót.  
- Congestion_Surcharge - Az út során a NYS (New York State) dugódíjra beszedett teljes összeg.  
- Airport_fee - $1,25 csak a LaGuardia és John F. Kennedy repülőtereken történő felvétel esetén.  
- trip duration - utazási idő, percben (kiszámítva az utazás kezdő és befejező időpontjaiból)  
- taxi speed - taxi haladási sebessége (m/h)  
- speed category - (0/1) azt nézi, hogy átlagsebesség alatti vagy fölötti volt a trip  
- tip percentage - mekkora hányada a tip a teljes összegnek  
- time slot - melyik napszakban volt az utazás  



