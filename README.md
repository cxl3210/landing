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





,1912,1914,1915,1920,1923,1924,1925,1926,1927,1929,1930,1931,1934,1935,1936,1937,1942,1943,1944,1945,1946,1948,1949,1950,1951,1952,1953,1954,1955,1956,1957,1958,1959,1960,1961,1962,1963,1964,1965,1966,1967,1968,1969,1970,1971,1972,1973,1974,1975,1976,1977,1978,1979,1980,1981,1982,1983,1985,1986,1987,1988,1989,1990,1991,1992,1993,1994,1995,1996,1997,1998,1999,2000,2001,2002,2003,2004,2005,2006,2007,2008,2009,2010,2011,2012,2013,2014,2015,2016
"Founder, Tokuji Hayakawa, invents the Tokubijo snap buckle and acquires utility model design patent,Moves to Hayashi-cho, Honjo-ku, Tokyo (now Tachikawa, Sumida-ku, Tokyo),Invents Hayakawa Mechanical Pencil and begins export to the US and Europe,Establishes branch factory in Oshiage, Tokyo (now Yahiro, Sumida-ku, Tokyo),All factories destroyed during Great Kanto Earthquake,Establishes Hayakawa Metal Works in Tanabe-cho, Higashinari-gun, Osaka Prefecture (now the location of the Head Office),Succeeds in assembling first Japan-made crystal radio set; begins mass production and sales,Begins export of radio sets and components to China, Southeast Asia, India, and South America,Holds Sharp radio trade fairs in Kyushu, Japan and Shanghai, China,Releases AC vacuum-tube radios,Hayakawa tours Hong Kong,Establishes sales agency in Hong Kong,Establishes Shanghai office,Hayakawa Metal Works Institute Co. incorporated with capital of 300,000 yen (May 1),Installs intermittent belt conveyor system,Establishes Hayakawa Commercial School for Youth,Changes company name to Hayakawa Electric Industry Co., Ltd.,Head office building completed,Establishes Hayakawa Electric branch factory,Establishes Kyoto Plant in Shimogyo-ku (now Minami-ku), Kyoto (sold in 1947),Forms labor union,Establishes Sharp Shoji,Released from special accounting company designation,Plant to employ the visually impaired incorporated as Tokusen Metal Limited Partnership,Successfully develops prototype TV set,Begins publication of Sharp News, an information magazine for retailers,Begins full-scale mass production of first Japan-made TV sets (TV3-14T),Constructs TV plant at the head office (now Tanabe Plant, Osaka) and installs endless conveyor system,Formulates in-house standards (HS: Hayakawa Standards),Spins off sales division to establish Sharp Electric Co.,Establishes Tokyo Sharp Geppan to sell Sharp products on monthly installment system; Sharp Geppan companies subsequently established nationwide,Begins publication of Mado, an in-house magazine,Begins R&D on solar cells,Constructs Yamato-koriyama Plant No. 1 (now Nara Plant),Establishes Central Research Laboratories,Establishes Sharp Electronics Corporation (SEC) in the US, the company’s first overseas sales base,Establishes service company in Osaka,Release world’s first all-transistor diode electronic desktop calculator (CS-10A) as company moves to become a comprehensive electronics manufacturer,Institutes 70 Strategy to strengthen distribution system,Releases home-use microwave oven with a turntable (R-600),Launches 55 Campaign that included Sharp technology fairs to celebrate 55th anniversary of company’s founding,Establishes Hayakawa Electric Europe GmbH (HEEG) (name changed to Sharp Electronics [Europe] GmbH [SEEG] in 1970) as sales base in West Germany,Launches MI campaign,Changes company name to Sharp Corporation,Establishes Sharp Corporation of Australia Pty. Ltd. (SCA) as sales base in Australia,Releases company’s first copier,Establishes Business Philosophy, Business Creed, and Basic Business Principles,Holds first company-wide QC circle convention,Begins mass production of color TVs at SCA in Australia,Launches New Life product strategy,Establishes Sharp System Service,Installs automated production line for the complete fabrication of calculators (awarded the Okochi Memorial Production Prize in 1981),Establishes Sharp Electronics (Svenska) AB (SES) (name changed to Sharp Electronics [Nordic] AB [SEN] in 2000) as sales base in Sweden,Announces one-trillion yen initiative,Establishes Sharp Consumer Electronics Co., Ltd.,Establishes Sharp (Phils.) Corporation (SPC) as manufacturing base in the Philippines,Establishes Sharp Engineering Corporation,Sharp Manufacturing Company of U.K. (SUKM) starts operations as production division of SUK,Builds “futuristic electric house” on the grounds of Yao Plant,Establishes Sharp Electronics Sales Corporation,The Sharp Columbus, a promotional event boat, cruises the waters of Japan for 18 months,Establishes Sharp Manufacturing France S.A. (SMF) as manufacturing base in France,Establishes Sharp Corporation (Taiwan) (SCOT) as sales base in Taiwan,Establishes Sharp Electronics Benelux B.V. as sales base in the Netherlands,Establishes Sharp Electronic Components (Taiwan) Corporation (SECT) as electronic components sales base, and Sharp Technology (Taiwan) Co., Ltd. (STT) as IC design and development base (STT liquidated in 2007),Begins production at Fukuyama Plant using 0.6 μm process design rules,Develops industry’s first reflective TFT LCD requiring no backlight,Establishes Sharp Laboratories of America, Inc. (SLA) as research base in the US,Establishes Nanjing Sharp Electronics Co., Ltd. (NSEC) as manufacturing base in China,All Sharp production bases in Japan certified for ISO 14001,Establishes Sharp Middle East Free Zone Establishment (SMEF) as sales base in Dubai, United Arab Emirates,Launches Sharp Space Town information service,Launches advertising campaign for AQUOS, calling it a TV for the 21st century,Releases TVs with Advanced Super View LCD,Ties up with El-Araby Group for air conditioning business in Egypt,Revises Sharp Business Standards and Action Guidelines; enacts Sharp Charter of Corporate Behavior,Starts eS-SEM strategic management system,Takes part in Team Minus 6%, Cool Biz, and Warm Biz, three initiatives of Japan’s Ministry of the Environment,Establishes Sharp Manufacturing Poland Sp. z o.o. (SMPL) as manufacturing base in Poland,Corporate Senior Executive Director Mikio Katayama named president; President Katsuhiko Machida named chairman,Introduces executive officer system,Establishes Sharp Electronics (Vietnam) Company Limited (SVN) as sales base in Vietnam,Akira Saeki, corporate senior advisor and former president, passes away,Establishes Sharp Laboratories of China Co., Ltd. (SLC) as R&D base in China,Executive Managing Officer Takashi Okuda named president; President Mikio Katayama named chairman,Reorganizes Japanese domestic sales companies: establishes Sharp Business Solutions Corporation (SBS) to handle B2B sales; changes name of solar and energy-related sales company to Sharp Energy Solutions Corporation (SESJ),50th anniversary since releasing the first calculator in Japan,Representative Director and Executive Vice President Shigeaki Mizushima named chairman,World's first Plasmacluster Air Purifier with Mosquito catcher without using chemicals introduced to Japanese market (introduced to ASEAN market in September 2015),"
