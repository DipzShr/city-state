# city-state Ruby Gem

**city-state** is a very simple Ruby Gem that you can use to get a list of states of a country. Also, you can get a list of cities from a state.

## Put this gem at your Gemfile:
```ruby
gem 'city-state'
```

## Get a list of states:
```ruby
CS.states(:us)
# => {:AK=>"Alaska", :AL=>"Alabama", :AR=>"Arkansas", :AZ=>"Arizona", :CA=>"California", :CO=>"Colorado", :CT=>"Connecticut", :DC=>"District of Columbia", :DE=>"Delaware", :FL=>"Florida", :GA=>"Georgia", :HI=>"Hawaii", :IA=>"Iowa", :ID=>"Idaho", :IL=>"Illinois", :IN=>"Indiana", :KS=>"Kansas", :KY=>"Kentucky", :LA=>"Louisiana", :MA=>"Massachusetts", :MD=>"Maryland", :ME=>"Maine", :MI=>"Michigan", :MN=>"Minnesota", :MO=>"Missouri", :MS=>"Mississippi", :MT=>"Montana", :NC=>"North Carolina", :ND=>"North Dakota", :NE=>"Nebraska", :NH=>"New Hampshire", :NJ=>"New Jersey", :NM=>"New Mexico", :NV=>"Nevada", :NY=>"New York", :OH=>"Ohio", :OK=>"Oklahoma", :OR=>"Oregon", :PA=>"Pennsylvania", :RI=>"Rhode Island", :SC=>"South Carolina", :SD=>"South Dakota", :TN=>"Tennessee", :TX=>"Texas", :UT=>"Utah", :VA=>"Virginia", :VT=>"Vermont", :WA=>"Washington", :WI=>"Wisconsin", :WV=>"West Virginia", :WY=>"Wyoming"} 
```

## Get a list of cities:
```ruby
CS.cities(:ak)
# => ["Adak", "Akhiok", "Akiachak", "Akiak", "Akutan", "Alakanuk", "Ambler", "Anchor Point", "Anchorage", "Angoon", "Atqasuk", "Barrow", "Bell Island Hot Springs", "Bethel", "Big Lake", "Buckland", "Chefornak", "Chevak", "Chicken", "Chugiak", "Coffman Cove", "Cooper Landing", "Copper Center", "Cordova", "Craig", "Deltana", "Dillingham", "Douglas", "Dutch Harbor", "Eagle River", "Eielson Air Force Base", "Fairbanks", "Fairbanks North Star Borough", "Fort Greely", "Fort Richardson", "Galena", "Girdwood", "Goodnews Bay", "Haines", "Homer", "Hooper Bay", "Juneau", "Kake", "Kaktovik", "Kalskag", "Kenai", "Ketchikan", "Kiana", "King Cove", "King Salmon", "Kipnuk", "Klawock", "Kodiak", "Kongiganak", "Kotlik", "Koyuk", "Kwethluk", "Levelock", "Manokotak", "May Creek", "Mekoryuk", "Metlakatla", "Mountain Village", "Nabesna", "Naknek", "Nazan Village", "Nenana", "New Stuyahok", "Nikiski", "Ninilchik", "Noatak", "Nome", "Nondalton", "Noorvik", "North Pole", "Northway", "Old Kotzebue", "Palmer", "Pedro Bay", "Petersburg", "Pilot Station", "Point Hope", "Point Lay", "Prudhoe Bay", "Russian Mission", "Sand Point", "Scammon Bay", "Selawik", "Seward", "Shungnak", "Sitka", "Skaguay", "Soldotna", "Stebbins", "Sterling", "Sutton", "Talkeetna", "Teller", "Thorne Bay", "Togiak", "Tok", "Toksook Bay", "Tuntutuliak", "Two Rivers", "Unalakleet", "Unalaska", "Valdez", "Wainwright", "Wasilla"]
```

## Update the database from MaxMind:
```ruby
CS.update
```

## Another countries:

When getting a city list, you can also specifies the country:
```ruby
CS.cities(:sp, :br)
```

The country is an optional argument. **city-state** always uses the last country that you used.
```ruby
CS.states(:br)
#  => {:AC=>"Acre", :AL=>"Alagoas", :AM=>"Amazonas", :AP=>"Amapa", :BA=>"Bahia", :CE=>"Ceara", :DF=>"Federal District", :ES=>"Espirito Santo", :GO=>"Goias", :MA=>"Maranhao", :MG=>"Minas Gerais", :MS=>"Mato Grosso do Sul", :MT=>"Mato Grosso", :PA=>"Para", :PB=>"Paraiba", :PE=>"Pernambuco", :PI=>"Piaui", :PR=>"Parana", :RJ=>"Rio de Janeiro", :RN=>"Rio Grande do Norte", :RO=>"Rondonia", :RR=>"Roraima", :RS=>"Rio Grande do Sul", :SC=>"Santa Catarina", :SE=>"Sergipe", :SP=>"Sao Paulo", :TO=>"Tocantins"}
CS.cities(:to)
#  => ["Aparecida do Rio Negro", "Araguaína", "Brejinho de Nazare", "Gurupi", "Itaguatins", "Miracema do Tocantins", "Monte Alegre", "Palmas", "Paraiso do Tocantins", "Parana", "Pedro Afonso", "Porto Nacional", "Presidente Kennedy", "Salvador", "Santo Antonio", "Sao Domingos", "Taguatinga", "Tucum"] 
```

# City-State License
city-state is a open source project by Daniel Loureiro with a MIT license. Also, it uses MaxMind open source database.

# MaxMind License
Database and Contents Copyright (c) 2015 MaxMind, Inc.
This work is licensed under the Creative Commons Attribution 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/.
