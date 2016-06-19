#########################################################################################
#                          Witaj w konfiguracji skryptu  Drop.                          #
#                                                                                       #
#                                      INFORMACJE                                       #
#                                                                                       #
#                           W skrypcie będą używane wartości:                           #
#                              true - oznacza TAK/WŁĄCZONY                              #
#                             false - oznacza NIE/WYŁĄCZONY                             #
#                                                                                       #
#                        Każda opcja nie będzie opisywana po kolei.                     #
#                     Z każdej "kategori" opisana jest jedna "sekcja".                  #
#                                                                                       #
#                      Skrypt  Drop został stworzony przez VillainTM.                   #
#                                                                                       #
#########################################################################################
configuration:
  drop:
# Konfiguracja dropu węgla.
    coal:
      #Szansa na znalezienie węgla. (podana w procentach)
      chance: '10.0'
    
      #Wysokość, od której możemy znaleźć węgiel.
      height: '100'
    
      #Wybór kilofów, jakimi możemy znaleźć węgiel.
      pickaxes:
        #Drewniany kilof.
        wood: 'true'
    
        #Kamienny kilof.
        stone: 'true'
    
        #Żelazny kilof.
        iron: 'true'
    
        #Złoty kilof.
        gold: 'true'
    
        #Diamentowy kilof.
        diamond: 'true'
    
      #Zarządzanie wypadaniem węgla z rudy.
      ore:
        #Czy węgiel ma wypadać z rudy.
        drop: 'false'
    
        #Jeżeli powyższa opcja jest wyłączona, to na jaki blok ma zamieniać rudę po zniszczeniu.
        replace: stone
    
        #Wiadomość ukazana, gdy wylatywanie węgla z rudy jest wyłączone.
        #Pozostaw puste (message: '') jeżeli nie chcesz, aby wiadomość się ukazała.
        message: '&b&lWegiel &fwypada ze &astone&f.'
# Konfiguracja dropu żelaza.
    iron:
      chance: '9.0'
      height: '80'
      pickaxes:
        wood: 'false'
        stone: 'true'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
      ore:
        drop: 'false'
        replace: stone
        message: '&b&lZelazo &fwypada ze &astone&f.'
# Konfiguracja dropu lazurytu.
    lapis:
      chance: '6.0'
      height: '70'
      pickaxes:
        wood: 'false'
        stone: 'true'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
      ore:
        drop: 'false'
        replace: stone
        message: '&b&lLazuryt &fwypada ze &astone&f.'
# Konfiguracja dropu złota.
    gold:
      chance: '6.0'
      height: '75'
      pickaxes:
        wood: 'false'
        stone: 'false'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
      ore:
        drop: 'false'
        replace: stone
        message: '&b&lZloto &fwypada ze &astone&f.'
# Konfiguracja dropu diamentów.
    diamond:
      chance: '4.0'
      height: '50'
      pickaxes:
        wood: 'false'
        stone: 'false'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
      ore:
        drop: 'false'
        replace: stone
        message: '&b&lDiament &fwypada ze &astone&f.'
# Konfiguracja dropu ksiazek.
    redstone:
      chance: '8.0'
      height: '65'
      pickaxes:
        wood: 'false'
        stone: 'false'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
# Konfiguracja dropu jablek.
    apple:
      chance: '8.0'
      height: '70'
      pickaxes:
        wood: 'false'
        stone: 'false'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
# Konfiguracja dropu czerwonego kamienia.
    redstone:
      chance: '7.0'
      height: '60'
      pickaxes:
        wood: 'false'
        stone: 'false'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
      ore:
        drop: 'false'
        replace: stone
        message: '&b&lCzerwony kamien &fwypada ze &astone&f.'
# Konfiguracja dropu szmaragdów.
    emerald:
      chance: '10.0'
      height: '100'
      pickaxes:
        wood: 'false'
        stone: 'false'
        iron: 'true'
        gold: 'false'
        diamond: 'true'
      ore:
        drop: 'false'
        replace: stone
        message: '&b&lSzmaragd &fwypada ze &astone&f.'
# Konfiguracja poziomów kopania.
  level:
    #Czy włączyć poziomy kopania.
    enable: 'true'
  
    #O ile punktów dodaje nam wymaganych do następnego poziomu.
    #Przykład: opcja jest ustawiona na 100.
    #Po uzyskaniu 100 punktów otrzymujemy 2 poziom.
    #Po uzyskaniu 200 punktów otrzymujemy 3 poziom.
    needed: '100'
#Konfiguracja "boosterów".
  multiplier:
    #Ile ma dodawać procent szansy na drop przy zaklęciu "szczęście 1".
    fortune1: '4'
  
    #Ile ma dodawać procent szansy na drop przy zaklęciu "szczęście 2".
    fortune2: '5'
  
    #Ile ma dodawać procent szansy na drop przy zaklęciu "szczęście 3".
    fortune3: '7'
  
    #Ile ma dodawać procent szansy na drop posiadając uprawnienie "nDrop.super-drop" lub "nDrop.*"
    super-drop: '5'
  
    #Ile ma dodawać procent szansy na drop, gdy "turbo drop" jest włączony.
    turbo-drop: '8'
  
    #Ile ma dodawać dodatkowo kulek doświadczenia, gdy "turbo experience" jest włączony.
    turbo-experience: '10'
#Konfiguracja wiadomości.
  messages:
    #Przedrostek przed wiadomościami.
    tag: '&6&lnDrop &e>'
  
    #Wiadomość ukazana, gdy nie mamy uprawnień do danej komendy.
    # {permission} zamieniane jest na wymagane uprawnienie
    nopermission: '&cBrak uprawnien! &7({permission})'
  
    #Wiadomość ukazana, gdy wpisany w komendzie gracz nie został znaleziony.
    playernotfound: '&cNie znaleziono gracza! &7(Wielkosc liter ma znaczenie)'
  
    #Wiadomość ukazana, gdy zdobędziemy nowy poziom kopania.
    newlevel: '&fGracz &a{player} &fawansowal na poziom &a{level}&f.'
  
    #Wiadomość ukazana, gdy znajdziemy surowiec kopiąc kamień.
    #Pozostaw puste (drop: '') jeżeli chcesz, aby wiadomość się nie ukazała.
    drop: '&fWykopales: &a{amount} {item} &7(+{points} pkt.)'
#Konfiguracja włączania/wyłączania poszczególnych rzeczy.
    turbo-drop:
      #Wiadomość ukazywana, gdy "turbo drop" zostanie włączony.
      enabled: '&b&lTurbo drop &fzostal &awlaczony&f.'
    
      #Wiadomość ukazywana, gdy "turbo drop" zostanie wyłączony.
      disabled: '&b&lTurbo drop &fzostal &cwylaczony&f.'
    turbo-experience:
      enabled: '&b&lTurbo experience &fzostal &awlaczony&f.'
      disabled: '&b&lTurbo experience &fzostal &cwylaczony&f.'
    item-drop:
      coal:
        #Wiadomość ukazywana, gdy wypadanie węgla zostanie włączone.
        enabled: '&fDrop &b&lwegla &fzostal &awlaczony&f.'
    
        #Wiadomość ukazywana, gdy wypadanie węgla zostanie wyłączone.
        disabled: '&fDrop &b&lwegla &fzostal &cwylaczony&f.'
      iron:
        enabled: '&fDrop &b&lzelaza &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&lzelaza &fzostal &cwylaczony&f.'
      book:
        enabled: '&fDrop &b&lksiazek &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&lksiazek &fzostal &cwylaczony&f.'
      apple:
        enabled: '&fDrop &b&ljablek &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&ljablek &fzostal &cwylaczony&f.'
      lapis:
        enabled: '&fDrop &b&llazurytu &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&llazurytu &fzostal &cwylaczony&f.'
      gold:
        enabled: '&fDrop &b&lzlota &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&lzlota &fzostal &cwylaczony&f.'
      diamond:
        enabled: '&fDrop &b&ldiamentu &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&ldiamentu &fzostal &cwylaczony&f.'
      redstone:
        enabled: '&fDrop &b&lczerwonego kamienia &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&lczerwonego kamienia &fzostal &cwylaczony&f.'
      emerald:
        enabled: '&fDrop &b&lszmaragdu &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&lszmaragdu &fzostal &cwylaczony&f.'
      cobble-stone:
        enabled: '&fDrop &b&lcobblestone/stone &fzostal &awlaczony&f.'
        disabled: '&fDrop &b&lcobblestone/stone &fzostal &cwylaczony&f.'
  other:
    #Czy "turbo drop" jest włączony.
    turbo-drop: 'false'
  
    #Czy "turbo experience" jest włączone.
    turbo-experience: 'false'
  
    #Ilość kulek doświadczenia, jakie dostajemy podczas wykopania kamienia.
    experience: '1'
#Ustawienia generatora kamienia.
  generator:
    #Czy włączyć generator kamienia
    enable: 'true'
  
    #Co ile ticków regeneruje się kamień
    #1 tick = 1/20 sekundy
    #2 ticki = 2/20 sekundy lub 1/10 sekundy
    regeneration-time: '10'
  
    #Konfiguracja tworzenia.
    # SLOT1 | SLOT2 | SLOT3
    # SLOT4 | SLOT5 | SLOT6
    # SLOT7 | SLOT8 | SLOT9
    crafting:
      #Okienko nr. 1
      slot1:
        #Ilość przedmiotu
        amount: '1'
    
        #Przedmiot
        item: 'stone'
      slot2:
        amount: '1'
        item: 'stone'
      slot3:
        amount: '1'
        item: 'stone'
      slot4:
        amount: '1'
        item: 'stone'
      slot5:
        amount: '1'
        item: 'stone'
      slot6:
        amount: '1'
        item: 'stone'
      slot7:
        amount: '1'
        item: 'stone'
      slot8:
        amount: '1'
        item: 'stone'
      slot9:
        amount: '1'
        item: 'stone'
      #Liczba przedmiotów, jakie wyjdą po wytworzeniu.
      result-number: '1'
