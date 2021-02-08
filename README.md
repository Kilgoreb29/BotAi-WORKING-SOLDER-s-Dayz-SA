# BotAi-WORKING-SOLDER-s-Dayz-SA

Copy @BotClientSide and @BotServerSide to your server
Copy Mission dayzOffline.chernarusplus in Missions
drop key

change Startoptions
"-mod= @BotClientSide;" "-servermod=@BotServerSide;"

Bot´s spawn as Mission....no manuel spawn!!!
you find coordinates in BOTFOLDER
also some config´s

vector BotSpawnPoint = "4541.687500 317.593628 8324.727539";

protected int m_botAcuracy = 10;
protected int BotSolderCountMin = 2;
protected int BotSolderCountMax = 4;
protected int botLootCountMin = 5;
protected int botLootCountMax = 15;
protected float Zone_Radius = 150;
protected bool isUseCheckPoints = false;
protected bool isBotKaratist = false;

akso

m_BotSolder.SetUseCheckpoint(); //

m_BotSolder.AddCheckpoint("1724.632080 451.730408 14298.412109");
m_BotSolder.AddCheckpoint("1681.035522 451.784302 14278.791016");
m_BotSolder.AddCheckpoint("1668.385742 451.730408 14268.739258");
m_BotSolder.AddCheckpoint("1653.012695 451.784302 14245.443359");
m_BotSolder.AddCheckpoint("1662.009521 451.784302 14220.044922");
m_BotSolder.AddCheckpoint("1668.885010 451.730408 14177.100586");
m_BotSolder.AddCheckpoint("1678.905029 451.784302 14134.460938");
m_BotSolder.AddCheckpoint("1687.656250 451.784302 14097.293945");
m_BotSolder.AddCheckpoint("1691.055054 451.728760 14072.710938");
m_BotSolder.AddCheckpoint("1697.563721 450.094635 14019.088867");
m_BotSolder.AddCheckpoint("1701.266235 448.636108 13981.079102");
m_BotSolder.AddCheckpoint("1709.151733 448.368225 13969.950195");
m_BotSolder.AddCheckpoint("1726.191772 447.882568 13954.740234");
m_BotSolder.AddCheckpoint("1734.303101 447.342072 13945.562500");
m_BotSolder.AddCheckpoint("1736.849487 447.158569 13939.061523");
m_BotSolder.AddCheckpoint("1803.257568 436.318970 13812.399414");
m_BotSolder.AddCheckpoint("1802.478149 435.682281 13794.238281");
m_BotSolder.AddCheckpoint("1764.742676 434.271759 13667.715820");
m_BotSolder.AddCheckpoint("1753.983521 434.111572 13660.847656");
m_BotSolder.AddCheckpoint("1697.765381 433.031982 13621.431641");
m_BotSolder.AddCheckpoint("1625.751953 437.192169 13583.775391");
m_BotSolder.AddCheckpoint("1615.443726 437.193420 13582.367188");
m_BotSolder.AddCheckpoint("1586.155762 439.010864 13609.286133");
m_BotSolder.AddCheckpoint("1566.816040 441.081787 13643.261719");
m_BotSolder.AddCheckpoint("1554.550049 441.587372 13645.919922");
m_BotSolder.AddCheckpoint("1533.254028 440.683624 13646.856445");
m_BotSolder.AddCheckpoint("1470.583130 444.685120 13679.353516");
m_BotSolder.AddCheckpoint("1448.422729 446.229736 13681.502930");
m_BotSolder.AddCheckpoint("1397.534424 448.255707 13663.409180");
m_BotSolder.AddCheckpoint("1377.747681 448.799530 13661.333984");
m_BotSolder.AddCheckpoint("1356.402222 451.658264 13669.961914");
m_BotSolder.AddCheckpoint("1339.632813 454.855988 13690.362305");
m_BotSolder.AddCheckpoint("1311.232178 457.548615 13730.733398");
m_BotSolder.AddCheckpoint("1368.332275 455.560181 13762.721680");
m_BotSolder.AddCheckpoint("1389.098022 453.795563 13785.572266");
m_BotSolder.AddCheckpoint("1394.411499 451.237183 13801.572266");
m_BotSolder.AddCheckpoint("1398.934204 451.644989 13828.162109");
m_BotSolder.AddCheckpoint("1419.962524 456.061951 13891.482422");
m_BotSolder.AddCheckpoint("1409.579224 458.430359 13947.408203");
m_BotSolder.AddCheckpoint("1421.006104 459.254517 13993.981445");
m_BotSolder.AddCheckpoint("1422.121094 459.807831 14022.114258");
m_BotSolder.AddCheckpoint("1388.509277 462.222443 14044.217773");
m_BotSolder.AddCheckpoint("1388.548340 462.354797 14044.183594");
m_BotSolder.AddCheckpoint("1333.772217 463.948151 14062.096680");
m_BotSolder.AddCheckpoint("1350.346069 465.658081 14107.701172");
m_BotSolder.AddCheckpoint("1461.509521 459.874268 14133.793945");
m_BotSolder.AddCheckpoint("1503.123291 455.995056 14137.425781");
m_BotSolder.AddCheckpoint("1554.196045 452.867004 14107.243164");
m_BotSolder.AddCheckpoint("1574.911743 452.540283 14100.198242");
m_BotSolder.AddCheckpoint("1629.664673 451.792175 14197.793945");
m_BotSolder.AddCheckpoint("1636.238647 451.792175 14221.260742");
m_BotSolder.AddCheckpoint("1671.278564 451.792175 14275.020508");
m_BotSolder.AddCheckpoint("1645.910522 451.807617 14315.247070");
m_BotSolder.AddCheckpoint("1669.397339 451.792175 14331.668945");
m_BotSolder.AddCheckpoint("1685.370361 451.792175 14341.243164");

and Guns and Gear

void createWeapFromBot(SurvivorBotBase m_BotSolder)
{
int randomWeapon = Math.RandomInt(1, 7);

switch( randomWeapon )
{
case 1:
{
m_BotSolder.AddWeapon("M4A1");
m_BotSolder.AddWeaponAtt("M4_RISHndgrd");
m_BotSolder.AddWeaponAtt("M4_MPBttstck");
m_BotSolder.AddWeaponAtt("ACOGOptic");
break;

/

// Ìàññèâû ñ ëóòîì è îäåæäîé
// Åñëè êàêîéòî òèï íå íóæåí ïðîñòî îñòàâëÿåì ïóñòûå êîâû÷êè ïðèìåð ---> TStringArray OtherEquip = {""};
ref TStringArray Shirt = {"GorkaEJacket_Autumn", "GorkaEJacket_Flat", "GorkaEJacket_PautRev", "GorkaEJacket_Summer"};
ref TStringArray Jeans = {"GorkaPants_Autumn", "GorkaPants_Flat", "GorkaPants_PautRev", "GorkaPants_Summer"};
ref TStringArray Shoes = {"TTSKOBoots", "WorkingBoots_Beige", "CombatBoots_Beige", "CombatBoots_Black", "CombatBoots_Brown"};
ref TStringArray BackPack = {"CoyoteBag_Brown", "CoyoteBag_Green", "HuntingBag", "TortillaBag", "WaterproofBag_Green"};
ref TStringArray Vest = {"HighCapacityVest_Black", "HighCapacityVest_Olive", "HuntingVest", "PlateCarrierVest", "UKAssVest_Camo"};
ref TStringArray Helm = {"GorkaHelmet", "Mich2001Helmet", "MotoHelmet_Black", "PumpkinHelmet", "SkateHelmet_Black"};
ref TStringArray Gloves = {"WorkingGloves_Beige", "WorkingGloves_Black", "NBCGlovesGray", "OMNOGloves_Brown", "SurgicalGloves_Blue"};
ref TStringArray OtherEquip = {"CivilianBelt", "MilitaryBelt"};

ref TStringArray RandomLoot = {"SardinesCan", "SodaCan_Cola", "SodaCan_Kvass", "Rice", "Rope", "Screwdriver", "AmmoBox_545x39_20Rnd"}; //Äîáàâëÿåì â ìàñèâ ëþáîé ëóò, êîëè÷åñòâî íå îãðàíè÷åíî



<p align="center">
<img src="https://github.com/x1234xx/BotAi-WORKING-SOLDER-s-Dayz-SA/blob/main/20210208002114_1.jpg" ><br>
  
  <p align="center">
<img src="https://github.com/x1234xx/BotAi-WORKING-SOLDER-s-Dayz-SA/blob/main/20210208002124_1.jpg" ><br>
   
  <p align="center">
<img src="https://github.com/x1234xx/BotAi-WORKING-SOLDER-s-Dayz-SA/blob/main/20210208002653_1.jpg" ><br>
