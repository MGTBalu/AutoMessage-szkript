# AutoMessage Szkript - Készítette: MGTBalu

options:
  message1: &7Tudtad? A szerver tulajdonosai &cMGTBalu &7és &cTryjinn!
  message2: &7Használd a &e/kulcsok &7parancsot hogy kulcsokat vásárolhass!
  message3: &7Ládakulcsokat, rangokat szeretnél vásárolni? &c/webshop
  message4: &7Csalót találtál? Jelentsd őket a &4/report &7paranccsal!
  message5: &7Tudtad? A szerveren megtalálható a lottó! &a/lottery help
  message6: &7Jelenleg a &6&lSky&e&lRealm &7szerveren játszol!
  message7: &7Használd a &b/rangok &7parancsot hogy rangokat vásárolhass!
  message8: &7Hibát találtál? Jelentsd discord szerverünkön! &3/discord
  message9: &7Tudtad? A párbaj elérhető a szerveren! &9/duel
  separator: &8&m-----------------------------------------------------

every 2 minutes:
  set {_random} to random integer between 1 and 9
  
  if {_random} is 1:
    set {_message} to "{@message1}"
  else if {_random} is 2:
    set {_message} to "{@message2}"
  else if {_random} is 3:
    set {_message} to "{@message3}"
  else if {_random} is 4:
    set {_message} to "{@message4}"
  else if {_random} is 5:
    set {_message} to "{@message5}"
  else if {_random} is 6:
    set {_message} to "{@message6}"
  else if {_random} is 7:
    set {_message} to "{@message7}"
  else if {_random} is 8:
    set {_message} to "{@message8}"
  else if {_random} is 9:
    set {_message} to "{@message9}"
    
  broadcast "{@separator}"
  broadcast "%{_message}%"
  broadcast "{@separator}"
