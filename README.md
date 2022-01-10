---
description: From the original Knowledgebase
---

# Collection of Premade Circuits

**NTNET SCANNER FOR YOUR DOOR NTNET NEEDS**\
****By Letter N

```
{"assembly":{"type":"type-d electronic assembly","name":"NTNET SCANNER"},"components":[{"type":"tesla power relay"},{"type":"NTNet scanner"},{"type":"text-to-speech circuit","inputs":[[1,0,"105"]]},{"type":"ranged sensor"}],"wires":[[[2,"I",1],[4,"O",1]],[[2,"O",1],[3,"I",1]],[[2,"A",1],[4,"A",1]],[[2,"A",2],[3,"A",1]]]}
```

**Generic Follower Bot**\
****By Letter N

Features:

* You only have to type the person/thing to follow
* A ticker switch to turn it off
* 3 locomotive circuits with .1 second delay each, so it can run faster

```
{"assembly":{"type":"type-a electronic drone","name":"Generic FollowerBot","opened":1},"components":[{"type":"large tesla power relay"},{"type":"toggle button","name":"Ticker"},{"type":"fast ticker","name":"Main Ticker"},{"type":"one-sec delay circuit","name":"Overclocker"},{"type":"basic pathfinder"},{"type":"locomotion circuit","inputs":[[1,0,4]]},{"type":"tenth-sec delay circuit"},{"type":"locomotion circuit","inputs":[[1,0,4]]},{"type":"tenth-sec delay circuit"},{"type":"locomotion circuit","inputs":[[1,0,4]]},{"type":"advanced locator","inputs":[[2,0,5]]},{"type":"text pad","name":"Target Here"},{"type":"screen"},{"type":"concatenator","inputs":[[1,0,"Target: "]]}],"wires":[[[2,"O",1],[3,"I",1]],[[3,"A",1],[4,"A",1]],[[3,"A",1],[5,"A",1]],[[3,"A",1],[11,"A",1]],[[4,"A",2],[5,"A",1]],[[4,"A",2],[11,"A",1]],[[5,"I",1],[11,"O",1]],[[5,"O",1],[6,"I",1]],[[5,"O",1],[8,"I",1]],[[5,"O",1],[10,"I",1]],[[5,"A",2],[6,"A",1]],[[6,"A",2],[7,"A",1]],[[7,"A",2],[8,"A",1]],[[8,"A",2],[9,"A",1]],[[9,"A",2],[10,"A",1]],[[11,"I",1],[12,"O",1]],[[12,"O",1],[14,"I",2]],[[12,"A",1],[14,"A",1]],[[13,"I",1],[14,"O",1]],[[13,"A",1],[14,"A",2]]]}
```

**Generic Infinite Power**\
****By Letter N

Features:

* Screen to tell what is it pointing
* custom delay (recommended is 3)(tickers in seconds)
* fast (TM)charging

```
{"assembly":{"type":"electronic machine","name":"Infinite Power MK2","opened":1},"components":[{"type":"toggle button","name":"Light Switch"},{"type":"light","name":"Light"},{"type":"ranged sensor","name":"Pointy Sensor"},{"type":"large power transmission circuit","name":"Power Relay"},{"type":"large power transmission circuit","name":"Power Relay"},{"type":"slow ticker","name":"Ticker","inputs":[[1,0,1]]},{"type":"custom delay circuit","name":"Anti Overclocking Clock"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"tiny photovoltaic cell"},{"type":"reference to string"},{"type":"screen"}],"wires":[[[1,"A",1],[2,"A",1]],[[3,"O",1],[4,"I",1]],[[3,"O",1],[5,"I",1]],[[3,"O",1],[31,"I",1]],[[3,"A",1],[31,"A",1]],[[4,"A",1],[7,"A",2]],[[4,"A",2],[5,"A",1]],[[6,"A",1],[7,"A",1]],[[31,"O",1],[32,"I",1]],[[31,"A",2],[32,"A",1]]]}
```

**Door Remotes**\
****By Letter N\
\
Features:

* door remote that the heads start with that can open/close/bolt/emergency doors they have access to from a distance
* you scan your ID into it to set the access

```
{"assembly":{"type":"type-a electronic assembly","name":"Generic Door Remote MK 7","opened":1},"components":[{"type":"tesla power relay"},{"type":"ranged sensor"},{"type":"NTNet scanner"},{"type":"NTNet networking circuit","inputs":[[1,0,"337"],[2,0,"emergency"],[3,0,""],[4,0,"32405a434c415640595e5a4a48574947484d42415a2b"]]},{"type":"card reader"},{"type":"four multiplexer","inputs":[[1,0,3],[2,0,"open"],[3,0,"bolt"],[4,0,"emergency"],[5,0,"if you are seeing this, this is broken"]]},{"type":"memory chip","name":"MODE 1 To 3","inputs":[[1,0,0]]},{"type":"addition circuit","name":"MODE + 1","inputs":[[1,0,3],[2,0,1]]},{"type":"greater_than or equal gate","name":"More Than 4","inputs":[[1,0,4],[2,0,4]]},{"type":"memory chip","name":"Buffer","inputs":[[1,0,4]]},{"type":"memory chip","name":"Return 0","inputs":[[1,0,0]]},{"type":"screen","inputs":[[1,0,"emergency"]]},{"type":"button"}],"wires":[[[2,"O",1],[3,"I",1]],[[2,"A",1],[3,"A",1]],[[3,"O",1],[4,"I",1]],[[3,"A",2],[4,"A",1]],[[4,"I",2],[6,"O",1]],[[4,"I",4],[5,"O",3]],[[6,"I",1],[7,"O",1]],[[6,"O",1],[12,"I",1]],[[6,"A",1],[7,"A",2]],[[6,"A",2],[12,"A",1]],[[7,"I",1],[11,"O",1]],[[7,"I",1],[10,"O",1]],[[7,"O",1],[8,"I",1]],[[7,"A",1],[13,"A",1]],[[7,"A",2],[8,"A",1]],[[8,"O",1],[9,"I",1]],[[8,"O",1],[10,"I",1]],[[8,"A",2],[9,"A",1]],[[9,"A",2],[11,"A",1]],[[9,"A",3],[10,"A",1]]]}
```

**Advanced Medical Scanner**\
****By roushguy

```
{"assembly":{"type":"type-c electronic assembly","name":"RoushTek Health AnaLight","detail_color":"#5D99BE"},"components":[{"type":"sensor"},{"type":"tiny photovoltaic cell"},{"type":"button"},{"type":"integrated adv. medical analyser"},{"type":"advanced light","inputs":[[1,0,"#FFFFFF"],[2,0,10]]},{"type":"number to string","name":"Health","inputs":[[1,0,94]]},{"type":"number to string","name":"Missing","inputs":[[1,0,6]]},{"type":"number to string","name":"Brute","inputs":[[1,0,6]]},{"type":"number to string","name":"Burn","inputs":[[1,0,0]]},{"type":"number to string","name":"Tox","inputs":[[1,0,0]]},{"type":"number to string","name":"Oxy","inputs":[[1,0,0]]},{"type":"number to string","name":"Clone","inputs":[[1,0,0]]},{"type":"concatenator","inputs":[[1,0,"Total Health: "],[2,0,"94"],[3,0," Total Damage: "],[4,0,"6"],[5,0," Brute Damage: "],[6,0,"6"],[7,0," Burn Damage: "],[8,0,"0"]]},{"type":"concatenator","inputs":[[1,0,"Total Health: 94 Total Damage: 6 Brute Damage: 6 Burn Damage: 0"],[2,0," Toxin Damage:"],[3,0,"0"],[4,0," Oxygen Damage: "],[5,0,"0"],[6,0," Clone Damage: "],[7,0,"0"]]},{"type":"text-to-speech circuit","inputs":[[1,0,"Total Health: 94 Total Damage: 6 Brute Damage: 6 Burn Damage: 0 Toxin Damage:0 Oxygen Damage: 0 Clone Damage: 0"]]}],"wires":[[[1,"O",1],[4,"I",1]],[[1,"A",1],[4,"A",1]],[[3,"A",1],[5,"A",1]],[[4,"O",1],[6,"I",1]],[[4,"O",2],[7,"I",1]],[[4,"O",3],[8,"I",1]],[[4,"O",4],[9,"I",1]],[[4,"O",5],[10,"I",1]],[[4,"O",6],[11,"I",1]],[[4,"O",7],[12,"I",1]],[[4,"A",2],[6,"A",1]],[[4,"A",2],[7,"A",1]],[[4,"A",2],[8,"A",1]],[[4,"A",2],[9,"A",1]],[[4,"A",2],[10,"A",1]],[[4,"A",2],[11,"A",1]],[[4,"A",2],[12,"A",1]],[[6,"O",1],[13,"I",2]],[[7,"O",1],[13,"I",4]],[[8,"O",1],[13,"I",6]],[[9,"O",1],[13,"I",8]],[[10,"O",1],[14,"I",3]],[[11,"O",1],[14,"I",5]],[[12,"O",1],[14,"I",7]],[[12,"A",2],[13,"A",1]],[[13,"O",1],[14,"I",1]],[[13,"A",2],[14,"A",1]],[[14,"O",1],[15,"I",1]],[[14,"A",2],[15,"A",1]]]}
```

**Pointer Agent ID**\
****By PKPenguin321

Features:

* Swipe as many IDs as you want. Turn it on or off with the toggle button.
* While on, point at a door. It will use all swiped IDs on the door, attempting to open it.

```
{"assembly":{"type":"type-f electronic assembly","name":"Pointer ID","opened":1,"detail_color":"#CC4242"},"components":[{"type":"card reader"},{"type":"append circuit","inputs":[[1,0,[]]]},{"type":"memory chip","name":"MSG Scanned","inputs":[[1,0,"New ID added."]]},{"type":"screen","inputs":[[1,0,"New ID added."]]},{"type":"advanced locator","inputs":[[1,0,"pointer"],[2,0,8]]},{"type":"toggle button","name":"Toggle Point Detector"},{"type":"custom ticker","inputs":[[1,0,1],[2,0,1.5]]},{"type":"examiner"},{"type":"global positioning system"},{"type":"addition circuit","name":"X Abs Getter","inputs":[[1,0,180],[2,0,0]]},{"type":"addition circuit","name":"Y Abs Getter","inputs":[[1,0,119],[2,0,7]]},{"type":"Tile pointer","inputs":[[1,0,180],[2,0,126]]},{"type":"tile analyzer"},{"type":"at circuit","inputs":[[1,0,["Research Division Access","the proximity checker","the pointer"]]]},{"type":"NTNet scanner"},{"type":"delete circuit","inputs":[[1,0,["/datum/weakref","/datum/weakref","/datum/weakref"]]]},{"type":"tenth-sec delay circuit"},{"type":"NTNet networking circuit","inputs":[[2,0,"open"]]},{"type":"list set circuit","inputs":[[1,0,[]]]},{"type":"at circuit","inputs":[[1,0,[]]]},{"type":"addition circuit","inputs":[[1,0,1],[2,0,1]]},{"type":"memory chip","name":"MEM 1","inputs":[[1,0,1]]},{"type":"tenth-sec delay circuit"},{"type":"tesla power relay"}],"wires":[[[1,"O",3],[2,"I",2]],[[1,"A",1],[2,"A",1]],[[1,"A",1],[3,"A",1]],[[2,"I",1],[19,"O",1]],[[2,"O",1],[19,"I",1]],[[2,"A",2],[19,"A",1]],[[3,"O",1],[4,"I",1]],[[3,"A",2],[4,"A",1]],[[5,"O",1],[8,"I",1]],[[5,"A",1],[7,"A",1]],[[5,"A",2],[8,"A",1]],[[6,"O",1],[7,"I",1]],[[8,"O",3],[10,"I",2]],[[8,"O",4],[11,"I",2]],[[8,"A",2],[9,"A",1]],[[9,"O",1],[10,"I",1]],[[9,"O",2],[11,"I",1]],[[9,"A",2],[11,"A",1]],[[9,"A",2],[10,"A",1]],[[9,"A",2],[12,"A",1]],[[10,"O",1],[12,"I",1]],[[11,"O",1],[12,"I",2]],[[12,"O",1],[13,"I",1]],[[12,"A",2],[13,"A",1]],[[13,"O",1],[14,"I",1]],[[13,"O",1],[16,"I",1]],[[13,"A",2],[14,"A",1]],[[14,"I",1],[16,"O",1]],[[14,"O",1],[15,"I",1]],[[14,"A",1],[17,"A",2]],[[14,"A",2],[15,"A",1]],[[15,"O",1],[18,"I",1]],[[15,"A",2],[20,"A",1]],[[15,"A",3],[16,"A",1]],[[16,"I",1],[16,"O",1]],[[16,"A",2],[17,"A",1]],[[18,"I",4],[20,"O",1]],[[18,"A",1],[20,"A",2]],[[19,"O",1],[20,"I",1]],[[20,"I",2],[22,"O",1]],[[20,"I",2],[21,"O",1]],[[20,"A",1],[23,"A",2]],[[20,"A",2],[21,"A",1]],[[20,"A",3],[22,"A",1]],[[21,"I",1],[22,"O",1]],[[21,"I",1],[21,"O",1]],[[21,"A",2],[23,"A",1]]]}
```

**Shard Thrower**\
****By Deleted 7esla\
(Probably nerfed)

```
{"assembly":{"type":"type-d electronic machine","opened":1},"components":[{"type":"adjacent locator","name":"Adj Loc A"},{"type":"adjacent locator","name":"Adj Loc B"},{"type":"examiner"},{"type":"ranged sensor"},{"type":"custom ticker","inputs":[[1,0,1],[2,0,0.001]]},{"type":"grabber","name":"Grabber A","inputs":[[2,0,1]]},{"type":"grabber","name":"Grabber B","inputs":[[2,0,1]]},{"type":"list deconstructor","name":"List D A","inputs":[[1,0,["the shard"]]]},{"type":"list deconstructor","name":"List D B","inputs":[[1,0,["the shard","the shard","the shard"]]]},{"type":"large tesla power relay","name":"Power Tesla"},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"thrower","inputs":[[1,0,0],[2,0,-2]]},{"type":"tenth-sec delay circuit"},{"type":"tenth-sec delay circuit"},{"type":"tenth-sec delay circuit"},{"type":"tenth-sec delay circuit"},{"type":"tenth-sec delay circuit"},{"type":"tenth-sec delay circuit"},{"type":"tenth-sec delay circuit"}],"wires":[[[1,"O",1],[6,"I",1]],[[1,"A",1],[5,"A",1]],[[1,"A",2],[6,"A",1]],[[2,"O",1],[7,"I",1]],[[2,"A",1],[5,"A",1]],[[2,"A",2],[7,"A",1]],[[3,"I",1],[4,"O",1]],[[3,"O",3],[11,"I",1]],[[3,"O",3],[12,"I",1]],[[3,"O",3],[13,"I",1]],[[3,"O",3],[14,"I",1]],[[3,"O",3],[15,"I",1]],[[3,"O",3],[16,"I",1]],[[3,"O",3],[17,"I",1]],[[3,"O",3],[18,"I",1]],[[3,"O",4],[11,"I",2]],[[3,"O",4],[12,"I",2]],[[3,"O",4],[13,"I",2]],[[3,"O",4],[14,"I",2]],[[3,"O",4],[15,"I",2]],[[3,"O",4],[16,"I",2]],[[3,"O",4],[17,"I",2]],[[3,"O",4],[18,"I",2]],[[3,"A",1],[4,"A",1]],[[3,"A",2],[11,"A",1]],[[3,"A",2],[19,"A",1]],[[5,"A",1],[6,"A",2]],[[5,"A",1],[7,"A",2]],[[5,"A",1],[8,"A",2]],[[5,"A",1],[9,"A",2]],[[6,"O",4],[8,"I",1]],[[6,"A",2],[8,"A",1]],[[7,"O",4],[9,"I",1]],[[7,"A",2],[9,"A",1]],[[8,"O",1],[11,"I",3]],[[8,"O",2],[12,"I",3]],[[8,"O",3],[13,"I",3]],[[8,"O",4],[14,"I",3]],[[9,"O",1],[15,"I",3]],[[9,"O",2],[16,"I",3]],[[9,"O",3],[17,"I",3]],[[9,"O",4],[18,"I",3]],[[12,"A",1],[19,"A",2]],[[13,"A",1],[20,"A",2]],[[14,"A",1],[21,"A",2]],[[15,"A",1],[22,"A",2]],[[16,"A",1],[23,"A",2]],[[17,"A",1],[24,"A",2]],[[18,"A",1],[25,"A",2]],[[19,"A",2],[20,"A",1]],[[20,"A",2],[21,"A",1]],[[21,"A",2],[22,"A",1]],[[22,"A",2],[23,"A",1]],[[23,"A",2],[24,"A",1]],[[24,"A",2],[25,"A",1]]]}
```

**Signaler String Sending System**\
****By PKPenguin321\
\
Features:

* Set the sender and reciever to the same frequency. Frequency should be usually 4 numbers.
* Allows sending of arbitrary strings without using NTNet, which should hypothetically work anywhere even without telecomms.
* Only downside is that the longer your string, the longer it takes to send.

Sender:

```
{"assembly":{"type":"type-b electronic assembly","name":"Signaler String Sender","detail_color":"#E39751"},"components":[{"type":"tesla power relay"},{"type":"lowercase string converter","inputs":[[1,0,"How are you doing?"]]},{"type":"memory chip","name":"MEM Greater 1","inputs":[[1,0,1]]},{"type":"addition circuit","name":"Greater Addition","inputs":[[1,0,1],[2,0,1]]},{"type":"string exploder","inputs":[[1,0,"how are you doing?"]]},{"type":"at circuit","inputs":[[1,0,["h","o","w"," ","a","r","e"," ","y","o","u"," ","d","o","i","n","g","?"]]]},{"type":"search circuit","name":"TABLE1 - Char2Index","inputs":[[1,0,[" ","0","1","2","3","4","5","6","7","8","9","a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z",",",".","!","?","'",":","#"]]]},{"type":"memory chip","name":"MEM Bad Char Index","inputs":[[1,0,44]]},{"type":"at circuit","name":"TABLE2 - Index2Code","inputs":[[1,0,["111","112","113","114","121","122","123","124","131","132","133","134","141","142","143","144","211","212","213","214","221","222","223","224","231","232","233","234","241","242","243","244","311","312","313","314","321","322","323","324","331","332","333","334"]],[2,0,41]]},{"type":"string exploder","inputs":[[1,0,"444"]]},{"type":"at circuit","inputs":[[1,0,["4","4","4"]]]},{"type":"string to number"},{"type":"integrated signaler","inputs":[[1,0,1337],[2,0,4]]},{"type":"half-sec delay circuit"},{"type":"addition circuit","name":"Lesser Addition","inputs":[[1,0,1],[2,0,1]]},{"type":"equal gate"},{"type":"memory chip","name":"MEM 1","inputs":[[1,0,1]]},{"type":"memory chip","name":"MEM STOPchar Code","inputs":[[1,0,"444"]]},{"type":"equal gate","name":"IF STOPchar Sent","inputs":[[1,0,"444"],[2,0,"444"]]},{"type":"text pad","name":"Text To Send"},{"type":"number pad","name":"Set Frequency"},{"type":"tenth-sec delay circuit"}],"wires":[[[2,"I",1],[20,"O",1]],[[2,"O",1],[5,"I",1]],[[2,"A",1],[20,"A",1]],[[2,"A",2],[5,"A",1]],[[3,"O",1],[4,"I",1]],[[3,"O",1],[6,"I",2]],[[3,"A",1],[6,"A",3]],[[4,"I",1],[4,"O",1]],[[4,"O",1],[6,"I",2]],[[4,"A",1],[19,"A",3]],[[4,"A",2],[6,"A",1]],[[5,"O",1],[6,"I",1]],[[5,"A",2],[6,"A",1]],[[6,"O",1],[7,"I",2]],[[6,"A",2],[7,"A",1]],[[6,"A",3],[18,"A",1]],[[7,"O",1],[9,"I",2]],[[7,"A",2],[9,"A",1]],[[7,"A",3],[8,"A",1]],[[8,"O",1],[9,"I",2]],[[8,"A",2],[9,"A",1]],[[9,"O",1],[10,"I",1]],[[9,"O",1],[19,"I",2]],[[9,"A",2],[22,"A",1]],[[10,"I",1],[18,"O",1]],[[10,"O",1],[11,"I",1]],[[10,"A",1],[22,"A",2]],[[10,"A",2],[11,"A",1]],[[11,"I",2],[17,"O",1]],[[11,"I",2],[15,"O",1]],[[11,"O",1],[12,"I",1]],[[11,"A",1],[15,"A",2]],[[11,"A",2],[12,"A",1]],[[11,"A",3],[17,"A",1]],[[11,"A",3],[19,"A",1]],[[12,"O",1],[13,"I",2]],[[12,"A",2],[13,"A",1]],[[13,"I",1],[21,"O",1]],[[13,"A",2],[14,"A",1]],[[14,"A",2],[15,"A",1]],[[15,"I",1],[15,"O",1]],[[15,"I",1],[17,"O",1]],[[18,"O",1],[19,"I",2]],[[18,"A",2],[22,"A",1]]]}
```

Receiver:

```
{"assembly":{"type":"type-b electronic assembly","name":"Signaler String Reciever","detail_color":"#E39751"},"components":[{"type":"tesla power relay"},{"type":"search circuit","name":"TABLE1 - Code2Index","inputs":[[1,0,["111","112","113","114","121","122","123","124","131","132","133","134","141","142","143","144","211","212","213","214","221","222","223","224","231","232","233","234","241","242","243","244","311","312","313","314","321","322","323","324","331","332","333","334"]],[2,0,"331"]]},{"type":"at circuit","name":"TABLE2 - Index2Char","inputs":[[1,0,[" ","0","1","2","3","4","5","6","7","8","9","a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z",",",".","!","?","'",":","#"]],[2,0,41]]},{"type":"integrated signaler","name":"Signaler 1","inputs":[[1,0,1337],[2,0,1]]},{"type":"integrated signaler","name":"Signaler 2","inputs":[[1,0,1337],[2,0,2]]},{"type":"integrated signaler","name":"Signaler 3","inputs":[[1,0,1337],[2,0,3]]},{"type":"integrated signaler","name":"Signaler 4","inputs":[[1,0,1337],[2,0,4]]},{"type":"number pad","name":"Set Frequency"},{"type":"memory chip","name":"MEM One","inputs":[[1,0,"1"]]},{"type":"memory chip","name":"MEM Two","inputs":[[1,0,"2"]]},{"type":"memory chip","name":"MEM Three","inputs":[[1,0,"3"]]},{"type":"memory chip","name":"MEM Four","inputs":[[1,0,"4"]]},{"type":"small concatenator"},{"type":"get length","inputs":[[1,0,"444"]]},{"type":"equal gate","name":"IF CodeLength Is 3","inputs":[[1,0,3],[2,0,3]]},{"type":"equal gate","name":"IF STOPchar Recieved","inputs":[[1,0,"444"],[2,0,"444"]]},{"type":"small memory circuit","name":"MEM String Setter","inputs":[[1,0,"444"]]},{"type":"small concatenator"},{"type":"large screen","inputs":[[1,0,"how are you doing?"]]},{"type":"memory chip","name":"MEM Null"}],"wires":[[[2,"I",2],[17,"O",1]],[[2,"O",1],[3,"I",2]],[[2,"A",1],[17,"A",2]],[[2,"A",2],[3,"A",1]],[[3,"O",1],[18,"I",2]],[[3,"A",2],[18,"A",1]],[[4,"I",1],[8,"O",1]],[[4,"A",3],[9,"A",1]],[[5,"I",1],[8,"O",1]],[[5,"A",3],[10,"A",1]],[[6,"I",1],[8,"O",1]],[[6,"A",3],[11,"A",1]],[[7,"I",1],[8,"O",1]],[[7,"A",3],[12,"A",1]],[[9,"O",1],[13,"I",2]],[[9,"A",2],[13,"A",1]],[[10,"O",1],[13,"I",2]],[[10,"A",2],[13,"A",1]],[[11,"O",1],[13,"I",2]],[[11,"A",2],[13,"A",1]],[[12,"O",1],[13,"I",2]],[[12,"A",2],[13,"A",1]],[[13,"I",1],[13,"O",1]],[[13,"I",1],[17,"O",2]],[[13,"I",1],[20,"O",1]],[[13,"I",2],[17,"O",2]],[[13,"I",2],[20,"O",1]],[[13,"O",1],[14,"I",1]],[[13,"O",1],[17,"I",1]],[[13,"O",1],[16,"I",1]],[[13,"A",2],[14,"A",1]],[[14,"O",1],[15,"I",1]],[[14,"A",2],[15,"A",1]],[[15,"A",2],[16,"A",1]],[[16,"A",2],[19,"A",1]],[[16,"A",2],[20,"A",1]],[[16,"A",3],[17,"A",1]],[[18,"I",1],[18,"O",1]],[[18,"I",1],[20,"O",1]],[[18,"I",2],[20,"O",1]],[[18,"O",1],[19,"I",1]]]}
```

**No Name - Remove Blood From Patient**\
****By Asd\
\
Features:

* This will remove 20-30% of your patients blood over \~15 seconds and vaporize it all

```
{"assembly":{"type":"type-a electronic mechanism","opened":1},"components":[{"type":"sensor"},{"type":"integrated hypo-injector","inputs":[[2,0,-30]]},{"type":"reagent pump"},{"type":"smoke generator"},{"type":"custom delay circuit","inputs":[[1,0,60]]},{"type":"screen","inputs":[[1,0,"Ready!"]]},{"type":"integrated hypo-injector","inputs":[[2,0,-30]]},{"type":"integrated hypo-injector","inputs":[[2,0,-30]]},{"type":"integrated hypo-injector","inputs":[[2,0,-30]]},{"type":"wire node"},{"type":"starter"}],"wires":[[[3,"A",2],[4,"A",1]],[[3,"I",2],[4,"O",2]],[[3,"I",1],[7,"O",2]],[[3,"I",3],[7,"O",1]],[[3,"I",1],[8,"O",2]],[[3,"I",1],[9,"O",2]],[[3,"I",3],[9,"O",1]],[[1,"A",1],[2,"A",1]],[[9,"A",2],[10,"A",1]],[[2,"O",2],[3,"I",1]],[[2,"O",1],[3,"I",3]],[[3,"I",3],[8,"O",1]],[[2,"A",2],[10,"A",1]],[[2,"A",2],[7,"A",1]],[[7,"A",2],[10,"A",1]],[[7,"A",2],[8,"A",1]],[[8,"A",2],[10,"A",1]],[[3,"A",1],[10,"A",2]],[[8,"A",2],[9,"A",1]],[[5,"A",2],[6,"A",1]],[[1,"O",1],[2,"I",1]],[[1,"O",1],[7,"I",1]],[[1,"O",1],[8,"I",1]],[[1,"O",1],[9,"I",1]],[[4,"A",3],[11,"A",1]],[[5,"A",1],[11,"A",1]],[[2,"A",4],[11,"A",1]],[[7,"A",4],[11,"A",1]],[[8,"A",4],[11,"A",1]],[[9,"A",4],[11,"A",1]]]}
```
