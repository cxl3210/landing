# landing
# landing

playPrevious:function(){
  var index=this.attributes['index'];
  index=index-1;
  if(index===-1){
    if(this.attributes['loop']){
      index=audioData.length-1;
    }else{
       this.handler.state = constants.states.START_MODE;
       var message = 'You have reached at the start of the playlist.';
       this.response.speak(message).audioPlayerStop();
       return this.emit(':responseReady');
    }
  }
    this.attributes['index'] = index;
    this.attributes['offsetInMilliseconds'] = 0;
    this.attributes['playbackIndexChanged'] = true;
    controller.plays.call(this);
}


play:function(){
  this.attributes['state']='PLAYMODE';
  if (this.attributes['playbackFinished']) {
      this.attributes['index'] = 0;
      this.attributes['offsetInMilliseconds'] = 0;
      this.attributes['playbackIndexChanged'] = true;
      this.attributes['playbackFinished'] = false;
  }
}


var audioEventHandlers=function(){
   'PlaybackFinished' : function () {
        this.attributes['playbackFinished'] = true;
        this.attributes['enqueuedToken'] = false;
        this.emit(':saveState', true);
}



 
 
  1912
 
 
  1914
 
 
  1915
 
 
  1920
 
 
  1923
 
 
  1924
 
 
  1925
 
 
  1926
 
 
  1927
 
 
  1929
 
 
  1930
 
 
  1931
 
 
  1934
 
 
  1935
 
 
  1936
 
 
  1937
 
 
  1942
 
 
  1943
 
 
  1944
 
 
  1945
 
 
  1946
 
 
  1948
 
 
  1949
 
 
  1950
 
 
  1951
 
 
  1952
 
 
  1953
 
 
  1954
 
 
  1955
 
 
  1956
 
 
  1957
 
 
  1958
 
 
  1959
 
 
  1960
 
 
  1961
 
 
  1962
 
 
  1963
 
 
  1964
 
 
  1965
 
 
  1966
 
 
  1967
 
 
  1968
 
 
  1969
 
 
  1970
 
 
  1971
 
 
  1972
 
 
  1973
 
 
  1974
 
 
  1975
 
 
  1976
 
 
  1977
 
 
  1978
 
 
  1979
 
 
  1980
 
 
  1981
 
 
  1982
 
 
  1983
 
 
  1985
 
 
  1986
 
 
  1987
 
 
  1988
 
 
  1989
 
 
  1990
 
 
  1991
 
 
  1992
 
 
  1993
 
 
  1994
 
 
  1995
 
 
  1996
 
 
  1997
 
 
  1998
 
 
  1999
 
 
  2000
 
 
  2001
 
 
  2002
 
 
  2003
 
 
  2004
 
 
  2005
 
 
  2006
 
 
  2007
 
 
  2008
 
 
  2009
 
 
  2010
 
 
  2011
 
 
  2012
 
 
  2013
 
 
  2014
 
 
  2015
 
 
  2016
 





productblishes Sharp Electronics GmbH (SEA) as sales base in Austria (merges with SEEG in 2004 to become SEEG Austria Branch). Establishes Sharp-Roxy Sales (Singapore) Pte., Ltd. (SRS) as sales base in Singapore. Establishes Sharp Electrónica España S.A. (SEES) as manufacturing and sales base in Spain (ceases manufacturing in 2011). Senior Executive Director Haruo Tsuji named president, President Akira Saeki named chairman. Establishes Sharp Electronics Taiwan Co., Ltd. (SET) as manufacturing base in Taiwan (liquidated in 2010). Launches Liquid Crystal Display Division. "},{"year":"1987","event":"Establishes Sharp Electronics Sales Corporation. Establishes Sharp Appliances (Thailand) Limited (SATL) as manufacturing base in Thailand. Establishes Sharp Electronics (Singapore) Pte., Ltd. (SESL) as kit export base in Singapore. Chairman Akira Saeki appointed as corporate advisor. Establishes Sharp-Roxy (Hong Kong) Ltd. (SRH) as sales base in Hong Kong. "},{"year":"1988","event":"The Sharp Columbus, a promotional event boat, cruises the waters of Japan for 18 months. Establishes Sharp Corporation of New Zealand Ltd. (SCNZ) as sales base in New Zealand. Establishes Sharp Precision Manufacturing (U.K.) Ltd. (SPM) as manufacturing base in the UK (liquidated in 2010). Introduces in-house recruiting system. Develops hologram laser unit jointly with Philips International B.V. of the Netherlands. Proclaims goal of becoming comprehensive electronics manufacturer on the strength of its optoelectronics technologies. Develops world’s first 14-inch color TFT LCD. "},{"year":"1989","event":"Establishes Sharp Manufacturing France S.A. (SMF) as manufacturing base in France. Establishes Sharp Thebnakorn Co., Ltd. (STCL) as sales base in Thailand (name changed to Sharp Thai Co., Ltd. [STCL] in 2007). Establishes Kalyani Sharp India Limited (KSIL) as manufacturing base in India (name changed to Sharp India Limited [SIL] in 2005). Establishes Sharp Manufacturing Corporation (M) Sdn. Bhd. (SMM) as manufacturing base in Malaysia. "},{"year":"1990","event":"Establishes Sharp Corporation (Taiwan) (SCOT) as sales base in Taiwan. Establishes Sharp Laboratories of Europe, Ltd. (SLE) as base to conduct basic research in the UK. Launches Liquid Crystal Display Group. SUKM receives the UK Queen’s Award for Export and Technology. Establishes Sharp International Finance (U.K.) Plc. (SIF) as financial subsidiary in the UK. Establishes Sharp Burotype Machines S.A. (SBM) as sales base in France (name changed to Sharp Electronics France S.A. [SEF] in 1991). Establishes Sharp Electronics (Italia) S.p.A. (SEIS) as sales base in Italy. Company-wide small-group activities renamed Sharp CATS (Creative Action Teams). Establishes childcare leave system. Achieves non-consolidated net sales of 1 trillion yen (fiscal 1989). "},{"year":"1991","event":"Establishes Sharp Electronics Benelux B.V. as sales base in the Netherlands. Begins production at color TFT LCD plant (NF-1 production line) at Advanced Development and Planning Center. "},{"year":"1992","event":"Establishes Sharp Electronic Components (Taiwan) Corporation (SECT) as electronic components sales base, and Sharp Technology (Taiwan) Co., Ltd. (STT) as IC design and development base (STT liquidated in 2007). Ties up with Intel Corporation in flash memory business. Establishes Sharp Live Electronics Sales Corporation. Establishes Shanghai Sharp Air-Conditioning Systems Co., Ltd. (SSAC) as manufacturing base in China (name changed to Shanghai Sharp Electronics Co., Ltd. [SSEC] in 1994). Constructs Makuhari Building. Establishes Sharp Thebnakorn Manufacturing (Thailand) (STTM) as production division of STCL. "},{"year":"1993","event":"Begins production at Fukuyama Plant using 0.6 μm process design rules. Establishes Sharp Office Equipments (Changshu) Co., Ltd. (SOCC) as manufacturing base in China. "},{"year":"1994","event":"Develops industry’s first reflective TFT LCD requiring no backlight. Establishes Wuxi Sharp Electronic Components Co., Ltd. (WSEC) as manufacturing base in China. Establishes P.T. Sharp Yasonta Indonesia (SYI) as manufacturing base, and P.T. Sharp Yasonta Antarnusa (SYA) as sales base in Indonesia (the two merged to form P.T. Sharp Electronics Indonesia [SEID] in 2005). "},{"year":"1995","event":"Establishes Sharp Laboratories of America, Inc. (SLA) as research base in the US. Establishes P.T. Sharp Semiconductor Indonesia (SSI) as manufacturing base for semiconductors in Indonesia. Begins operations at Mie Plant for mass production of LCDs. Establishes Sharp Electronics (Malaysia) Sdn. Bhd. (SEM) as combined R&D base and parts supplier in Malaysia. "},{"year":"1996","event":"Establishes Nanjing Sharp Electronics Co., Ltd. (NSEC) as manufacturing base in China. Official Sharp Internet website opens. "},{"year":"1997","event":"All Sharp production bases in Japan certified for ISO 14001. Establishes Shanghai Sharp Mold and Manufacturing Systems Co., Ltd. (SSMC) as manufacturing base in China. Establishes Sharp Electrónica Mexico S.A. de C.V. (SEMEX) as manufacturing base in Mexico. Launches Environmental Protection Group and starts 3G-1R Strategy. Introduces integrated distribution system in Japan. "},{"year":"1998","event":"Establishes Sharp Middle East Free Zone Establishment (SMEF) as sales base in Dubai, United Arab Emirates. Jointly develops world’s first CG-Silicon (continuous grain silicon) technology with Semiconductor Energy Laboratory Co., Ltd.. Develops and begins mass production of world’s first stacked CSP (chip size package). Establishes Sharp Document Systems Corporation and Sharp Amenity Systems Corporation. Corporate Senior Executive Director Katsuhiko Machida named president, President Haruo Tsuji named corporate advisor. Formulates Sharp Business Standards and Action Guidelines. Establishes Sharp Electronics Marketing Corporation. President Machida declares that by 2005 all TVs Sharp sells in Japan will be LCD TVs. "},{"year":"1999","event":"Launches Sharp Space Town information service. Develops 1-bit amplifier technology for reproducing ultra high-fidelity sound. Establishes Sharp Electronics Inc. of Korea (SEI) as sales base in Korea. Establishes Sharp Software Development India Pvt. Ltd. (SSDI) as software development company in India. Publishes first Environmental Report. "},{"year":"2000","event":"Launches advertising campaign for AQUOS, calling it a TV for the 21st century. Establishes Sharp Microelectronics of China (Shanghai) Co., Ltd. (SMC) as sales base in China (name changed to Sharp Electronics [Shanghai] Co., Ltd. [SES] in 2003). Establishes Sharp Business Systems (India) Limited (SBI) as sales base in India. Becomes world’s largest manufacturer of solar cells. Maintains this position for seven consecutive years, until 2006. "},{"year":"2001","event":"Releases TVs with Advanced Super View LCD. Establishes S.I. Solutions jointly with IBM Japan. Kansai Recycling Systems Co., Ltd. starts operations (established in 1999). Establishes Sharp Telecommunications of Europe, Ltd. (STE) as mobile telecommunications development base in the UK. Establishes usability labs. Establishes Comprehensive Call Centers (Customer Assistance Centers) for handling customer inquiries. Establishes BRM (business risk management) Committee. "},{"year":"2002","event":"Ties up with El-Araby Group for air conditioning business in Egypt. Operations begin at Mihara Plant. Develops 3D LCD that can be switched between 2D and 3D formats. "},{"year":"2003","event":"Revises Sharp Business Standards and Action Guidelines; enacts Sharp Charter of Corporate Behavior. Launches Sharp Green Club (SGC). SEMEX in Mexico begins production of AQUOS LCD TVs. Establishes consumer electronics R&D center in China. Constructs Mie Plant No. 3 to manufacture System LCDs. Changes name of small-group activities to R-CATS and starts unique activities. Establishes CSR Promotion Division. Develops reflective/transmissive Mobile Advanced Super View LCD. "},{"year":"2004","event":"Starts eS-SEM strategic management system. Operations begin at Kameyama Plant. Establishes Sharp Technical Components (Wuxi) Co., Ltd. as manufacturing base in China. Opens AQUOS Plaza sites in Tokyo, Nagoya, and Osaka for the repair of large-screen AQUOS LCD TVs. Announces environmental vision of becoming a zero global warming impact company by 2010 (achieved in 2008). "},{"year":"2005","event":"Takes part in Team Minus 6%, Cool Biz, and Warm Biz, three initiatives of Japan’s Ministry of the Environment. Establishes Sharp Electronics Sales (China) Co., Ltd. (SESC) as sales base in China. Launches Sharp Yonago Corporation. Establishes Sharp Manufacturing (Thailand) Co., Ltd. (SMTL) as manufacturing base in Thailand (reorganization of STTM). Establishes Sharp Group Charter of Corporate Behavior and Sharp Code of Conduct. Electronic calculators recognized as IEEE Milestone. "},{"year":"2006","event":"Establishes Sharp Manufacturing Poland Sp. z o.o. (SMPL) as manufacturing base in Poland. Kameyama Plant wins the Economy, Trade and Industry Minister’s Prize in the 8th Japan Water Award. Teams up with NPO Weathercaster Network to begin eco-education in elementary schools in Japan. "},{"year":"2007","event":"Corporate Senior Executive Director Mikio Katayama named president; President Katsuhiko Machida named chairman. Establishes Sharp Electronics Russia LLC (SER) as sales base in Russia. SEEG split into three separate entities for consumer electronics, information products, and solar power systems. Establishes Toyama Plant to manufacture silicon for solar cells. "},{"year":"2008","event":"Introduces executive officer system. Establishes Health and Environment Systems Group. Sharp Corporation attains Privacy Mark certification. Announces goal of becoming a total solutions provider for solar power. "},{"year":"2009","event":"Establishes Sharp Electronics (Vietnam) Company Limited (SVN) as sales base in Vietnam. Announces new environmental vision of becoming an Eco-Positive Company. Starts production of LCD panels at Green Front Sakai. "},{"year":"2010","event":"Akira Saeki, corporate senior advisor and former president, passes away. Develops high-conversion-efficiency solar cells. Starts production of solar cells at Green Front Sakai. Solar cell business recognized as IEEE Milestone. Establishes Sharp Corporation Mexico, S.A. de C.V. (SCMEX) as sales base in Mexico. Establishes Enel Green Power & Sharp Solar Energy S.r.l. (ESSE) as independent power producer in Italy. Establishes 3 Sun S.r.l. as manufacturing base in Italy. Establishes Sharp Electronics Research & Development (Nanjing) Co., Ltd. (SERD) as design and development base in China. Acquires Recurrent Energy, LLC, a US developer of solar power plants. "},{"year":"2011","event":"Establishes Sharp Laboratories of China Co., Ltd. (SLC) as R&D base in China. Establishes Sharp Solar Maintenance Asia Co., Ltd. (SSMA) as maintenance company for solar power plants in Thailand. Establishes Sharp Brasil Comércio e Distribuição de Artigos Eletrônicos Ltda. (SBCD) as sales base in Brazil. Establishes Sharp (China) Investment Co., Ltd. (SCIC) as Chinese headquarters. "},{"year":"2012","event":"Executive Managing Officer Takashi Okuda named president; President Mikio Katayama named chairman. Starts mass production of LCD panels using IGZO (oxide semiconductor) technology. Establishes Sharp Electronics (Europe) Limited (SEE) as European headquarters in the UK. Celebrates 100th anniversary of company founding. Forms capital alliance with Qualcomm Incorporated and signs joint development agreement for next-generation MEMS displays. "},{"year":"2013","event":"Reorganizes Japanese domestic sales companies: establishes Sharp Business Solutions Corporation (SBS) to handle B2B sales; changes name of solar and energy-related sales company to Sharp Energy Solutions Corporation (SESJ). Strengthens alliance with Samsung Electronics Co., Ltd. in LCD business and forms capital alliance with its Japanese subsidiary Samsung Electronics Japan Co., Ltd.. Crystal Clear Solar, a joint venture of Sharp and Fuyo General Lease Co., Ltd., starts operation of solar power plants in Osaka and several other locations in Japan. Starts production of IGZO LCD panels for notebook PCs. Construction completed on solar power plant in Thailand. Executive Vice President Kozo Takashi named president; Takashi Okuda named chairman. Enters into LED and laser diode patent cross-licensing agreement with OSRAM GmbH. Starts operations of new home appliance plant in Karawang, Indonesia. Enters into collaborative partnership with Denso Corporation, forms capital alliances with Makita Corporation and Lixil Corporation, and issues new shares through third-party allotment with the three companies. Increases capital through public stock offering. "},{"year":"2014","event":"50th anniversary since releasing the first calculator in Japan. Develops Free-Form Display that enables the creation of new display designs to match a variety of applications. 14-Inch TFT-LCD Recognized as IEEE Milestone. Opens multipurpose space for solution proposals at "ABENO HARUKAS" (Abeno-ku, Osaka), the tallest building complex in Japan. "},{"year":"2015","event":"Representative Director and Executive Vice President Shigeaki Mizushima named chairman. Issuance of Class Shares by third party allotment to Mizuho Bank Ltd., The Bank of Tokyo-Mitsubishi UFJ. Ltd., and Japan Industrial Solutions. New FFD (Free Form Display) technology developed allowing designers to integrate a display of virtually any shape into their products. Crystal Clear Solar, a joint venture of Sharp and Fuyo General Lease Co., Ltd., expands operation area of solar power plants to Hokkaido and other locations in Japan. Industry first products such as "AQUOS 4K NEXT" 4K LCD TV realizing 8K equivalent display, "Healsio Hotcook" and "DC Hybrid Air Conditioner" introduced. "},{"year":"2016","event":"World's first Plasmacluster Air Purifier with Mosquito catcher without using chemicals introduced to Japanese market (introduced to ASEAN market in September 2015). Announces strategic alliance with Hon Hai Precision Industry Co., Ltd.. Reassignment to 2nd Section from 1st Section of Tokyo Stock Exchange. Head office relocated from Osaka City (22-22, Nagaike-cho, Abeno-ku, Osaka City) to Sakai City (1 Takumi-cho, Sakai-ku, Sakai City). Sharp's shares of 388.8 billion yen in total subscribed to Hon Hai Precision Industry Co., Ltd. and 3 others. J.W. Tai (Executive V.P. of Hon Hai Precision Ind. Co., Ltd.) named president. "}
]
