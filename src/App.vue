<template>
    <div id="app">
        <!-- navigacija-->
        <div class="navigacija">
            <ul class="navi flex-row">
                <a href="index.html#o_nama_link"><li >O nama</li></a>
                <a href="index.html#kuce_za_odmor"><li >Kuće za odmor</li></a>
                <a href="index.html#ugostiteljski_objekt"><li >Ugostiteljski objekt</li></a>
                <a href="index.html#elektrane"><li >Elektrane</li></a>
                <a href="index.html#kontakt"><li >Kontakt</li></a>
                <a href="#"><li class="eng">eng</li></a>
            </ul>
        </div>
        <!--prvi section gdje se nalaze logo, o nama tekst i slider-->
        <div class="flex-row">
            <!-- div za logo i O nama tekst - poreda ih jedan ispod drugog-->
            <div class="o_nama">
                <!-- slika loga-->
                <div id="logo">
                    <img src="./assets/images/logo_vlastelini.svg" alt="Logo Vlastellini" class="logo-img">
                </div>
                <!-- O nama tekst -->     
                <div class="o_nama__box bg_orange m_t_m box_shadow_text" data-aos="flip-up" data-aos-delay="100" data-aos-duration="1000" data-aos-easing="ease-in-out" data-aos-anchor-placement="top-center" data-aos-once="true" data-aos-mirror="true">
                    <div id="o_nama_link" class="pd_tb_l">
                        <h1 class="m_b_xm">O nama</h1>
                        <p class="tekst_o_nama">Društvo Vlastelini d.o.o. osnovano je 2015. godine i u privatnom je vlasništvu. Danom osnutka društvo je preuzelo poslovanje nekadašnje tvrtke Hena d.o.o., a sadašnje glavne djelatnosti društva su pružanje turističkih usluga, poljoprivredne djelatnosti povezane s ugostiteljstvom i turizmom, upravljanje sunčanim elektranama te računovodstveni i knjigovodstveni poslovi.</p>
                    </div>
                </div>
            </div>
            <!-- SLIDER -->
            <div class="slider box_shadow_img">
                <template >
                    <!-- Hooper template koji sam koristio za slider -->
                    <hooper :settings="hooperSettings" class="slider_img"><!-- settings za slike se nalazi dolje u <script> -->
                        <slide class="slider_img">
                            <img src="./assets/images/slider/Rotacija1.jpg" alt="Villa Vlastellini" class="slider_img"/>
                        </slide>
                        <slide class="slider_img">
                            <img src="./assets/images/slider/Rotacija2.jpg" alt="Villa Vlastellini" class="slider_img"/>
                        </slide>
                        <slide class="slider_img">
                            <img src="./assets/images/slider/Rotacija3.jpg" alt="Villa Vlastellini" class="slider_img"/>
                        </slide>
                        <slide class="slider_img">
                            <img src="./assets/images/slider/Rotacija4.jpg" alt="Villa Vlastellini" class="slider_img"/>
                        </slide>
                        <slide class="slider_img">
                            <img src="./assets/images/slider/Rotacija6.jpg" alt="Villa Vlastellini" class="slider_img"/>
                        </slide>
                        <!-- strelica za lisatnje slika - koja ne radi - tj. nisam je mogao staviti u bijelu boju jer je vec automatski crna i mala -->
                        <!--<hooper-navigation slot="hooper-addons"></hooper-navigation>-->
                        <!-- navigacija na slideru -->
                        <hooper-pagination slot="hooper-addons"></hooper-pagination>
                    </hooper>
                </template>
            </div>
        </div>
        <!--Drugi section gdje se nalaze tri manja diva sa tekstom o uslugama i slikom iznad-->
        <div id="section_2" class="flex-row" data-aos-anchor-placement="top-top">
            <!-- data-aos sam koristio za animacije  -->
            <div class="usluge" data-aos="zoom-in" data-aos-delay="100" data-aos-duration="1000" data-aos-easing="ease-in-out" data-aos-once="true">
                <div class="usluge_slika_div">
                    <img src="./assets/images/icons/house.svg" alt="House Icon" class="usluge_slika">
                </div>
                <p>Turističke usluge koje društvo pruža obavljaju se u kvalitetno opremljenim smještajnim objektima -luksuznim vilama za odmor karakterističnim po svojoj lokaciji, autentičnosti, opremljenosti, sadržaju i komforu. Luksuzni objekti opremljeni su u skladu s najvišim tehnološkim standardima, uz poštovanje umjetnosti, prirode i ekoloških načela, kako bi gostima pružili oazu za potpuno opuštanje i uživanje.</p>
            </div>
            <!--data-aos-anchor-placement="bottom-bottom"-->
            <div class="usluge_paneli" 
                  data-aos="zoom-in" 
                  data-aos-delay="300"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <div class="usluge_slika_div">
                    <img src="./assets/images/icons/solarne.svg" alt="Solar panel" class="usluge_slika_paneli">
                </div>
                <p>Izgradnjom dviju sunčanih elektrana društvo je svoju djelatnost proširilo i na proizvodnju struje iz sunčane energije, želeći na taj način dati svoj doprinos očuvanju okoliša. Naime, sunčane elektrane nemaju štetnih proizvoda prilikom proizvodnje električne energije što ih čini potpuno prihvatljivim za okoliš, stoga se ta djelatnost u postpunosti uklopila u cilj društva.</p>
            </div>
            <div class="usluge"
                  data-aos="zoom-in" 
                  data-aos-delay="500"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true"> 
                <div class="usluge_slika_div">
                    <img src="./assets/images/icons/food.svg" alt="Food" class="usluge_slika">
                </div>
                <p>Društvo Vlastelini d.o.o. u svom vlasništvu ima i ugostiteljski objekt Velo Kafe, smješten u jednoj od najljepših zgrada na labinskom starogradskom trgu. Sastoji se od tri etaže, od kojih svaka ima svoju zasebnu funkciju, a zajedno pružaju cjelovitu ugostiteljsku uslugu.</p>
            </div>
        </div>
        <!-- Section 3 - Društvo Vlastellini d.o.o.  -->
        <div id="kuce_za_odmor" class="flex-row">
            <div data-aos="fade-right" data-aos-delay="100" data-aos-duration="1000" data-aos-easing="ease-in-out" data-aos-once="true">
                <img src="./assets/images/drustvo_vlastelini.png" alt="Društvo Vlastellini" class="slika_lijevo box_shadow_img" />
            </div>
            <div class="section_3 text_desno bg_orange box_shadow_text pd_tb_l m_b_l"
                      data-aos="fade-up"
                      data-aos-delay="100"
                      data-aos-duration="1000"
                      data-aos-easing="ease-in-out"
                      data-aos-once="true">
                <div class="section_3__content">
                    <h2 class="section_3__naslov m_b_xm">Društvo VLASTELLINI d.o.o.<br> danas ima ove bitne<br> sastavnice</h2>
                    <ol class="section_3__text">
                        <li>
                            Villa Vlastelini - Santo Spirito - kvalitetno opremljena luksuzna kuća za odmor smještena u blizini starogradske jezgre grada Labina.
                        </li>
                        <li>
                            Villa Vlastelini - Porto Longo - kvalitetno opremljena luksuzna kuća za odmor na samoj morskoj obali u mjestu Prtlog/Duga Luka 
                        </li>
                        <li>
                            Energo Sol Labin d.o.o., sunčana elektrana snage 480 kW
                        </li>
                        <li>
                            Sol Navitas Labin d.o.o., sunčana elektrana snage 180 kW
                        </li>
                        <li>
                            Velo Kafe - ugostiteljski objekt u Labinu
                        </li>
                    </ol>
                </div>
                
            </div>
            
        </div>
        <!-- Section 4 - Villa Vlastellini - Santo Spirito - slika i tekst sa animacijama -->
        <div class="flex-row section_4">
            <!-- Slika -->
            <div>
                <img src="./assets/images/villa_vlastelini_San_Spi.png" alt="Villa Vlastelini - Santo Spirito" class="slika_desno box_shadow_img"
                    data-aos="fade-up" 
                    data-aos-delay="100"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out"
                    data-aos-once="true" />
            </div>
            <!-- Tekst -->
            <div class="text_lijevo bg_orange box_shadow_text section_4__content pd_tb_l m_b_l" 
                  data-aos="fade-right" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <div class="section_4__content_text">
                    <h1>Villa Vlastelini</h1>
                    <h2 class="m_b_xm">-Santo Spirito</h2>
                    <p class="section_4__text m_b_xm">
                        Imanje je smješteno na gotovo 20 000 četvornih metara pomno uređenog okoliša, a sadrži gotovo sve prirodne blagodati ruralne Istre - mini farmu s domaćim životinjama, voćnjak i povrtnjak iz kojeg gosti mogu konzumirati ekološki uzgojene plodove, vanjski kamin s roštiljem te brojne rekreativne sadržaje poput teniskog terena, bazena, golf vježbališta i staze za trekking.
                    </p>
                    <!-- Karakteristike Ville - mala ikona i opis nalaze se ispod teksta o villi -->
                    <div class="section_4__usluge">
                        <div class="villa_usluge">
                            <img src="./assets/images/icons/plans.svg" alt="Plan ville" class="villa_icons">
                            <br>
                            <p class="villa_icons_text">Površina <br> Ville</p>
                            <p>265 m2</p>
                        </div>
                        <div class="villa_usluge">
                            <img src="./assets/images/icons/bed.svg" alt="Spavaća soba" class="villa_icons">
                            <br>
                            <p class="villa_icons_text">Spavaće <br> sobe</p>
                            <p>4</p>
                        </div>
                        <div class="villa_usluge">
                            <img src="./assets/images/icons/team2.svg" alt="Broj osoba" class="villa_icons">
                            <br>
                            <p class="villa_icons_text">Max. broj <br> osoba</p>
                            <p>8</p>
                        </div>
                        <div class="villa_usluge">
                            <img src="./assets/images/icons/bathtub.svg" alt="Broj kupaonica" class="villa_icons">
                            <br>
                            <p class="villa_icons_text">Broj <br> kupaonica</p>
                            <p>4</p>
                        </div>
                        <div class="villa_usluge">
                            <img src="./assets/images/icons/sea-waves.svg" alt="Udaljenost od mora" class="villa_icons">
                            <br>
                            <p class="villa_icons_text">Udaljenost <br> od mora</p>
                            <p>3.3 km</p>
                        </div>
                    </div>
                    <!-- Naračadsti button POGLEDAJ STRANICU -->
                    <a href="https://villa-vlastelini.com/santo-spirito/" target="_blank" title="pogledaj_stranicu">
                        <button class="btn_pogledaj_stranicu">
                            pogledaj stranicu
                        </button>
                    </a>
                </div>
            </div>
            
        </div>
        <!-- Section 5 - Villa Vlastellini - Porto Longo - slika i tekst sa animacijama -->
        <div class="flex-row sec_5">
            <!-- Slika -->
            <div>
                <img src="./assets/images/villa_vlastelini_Porto_longo.png" alt="Villa Vlastelini - Porto Longo" class="slika_lijevo box_shadow_img"
                  data-aos="fade-right" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
            </div>
            <!-- Tekst -->
            <div class="section_5__content text_desno bg_orange box_shadow_text pd_tb_l m_b_l"
                  data-aos="fade-up" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <h1 class="section_5__text">Villa Vlastelini</h1>
                <h2 class="section_5__text m_b_xm">-Porto Longo</h2>
                <p class="section_5__text m_b_xm">
                    Imanje je smješteno na gotovo 20 000 četvornih metara pomno uređenog okoliša, a sadrži gotovo sve prirodne blagodati ruralne Istre - mini farmu s domaćim životinjama, voćnjak i povrtnjak iz kojeg gosti mogu konzumirati ekološki uzgojene plodove, vanjski kamin s roštiljem te brojne rekreativne sadržaje poput teniskog terena, bazena, golf vježbališta i staze za trekking.
                </p>
                <!-- Karakteristike Ville - mala ikona i opis nalaze se ispod teksta o villi -->
                <div class="section_5__usluge">
                    <div class="villa_usluge">
                        <img src="./assets/images/icons/plans.svg" alt="Plan ville" class="villa_icons">
                        <br>
                        <p class="villa_icons_text">Površina <br> Ville</p>
                        <p>513 m2</p>
                    </div>
                    <div class="villa_usluge">
                        <img src="./assets/images/icons/bed.svg" alt="Spavaća soba" class="villa_icons">
                        <br>
                        <p class="villa_icons_text">Spavaće <br> sobe</p>
                        <p>5</p>
                    </div>
                    <div class="villa_usluge">
                        <img src="./assets/images/icons/team2.svg" alt="Broj osoba" class="villa_icons">
                        <br>
                        <p class="villa_icons_text">Max. broj <br> osoba</p>
                        <p>10</p>
                    </div>
                    <div class="villa_usluge">
                        <img src="./assets/images/icons/bathtub.svg" alt="Broj kupaonica" class="villa_icons">
                        <br>
                        <p class="villa_icons_text">Broj <br> kupaonica</p>
                        <p>5</p>
                    </div>
                    <div class="villa_usluge">
                        <img src="./assets/images/icons/sea-waves.svg" alt="Udaljenost od mora" class="villa_icons">
                        <br>
                        <p class="villa_icons_text">Udaljenost <br> od mora</p>
                        <p>30 m</p>
                    </div>
                </div>
                <!-- Naračadsti button POGLEDAJ STRANICU -->
                <a href="https://villa-vlastelini.com/porto-longo/" target="_blank" title="pogledaj_stranicu">
                    <button class="btn_pogledaj_stranicu btn_porto_longo">
                        pogledaj stranicu
                    </button>
                </a>
            </div>
        </div>
        <!-- Slika solarnih panela -->
        <div id="elektrane" class="flex-row">
            <img src="./assets/images/solar_panel_1.png" alt="Solarni paneli" class="slika_full_screen">
        </div>
        <!-- Section 7 - Tekst o sunčanim elektranama -->
        <div class="section_7"
                data-aos="zoom-in" 
                data-aos-delay="100"
                data-aos-duration="1000"
                data-aos-easing="ease-in-out"
                data-aos-once="true">
            <div class="section_7__content">
                <h1 class="m_b_xm">Sunčane elektrane</h1>
                <p class="m_b_xm">
                    2012. godine osnovane su tvrtke Sol Navitas Labin d.o.o. i Energo Sol Labin d.o.o. s ciljem proširenja djelatnosti na proizvodnju struje iz sunčane energije.
                </p>
                <p class="m_b_xm">
                    Nakon dvije godine analize i odabira tehnoloških rješenja, usklađivanja projekta sa zakonskim regulativama te provođenja samog projekta izgradnje sunčanih elektrana, početkom 2015. godine u rad su puštene prve sunčane elektrane na Labinštini, i to elektrana snage 180 kW na lokaciji Novi Labin, lokalitet Dubrova te elektrana snage 480 kW na lokaciji Ladenci/Batelići Cere, na periferiji grada Labina.
                </p>
                <p>
                    Sunčane elektrane električnu energiju proizvode u sunčanim ćelijama. Takve elektrane su tih uređaj koji nema pokretnih dijelova i ne ispuštaju onečišćujuće tvari u atmosferu, što ih čini značajno zdravijima za okoliš, u odnosu na tehnologije proizvodnje električne energije fosilnim gorivima. Fotonaponski sustav ne proizvodi buku, ne ispušta onečišćujuće tvari u atmosferu te proizvodi potpuno zelenu energiju.   
                </p>
            </div>
        </div>
        <!-- Section 8 - Energo Sol Labin d.o.o. -->
        <div class="section_8 flex-row">
            <div>
                <img src="./assets/images/Energo_sol.png" alt="Solarni paneli" class="slika_desno box_shadow_img"
                  data-aos="fade-up" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
            </div>
            <div class="section_8__content text_lijevo bg_orange box_shadow_text pd_tb_l m_b_l"
                  data-aos="fade-right" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <div class="section_8__content_text">
                    <h2 class="m_b_xm">Energo Sol Labin d.o.o.</h2>
                    <p>
                        Sunčana elektrana se nalazi u mjestu<br> Ladenci/Batelići na periferiji grada Labina.<br> 
                        Opremljena je fotonaponskim modulima koji<br> stvaraju ukupnu snagu od 480 kW.
                    </p>
                </div>
            </div>
        </div>
        <!-- Section 9 -  Sol Navitas Labin d.o.o. -->
        <div class="section_9 flex-row m_t_xl">
            <div>
                <img src="./assets/images/Sol_navitas.png" alt="Solarni paneli" class="slika_lijevo box_shadow_img"
                  data-aos="fade-right" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
            </div>
            <div class="section_9__content text_desno bg_orange box_shadow_text pd_tb_l" 
                  data-aos="fade-up" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <div class="section_9__content_text">
                    <h2 class="m_b_xm">Sol Navitas Labin d.o.o.</h2>
                    <p>
                        Sunčana elektrana se nalazi u mjestu Dubrova,<br> na periferiji grada Labina.<br>
                        Opremljena je fotonaponskim modulima koji<br> stvaraju ukupnu snagu od 180 kW.
                    </p>
                </div>
            </div>
        </div>
        <!-- Slika Labina -->
        <div id="section_10 flex-row">
            <img src="./assets/images/Labin.png" alt="Grad Labin" class="slika_panorama_labina m_t_xl">
        </div>
        <!-- Section 11 - Velo Kafe -->
        <div class="section_11 flex-row m_t_xl">
            <div>
                <img src="./assets/images/velo_kafe_1.png" alt="Velo Kafe" class="slika_desno box_shadow_img"
                    data-aos="fade-up" 
                    data-aos-delay="100"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out"
                    data-aos-once="true">
            </div>
            <div class="section_11__content text_lijevo bg_orange box_shadow_text pd_tb_l"
                  data-aos="fade-right" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <div class="section_11__content_text">
                    <h1 class="m_b_xm">Velo Kafe</h1>
                    <p>
                        Zgrada Velo Kafe se nalazi u centru starog grada Labina na adresi Titov trg 12. Povijest zgrade započinje početkom 19. stoljeća kada je labinski općinski liječnik dr. Barilovich sagradio kuću na mjestu današnje gradske kavane. U nadolazećim godinama taj će objekt postati jedinstvena institucija okupljanja i druženja tadašnje labinske elite.
                    </p>
                </div>
            </div>
        </div>
        <!-- Section 12 - trim manja teksta o Velo Kafe -->
        <div class="section_12 flex-row">
            <div class="usluge usluge2"
                  data-aos="zoom-in" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <p>
                    Već idući vlasnik gosp. Negri zgradu pretvara u kavanu, nazvavši je "Casino", prema istoimenom udruženju građana što je tih godina djelovalo u Labinu i čija je kavana bila redovno mjesto okupljanja. Godine 1893. gosp. Negri se obratio općinskim vlastima s molbom da mu se, radi zaštite od ljetnih vrućina, dozvoli izgradnja drvenog natkrivenog trijema.  
                </p>
            </div>
            <div class="usluge usluge2"
                  data-aos="zoom-in" 
                  data-aos-delay="300"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <p>
                    Dvadesetih godina ovog stoljeća zgrada dobiva još jedan kat, a tridesetih je godina na terasi postavljena metalna konstrukcija s kosinom radi prihvata već podosta razgranate Glicinije. Kratko vrijeme poslije Drugog svjetskog rata gradska kavana je bila  zatvorena, a ponovo je rekonstruirana krajem 1985. godine.
                </p>
            </div>
            <div class="usluge usluge2"
                  data-aos="zoom-in" 
                  data-aos-delay="500"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <p>
                    Trinaest godina kasnije, tadašnji vlasnik zgrade, HP Rabac d.d., prodaje je na javnom natječaju tvrtci Hena d.o.o., koja godinu dana nakon toga vrši cjelovitu rekonstrukciju najpoznatije labinske kavane. Krajem 20. stoljeća "Velo Kafe" zasjalo je u novom obliku s promijenjenim sadržajem adekvatnim zahtjevima modernog doba, ali istovremeno zadržavajući svoju tradicionalnost i povijesnu trajnost.
                </p>
            </div>
        </div>
        <!-- Section 13 - Ugostiteljski obrt -->
        <div id="ugostiteljski_objekt" class="section_13 flex-row">
            <div>
                <img src="./assets/images/velo_kafe_2.png" alt="Velo Kafe - ugostiteljski objekt" class="slika_lijevo box_shadow_img"
                  data-aos="fade-right" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
            </div>
            <div class="section_13__content text_desno bg_orange box_shadow_text pd_tb_l"
                  data-aos="fade-up" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <div class="section_13__content_text">
                    <h1 class="m_b_xm section_13__text">Ugostiteljski<br> objekt</h1>
                    <p class="m_b_xm section_13__text">
                        Ugostiteljski objekt Velo Kafe smješten je na labinskom starogradskom trgu. Jedan je od najvećih i najljepših ugostiteljskih objekata na ovom području. Zgrada je izgrađena početkom 19. stoljeća, a u međuvremenu je nekoliko puta dograđivana i adaptirana.
                    </p>
                    <p class="m_b_xm section_13__text">
                        Ugostiteljski objekt sastoji se od tri etaže, od kojih svaka ima svoju zasebnu funkciju, a zajedno pružaju cjelovitu ugostiteljsku uslugu.
                    </p>
                    <p class="section_13__text">
                        U suterenu objekta nalaze se kuhinja te konoba/restoran s velikim kaminom. Zbog topline uređenja u zimskom periodu stvoren je jedinstven i intiman ugođaj te je zajamčeno uživanje u gastronomskim delicijama internacionalnih i izvornih istarskih specijaliteta.
                    </p>
                </div>
            </div>
        </div>
        <!-- Section 14 - Ugostiteljski obrt drugi dio -->
        <div class="section_14 flex-row m_t_xl">
            <div>
              <img src="./assets/images/stari_grad.png" alt="Stari grad" class="slika_desno box_shadow_img"
                  data-aos="fade-up" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
            </div>
            <div class="section_14__content text_lijevo bg_orange box_shadow_text pd_tb_l"
                  data-aos="fade-right" 
                  data-aos-delay="100"
                  data-aos-duration="1000"
                  data-aos-easing="ease-in-out"
                  data-aos-once="true">
                <div>
                    <p class="m_b_xm section_14__content_text">
                        U prizemlju ugostiteljskog objekta nalazi se prekrasna gradska kavana s velikom terasom koja za vrijeme toplijih dana pruža izvrstan ugođaj i užitak boravka. Kavana Velo Kafe nudi veliki izbor toplih i osvježavajućih napitaka, sendviča, dnevno svježih kolača, sladoleda i sladolednih kupova, a bogatu ponudu odnedavno upotpunjuju i ukusni brunch-evi. Dugi niz godina nezaobilazno je mjesto jutarnjeg okupljanja.
                    </p>
                    <p class="m_b_xm section_14__content_text">
                        U sklopu objekta, na prvoj etaži nalazi se moderno uređen restoran čiju ponudu čine svježe i kvalitetne namirnice u spoju tradicionalne i moderne kuhinje. Gostima je na raspolaganju i bogata vinska karta sa vrhunskim domaćim i stranim vinima. U restoranu se istodobno može poslužiti veći broj gostiju, a u ljetnim mjesecima gosti mogu uživati na prostranoj terasi u hladovini gusto razgranate stoljetne Glicinije (jedinstvenog zaštićenog botaničkog spomenika prirode usred starog grada Labina), s pogledom na prekrasan labinski starogradski trg.
                    </p>
                </div>
            </div>
        </div>
        <!-- Footer - gdje se nalaze kontakt informacije -->
        <div id="kontakt" class="footer flex-row m_t_xl">
            <div class="usluge usluge_kontakt">
                <h2 class="m_b_xm">Kontakt</h2>
                <p>
                    Vlastelini d.o.o.,<br> 
                    Titov Trg 12, 52220 Labin, Hrvatska
                </p>
            </div>
            <div class="usluge usluge_kontakt m_t_l">
                <p>
                    <a href="tel:0038552852700" target="_blank" title="kontakt">telephone: +385 (0)52 852 700</a><br>
                    <a href="mailto:info@vlastelini.hr" target="_blank" title="kontakt">email: info@vlastelini.hr</a>
                </p>
                <p class="m_t_l">
                    © Vlastelini d.o.o. 2018. All Rights Reserved
                </p>
            </div>
            <div class="usluge m_t_l usluge_kontakt">
                <p>
                    Registrirano na Trgovačkom sudu u Pazinu.<br>
                    MBS: 130050751
                </p>
            </div>
        </div>
  </div>
  <!-- KRAJ - END -->
</template>

<script>
import AOS from 'aos'; //animacije  -- https://github.com/michalsnik/aos
import 'aos/dist/aos.css'; //animacije
import { Hooper, // slider -- https://github.com/baianat/hooper
        Slide,
        Progress as HooperProgress,
        Pagination as HooperPagination,
        Navigation as HooperNavigation } from 'hooper';
import 'hooper/dist/hooper.css'; // slider css

//import { Slide } from 'vue-burger-menu'

 export default {
    name: 'App',
    components: {
        Hooper,
        Slide,
        HooperPagination,
    },
    data () {
      return {
        hooperSettings: { // dio za slider
            itemsToShow: 1,
            //infiniteScroll: true,
            autoPlay: true,
            playSpeed: 5000,
            transition: 3000,
            rtl: false,
            touchDrag: true,
            initialSlide: 1,
            wheelControl: false,
        }
      }
    }
  }
AOS.init();

</script>

<style>
/*
CSS reset
*/
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed,
figure, figcaption, footer, header, hgroup,
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
 margin: 0;
 padding: 0;
 border: 0;
 font-size: 100%;
 font: inherit;
 vertical-align: baseline;
}

#app {
    display: flex;
    flex-direction: column;
}
/* Osnovni css za body, naslove, liste, paragraf*/
html {
    scroll-behavior: smooth;
}
body{
    font-family: 'Source Sans Pro', sans-serif;
    font-size: 14px;
    background-color: #CFCFCE;
    overflow-x: hidden;
    color: #474747;
}
h1, h2 {
    font-family: 'Playfair Display', serif;
    font-weight: bold;
}
h1 {
    font-size: 46px;
    line-height: 110%;
}
h2 {
    font-size: 28px;
    line-height: 120%;
    letter-spacing: 1.2px;
}
ul li {
    font-size: 16px;
}
ol li {
    line-height: 150%;
    padding-left: 10px;
    padding-top: 5px;
}
p {
    line-height: 150%;
}
/*LInkovi u navigaciji*/
a, a:link, a:visited {
    color: #585858;
    text-decoration: none;
}
a:hover {font-weight: bold;}
/*Linkovi u divu kontakta za telefon i email*/
a[title="kontakt"] {color: inherit;}
button:focus {outline:0;}
.pd_tb_s {
    padding: 20px 0px;
}
.pd_tb_m {
    padding: 40px 0px;
}
.pd_tb_l {
    padding: 60px 0px;
}
.m_t_s {
    margin-top: 20px;
}
.m_t_m {
    margin-top: 40px;
}
.m_t_l {
    margin-top: 60px;
}
.m_t_xl {
    margin-top: 80px;
}
.m_b_s{
    margin-bottom: 10px;
}
.m_b_m{
    margin-bottom: 20px;
}
.m_b_xl {
    margin-bottom: 80px;
}
.m_b_xm {
    margin-bottom: 30px;
}
.m_b_l {
    margin-bottom: 70px;
}
.flex-row {
    display: flex;
    flex-flow: row;
}
.navigacija {
    display: flex;
    justify-content: flex-end;
}
.navi {
    list-style: none;
    justify-content: space-around;
    margin-right: 5%;
    padding: 35px 0px;
    width: 60%;
}
/*klasa za jezik u navigaciji*/
.eng {
    margin-left: 70px;
}
/*narancasta pozadina*/
.bg_orange {
    background-color: rgb(144, 85, 5, 0.42);
    color: #FFFFFF;
}
.box_shadow_text {
    box-shadow: 0 10px 10px -10px #808080b4;
}
.box_shadow_img {
    box-shadow: 0 0 30px 2px #808080b4;
}
/*klasa u kojpj se nalaze logo i tekst o nama*/
.o_nama {
    width: 45%;
    height: 100%;
    display: flex;
    flex-flow: column;
    position: relative;
    z-index: 1;
}
/*klasa za slider*/
.slider {
    height: 550px;
    width: 60%;
    right: 0px;
    position: absolute;
}
/*klasa za slike u slideru*/
.slider_img {
    height: 550px;
    object-fit: cover;
    width: 100%;
}
/*klasa za logo*/
#logo {
    width: 50%;
    align-self: center;
}
/*div za o nama section*/
.o_nama__box {
    width:100%;
    align-self: center;
    display: flex;
    justify-content: center;
}
#o_nama_link {
    width: 50%;
}
#section_2 {
    justify-content: center;
}
/*klasa za tekst u drugom section-u*/
.usluge {
    width: 15%;
    padding: 100px 80px 70px 80px;
}
.usluge2 {
    padding: 70px 80px 70px 80px;
}
/*klasa za tekst u drugom section-u, ali samo za tekst o panelima*/
.usluge_paneli {
    padding: 70px;
    width: 15%;
}
/*klasa za div sa slikom u drugom section-u */
.usluge_slika_div {
    text-align: center;
    margin-bottom: 30px;
}
/*klasa za sliku u drugom section-u*/
.usluge_slika {
    width: 80px;
    height: 80px;
}
/*klasa za sliku u drugom section-u ali samo za sliku o panelima*/
.usluge_slika_paneli {
    width: 110px;
    height: 110px;
}
/*treći section*/
/* klasa za sliku koja se nalazi na lijevoj poziciji na stranici*/
.slika_lijevo{
    width: 100%;
    position: relative;
}
.text_desno {
    height: 100%;
    width: 50%;
    position: relative;
}
.text_desno::after {
    content: "";
    position: absolute;
    height: 100%;
    width: 20%;
    background-color: rgb(144, 85, 5, 0.42);
    top: 0px;
    left: -20%;
}
/*klasa za content sa desne strane*/
.section_3 {
    margin-top: 130px;
    display: flex;
    justify-content: center;
}
/*klasa za treći section samo za tekst*/
.section_3__content {
    width: 50%;
}
.section_3__text {
    padding-left: 10px;
    width: 75%;
}
/*Četvrti section - Villa Vlastellini - Santo Spirito*/
.section_4 {
    flex-direction: row-reverse;
}
.section_4__content {
    margin-top: 90px;
    padding-left: 150px;
}
/*Četvrti section - tekst ispod naslova*/
.section_4__text {
    width: 72%;
}
.section_4__content_text {
    padding-left: 60px;
}
.slika_desno{
    width: 100%;
    position: relative;
}
.text_lijevo {
    height: 100%;
    width: 40%;
    position: relative;
}
.text_lijevo::after {
    content: "";
    position: absolute;
    height: 100%;
    width: 20%;
    background-color: rgb(144, 85, 5, 0.42);
    top: 0px;
    right: -20%;
    /*box-shadow: 0 10px 10px -10px #808080b4;*/
}
/*Klasa za ikone za usluge u vilama*/
.villa_icons {
    width: 40px;
    color: #FFF;
    margin-bottom: 10px;
}
/*Četvrti section i peti section - klasa za div u kojem se nalaze sve usluge koje vila ima (kao neki container za sve usluge)*/
.section_4__usluge, .section_5__usluge {
    justify-content: space-between;
    display: flex;
    width: 70%;
    align-items: baseline;
}
/*Četvrti section - klasa za svaku pojedinu uslugu */
.villa_usluge {
    text-align: center;
    margin-bottom: 10px;
}
/*Klasa za opis usluge koji se nalazi ispod ikone (Površina ville, spavaće sobe ...)*/
.villa_icons_text {
    font-size: 13px;
    line-height: 120%;
    margin-bottom: 10px;
}
/*Klasa za button - POGLEDAJ STRANICU - koji se nalazi u četvrtom i petom section-u*/
.btn_pogledaj_stranicu {
    color: #FFF;
    background-color: #F89A1F;
    box-shadow: 0 3px 2px -2px #808080b4;
    text-transform: uppercase;
    border: none;
    padding: 10px 22px;
    margin-top: 25px;
    font-size: 12px;
    font-weight: bold;
    letter-spacing: 1px;
}
/*Peti section - Villa Vlastellini - Porto Longo*/
.section_5__content {
    margin-top: 100px;
}
.section_5__text {
    padding-left: 190px;
    text-align: left;
    width: 55%;
}
.section_5__usluge {
    padding-left: 190px;
    width: 55%;
}
.btn_porto_longo {
    margin-left: 190px;
}
/*Klasa za sliku u šestom section-u (solarni paneli)*/
.slika_full_screen {
    width: 100%;
    height: 400px;
    filter: sepia(100%);
    -webkit-box-shadow: 0 0 50px #808080b4;
            box-shadow: 0 0 50px #808080b4;       
}
/*Sedmi section - Sunčane elektrane*/
.section_7 {
    width: 35%;
    margin: auto;
    padding: 70px 0px;
}
/*Energo Sol Labin d.o.o.)*/
.section_8 {
    flex-direction: row-reverse;
}
.section_8__content {
    padding-left: 150px;
    margin-top: 30px;
}
.section_8__content_text {
    padding-left: 60px;
}
/*Deveti section - Sol Navitas Labin d.o.o.*/
.section_9__content {
    display: flex;
    justify-content: center;
    margin-top: 250px;
}
/*Deseti section - Slika Panorama Labina*/
.section_10 {
    object-fit: cover;
}
.slika_panorama_labina {
    width: 100%;
    height: 450px;;
    -webkit-box-shadow: 0 0 50px #808080b4;
            box-shadow: 0 0 50px #808080b4; 
    object-fit: cover;
}
/*Jedanaesti section - Velo Kafe*/
.section_11 {
    flex-direction: row-reverse;
}
.section_11__content {
    padding-left: 150px;
    margin-top: 120px;
}
.section_11__content_text {
    padding-left: 60px;
    width: 40%;
}
/* 12. Section - tri mala teksta ispod section-a Velo Kafe*/
.section_12 {
    justify-content: center;
}
/* 13. section - Ugostiteljski objekt*/
.section_13__content {
    display: flex;
    justify-content: center;
    margin-top: 80px;
}
.section_13__text {
    width: 60%;
    display: flex;
    padding-left: 170px;
}
/* 14. section - Ugostiteljski objekt - drugi dio*/
.section_14 {
    flex-direction: row-reverse;
}
.section_14__content {
    padding-left: 150px;
}
.section_14__content_text {
    padding-left: 60px;
    width: 60%;
}
.footer {
    background-color: #959693;
    color: #FFF;
    justify-content: center;
}
/*klase za navigaciju na slideru*/
.hooper-indicator {
    height: 12px;
    border-radius: 10px;
}
.hooper-indicator.is-active,
.hooper-indicator:hover {
    background-color: #F89A1F;
}
/************
RESPONSIVE DESIGN
***************/
@media only screen and (max-width: 1750px) {
.section_3__content {
    width: 55%;
}
.section_3__text {
    width: 80%;
}
.section_11__content {
    margin-top: 100px;
}
.section_13__text {
    width: 60%;
    padding-left: 150px;
}
}
@media only screen and (max-width: 1700px) {
.section_3__content {
    width: 60%;
}
.section_11__content {
    margin-top: 100px;
}
.section_13__text {
    width: 60%;
    padding-left: 120px;
}
.section_4__text {
    width: 80%;
}
.section_4__usluge {
    width: 80%;
}
.section_9__content {
    margin-top: 200px;
}
.section_14__content_text {
    width: 70%;
}
}
@media only screen and (max-width: 1670px) {
#o_nama_link {
    width: 60%;
    padding-left: 80px;
}
.section_3__content {
    width: 65%;
}
.section_7 {
    width: 45%;
}
.section_11__content_text {
    width: 55%;
}
.section_14__content_text {
    width: 80%;
}
}
@media only screen and (max-width: 1600px) {
.section_11__content_text {
    width: 65%;
}
.section_14__content_text {
    width: 85%;
}
}
@media only screen and (max-width: 1550px) {
#logo {
    padding-right: 120px;
}
.navi {
    margin-right: 3%;
}
#o_nama_link {
    padding-right: 120px;
}
.usluge {
    width: 17%;
    padding: 100px 40px 70px 40px;
}
.usluge2 {
    padding: 70px 60px 70px 60px;
}
.usluge_paneli {
    width: 17%;
}
.section_3 {
    margin-top: 100px;
}
.section_3__content {
    width: 70%;
}
.section_3__text {
    width: 80%;
}
.section_4__content {
    margin-top: 60px;
    padding-left: 120px;
    padding-right: 90px;
}
.section_4__text {
    width: 100%;
}
.section_4__content_text {
    padding-left: 0px;
}
.section_4__usluge {
    width: 100%;
}
.section_5__content {
    margin-top: 80px;
}
.section_5__text {
    padding-left: 80px;
    width: 75%;
}
.section_5__usluge {
    padding-left: 80px;
    width: 75%;
}
.btn_porto_longo {
    margin-left: 80px;
}
.text_desno::after {
    width: 27%;
    left: -27%;
}
.text_lijevo::after {
    width: 27%;
    right: -27%;
}
.slika_full_screen {
    height: 350px;       
}
.section_7 {
    width: 45%;
}
.section_8__content {
    padding-left: 60px;
    padding-right: 90px;
}
.section_8__content_text {
    padding-left: 60px;
}
.section_11__content {
    padding-left: 60px;
    padding-right: 90px;
    margin-top: 100px;
}
.section_11__content_text {
    width: 70%;
}
.section_13__content {
    margin-top: 60px;
}
.section_13__text {
    width: 75%;
    padding-left: 80px;
}
.section_14__content {
    padding-left: 60px;
    padding-right: 90px;
}
.section_14__content_text {
    width: 90%;
}
.eng {
    margin-left: 40px;
}
}
@media only screen and (max-width: 1480px) {
.section_3__content {
    width: 80%;
}
.section_9__content {
    margin-top: 170px;
}
.section_11__content_text {
    width: 90%;
}
.section_11__content {
    margin-top: 70px;
}
}
@media only screen and (max-width: 1400px) {
.o_nama {
    width: 50%;
}
.usluge {
    width: 21%;
    padding: 100px 20px 70px 20px;
}
.usluge_paneli {
    width: 21%;
}
.usluge2 {
    padding: 70px 30px 70px 30px;
}
.section_3 {
    margin-top: 60px;
}
.section_3__content {
    width: 87%;
}
.section_3__text {
    width: 90%;
}
.section_4__content {
    margin-top: 40px;
    padding-left: 40px;
    padding-right: 40px;
    width: 50%;
}
.section_5__content {
    margin-top: 40px;
    padding-left: 40px;
    padding-right: 40px;
}
.section_5__text {
    padding-left: 0px;
    width: 100%;
}
.section_5__usluge {
    padding-left: 0px;
    width: 100%;
}
.btn_porto_longo {
    margin-left: 0px;
}
.slika_full_screen {
    height: 300px;       
}
.section_7 {
    width: 55%;
}
.section_8__content {
    padding-left: 40px;
    padding-right: 110px;
}
.section_8__content_text {
    padding-left: 0px;
}
.section_9__content {
    margin-top: 120px;
    padding-right: 40px;
}
.slika_panorama_labina {
    height: 400px; 
}
.section_11__content {
    padding-left: 40px;
    padding-right: 90px;
    margin-top: 40px;
}
.section_11__content_text {
    width: 100%;
    padding-left: 0px;
}
.section_13__content {
    margin-top: 40px;
    padding-left: 40px;
    padding-right: 40px;
}
.section_13__text {
    width: 80%;
    padding-left: 40px;
}
.section_14__content {
    padding-left: 0px;
    padding-right: 90px;
    width: 50%;
}
.section_14__content_text {
    width: 100%;
}
}
@media only screen and (max-width: 1200px) {
.flex-row {
    display: flex;
    flex-flow: row;
    flex-wrap: wrap;
}
.navigacija {
    justify-content: space-around;
}
.navi {
    margin-right: 0%;
    width: 100%;
}
.eng {
    margin-left: 40px;
}
.o_nama {
    width: 100%;
    flex-flow: column;
    flex-wrap: wrap;
    justify-content: center;
}
.slider {
    height: 550px;
    width: 100%;
    position: absolute;
    margin-top: 250px;
}
.slider_img {
    height: 100%;;
    object-fit: cover;
    width: 100%;
}
#logo {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-top: 20px;
    padding-right: 0px;
}
.o_nama__box {
    width:100%;
    display: flex;
    justify-content: flex-start;
    margin-top: 620px;
}
#o_nama_link {
    width: 60%;
    padding-left: 80px;
    padding-right: 80px;
    justify-content: flex-start;
}
#section_2 {
    justify-content: space-between;
    padding-left: 80px;
    padding-right: 80px;
}
.usluge {
    width: 25%;
    padding: 100px 0px 70px 0px;
}
.usluge_paneli {
    padding: 70px;
    width: 25%;
}
.usluge_slika_div {
    text-align: center;
    margin-bottom: 30px;
}
.usluge_slika {
    width: 80px;
    height: 80px;
}
.usluge_slika_paneli {
    width: 110px;
    height: 110px;
}
.text_desno::after {
    width: 0px;
    left: 0px;
}
.text_lijevo::after {
    width: 0px;
    right: 0px;
}
.slika_lijevo{
    width: 100%;
    height: 650px;
    object-fit: cover;
    display: block;
    position: relative;
}
.slika_desno{
    width: 100%;
    height: 650px;
    object-fit: cover;
    position: relative;
    display: block;
}
#kuce_za_odmor {
    flex-flow: column;
}
.text_desno {
    width: 100%;
}
.text_desno::after {
    display: none;
}
.section_3 {
    margin-top: 20px;
    display: flex;
    justify-content: center;
}
.section_3__content {
    width: 100%;
    padding-left: 80px;
    padding-right: 80px;
}
.section_3__text {
    width: 100%;
}
.section_4 {
    flex-direction: column;
    display: block;
}
.section_4__content {
    margin-top: 20px;
    padding-left: 0px;
    padding-right: 0px;
}
.section_4__text {
    width: 100%;
}
.section_4__content_text {
    width: 60%;
    padding-left: 80px;
}
.section_4__text {
    padding-left: 0px;
    padding-right: 0px;
}
.text_lijevo {
    width: 100%;
}
.section_4__usluge, .section_5__usluge {
    width: 100%;
}
.sec_5 {
    flex-direction: column;
    display: block;
}
.section_5__content {
    padding-left: 0px;
    padding-right: 0px;
    margin-top: 20px;
}
.section_5__text {
    padding-left: 80px;
    width: 60%;
}
.section_5__usluge {
    padding-left: 80px;
    width: 60%;
}
.btn_porto_longo {
    margin-left: 80px;
}
.slika_full_screen {
    width: 100%;
    height: 300px;
    filter: sepia(100%);     
}
.section_7 {
    width: 100%;
    padding: 70px;
    padding-left: 0px;
    padding-right: 0px;
    margin: none;
    display:block;
}
.section_7__content {
    padding-left: 80px;
    padding-right: 80px;
    width: 80%;
}
.section_8 {
    flex-direction: column;
    display: block;
}
.section_8__content {
    padding-left: 0px;
    padding-right: 0px;
    margin-top: 20px;
}
.section_8__content_text {
    padding-left: 80px;
}
.section_9 {
    flex-direction: column;
    display: block;
    margin-top: 0px;
}
.section_9__content {
    margin-top: 20px;
    padding-left: 0px;
    padding-right: 0px;
    width: 100%;
    justify-content: flex-start;
}
.section_9__content_text {
    padding-left: 80px;
    width: 100%;
}
.slika_panorama_labina {
    height: 400px;;
}
.section_11 {
    flex-direction: column;
    display: block;
}
.section_11__content {
    padding-left: 0px;
    padding-right: 0px;
    margin-top: 20px;
}
.section_11__content_text {
    padding-left: 80px;
    width: 60%;
}
.section_12 {
    justify-content: space-between;
    padding-left: 80px;
    padding-right: 80px;
}
.usluge2 {
    padding: 70px 0px 70px 0px;
}
.section_13 {
    flex-direction: column;
    display: block;
}
.section_13__content {
    margin-top: 20px;
    padding-left: 0px;
    padding-right: 0px;
}
.section_13__text {
    width: 80%;
    padding-left: 80px;
}
.section_14 {
    flex-direction: column;
    display: block;
}
.section_14__content {
    margin-top: 20px;
    padding-left: 0px;
    padding-right: 0px;
}
.section_14__content_text {
    padding-left: 80px;
    width: 80%;
}
.footer {
    background-color: #959693;
    color: #FFF;
    justify-content: space-between;
    padding-left: 80px;
    padding-right: 80px;
}
.usluge_kontakt {
    padding-top: 70px;
    padding-bottom: 20px;
}
}
@media only screen and (max-width: 1000px) {
.slika_lijevo{
    height: 550px;
}
.slika_desno{
    height: 550px;
}
}
@media only screen and (max-width: 900px) {
.slika_lijevo{
    height: 500px;
}
.slika_desno{
    height: 500px;
}
.usluge {
    width: 30%;
}
.usluge_paneli {
    padding: 70px 10px;
    width: 30%;
}
.slika_panorama_labina {
    height: 350px;;
}
.slika_full_screen {
    height: 270px;     
}
}
@media only screen and (max-width: 800px) {
.slider {
    height: 480px;
}
.o_nama__box {
    margin-top: 550px;
}
.slika_lijevo{
    height: 490px;
}
.slika_desno{
    height: 490px;
}
.section_4__content_text {
    width: 80%;
    padding-left: 30px;
}
.section_5__text {
    width: 80%;
    padding-left: 30px;
}
.section_5__usluge {
    width: 80%;
    padding-left: 30px;
}
.btn_porto_longo {
    margin-left: 30px;
}
.slika_panorama_labina {
    height: 320px;
}
.slika_full_screen {
    height: 250px;     
}
#o_nama_link {
    width: 80%;
    padding-left: 30px;
    padding-right: 30px;
}
.section_3__content {
    padding-left: 30px;
    padding-right: 30px;
}
.section_7__content {
    padding-left: 30px;
    padding-right: 30px;
    width: 80%;
}
.section_8__content_text {
    padding-left: 30px;
}
.section_9__content_text {
    padding-left: 30px;
}
.section_11__content_text {
    padding-left: 30px;
    width: 60%;
}
.section_12 {
    justify-content: space-around;
    padding-left: 20px;
    padding-right: 20px;
}
.section_13__text {
    width: 80%;
    padding-left: 30px;
}
.section_14__content_text {
    padding-left: 30px;
    width: 80%;
}
#section_2 {
    justify-content: space-around;
    padding-left: 20px;
    padding-right: 20px;
}
.usluge {
    width: 30%;
    padding: 100px 0px 70px 0px;
}
.usluge_paneli {
    padding: 70px 0px;
    width: 30%;
}
.footer {
    justify-content: space-around;
    padding-left: 20px;
    padding-right: 20px;
}
}
@media only screen and (max-width: 700px) {
.slider {
    height: 400px;
    margin-top: 150px;
}
.o_nama__box {
    margin-top: 420px;
}
.logo-img {
    width: 250px;
}
#logo {
    margin-top: -30px;
}
.pd_tb_l {
    padding: 30px 0px;
}
.slika_lijevo{
    height: 400px;
}
.slika_desno{
    height: 400px;
}
h1 {
    font-size: 40px;
}
h2 {
    font-size: 22px;
}
.usluge_slika {
    width: 60px;
    height: 60px;
}
.usluge_slika_paneli {
    width: 90px;
    height: 90px;
}
.usluge_kontakt {
    padding-top: 40px;
    padding-bottom: 40px;
}
.slika_panorama_labina {
    height: 300px;
}
.slika_full_screen {
    height: 230px;     
}
}
@media only screen and (max-width: 600px) {
.slider {
    height: 350px;
}
.o_nama__box {
    margin-top: 370px;
}
.slika_lijevo{
    height: 350px;
}
.slika_desno{
    height: 350px;
}
.slika_panorama_labina {
    height: 300px;
}
.slika_full_screen {
    height: 220px;     
}
.m_b_xl {
   margin-bottom: 30px;
}
#section_2 {
    flex-direction: column;
    padding: 40px 0px;
}
.usluge {
    width: 90%;
    padding: 20px;
}
.usluge_paneli {
    width: 90%;
    padding: 0px 20px;
}
.section_11__content_text {width: 80%;}
.section_12 {padding: 30px 0px;}
.footer {padding: 30px 0px;}
.usluge_kontakt {padding-top: 0px;}
.m_b_l {margin-top: 20px;}
.eng {margin-left: 0px;}
}
@media only screen and (max-width: 500px) {
.slider {
    height: 290px;
}
.o_nama__box {
    margin-top: 310px;
}
a {
    padding-left: 5px;
}
.slika_lijevo{
    height: 280px;
}
.slika_desno{
    height: 280px;
}
.slika_panorama_labina {
    height: 250px;
}
.slika_full_screen {
    height: 180px;     
}
.usluge {width: 85%;}
.usluge_paneli {width: 85%;}
}
@media only screen and (max-width: 400px) {
.slider {height: 270px;}
.o_nama__box {margin-top: 290px;}
.slika_lijevo{height: 250px;}
.slika_desno{height: 250px;}
.slika_panorama_labina {height: 230px;}
.slika_full_screen {height: 160px;}
}
@media only screen and (max-width: 360px) {
.slika_lijevo{height: 230px;}
.slika_desno{height: 230px;}
.slika_panorama_labina {height: 210px;}
.slika_full_screen {height: 150px;}
}
</style>
