Write a SQL solution to output the population density (population per unit area) of all countries.

SELECT country, (CAST(REPLACE(population, ',', '')::integer AS FLOAT)/CAST(REPLACE(area, ',', '')::integer AS FLOAT))PopulationDensity FROM world WHERE REPLACE(area, ',', '')::integer >0;

"country","populationdensity"
"China",153
"India",464
"United States",36
"Indonesia",150
"Pakistan",286
"Brazil",25
"Nigeria",226
"Bangladesh",1265
"Russia",8
"Mexico",66
"Japan",346
"Ethiopia",114
"Philippines",367
"Egypt",102
"Vietnam",313
"DR Congo",39
"Turkey",109
"Iran",51
"Germany",240
"Thailand",136
"United Kingdom",280
"France",119
"Italy",205
"Tanzania",67
"South Africa",48
"Myanmar",83
"Kenya",94
"South Korea",527
"Colombia",45
"Spain",93
"Uganda",228
"Argentina",16
"Algeria",18
"Sudan",24
"Ukraine",75
"Iraq",92
"Afghanistan",59
"Poland",123
"Canada",4
"Morocco",82
"Saudi Arabia",16
"Uzbekistan",78
"Peru",25
"Angola",26
"Malaysia",98
"Mozambique",39
"Ghana",136
"Yemen",56
"Nepal",203
"Venezuela",32
"Madagascar",47
"Cameroon",56
"Côte d'Ivoire",82
"North Korea",214
"Australia",3
"Niger",19
"Taiwan",672
"Sri Lanka",341
"Burkina Faso",76
"Mali",16
"Romania",83
"Malawi",202
"Chile",25
"Kazakhstan",6
"Zambia",24
"Guatemala",167
"Ecuador",71
"Syria",95
"Netherlands",508
"Senegal",86
"Cambodia",94
"Chad",13
"Somalia",25
"Zimbabwe",38
"Guinea",53
"Rwanda",525
"Benin",107
"Burundi",463
"Tunisia",76
"Bolivia",10
"Belgium",382
"Haiti",413
"Cuba",106
"South Sudan",18
"Dominican Republic",224
"Czech Republic (Czechia)",138
"Greece",80
"Jordan",114
"Portugal",111
"Azerbaijan",122
"Sweden",24
"Honduras",88
"United Arab Emirates",118
"Hungary",106
"Tajikistan",68
"Belarus",46
"Austria",109
"Papua New Guinea",19
"Serbia",99
"Israel",399
"Switzerland",219
"Togo",152
"Sierra Leone",110
"Hong Kong",7139
"Laos",31
"Paraguay",17
"Bulgaria",64
"Libya",3
"Lebanon",667
"Nicaragua",55
"Kyrgyzstan",34
"El Salvador",313
"Turkmenistan",12
"Singapore",8357
"Denmark",136
"Finland",18
"Congo",16
"Slovakia",113
"Norway",14
"Oman",16
"State of Palestine",847
"Costa Rica",99
"Liberia",52
"Ireland",71
"Central African Republic",7
"New Zealand",18
"Mauritania",4
"Panama",58
"Kuwait",239
"Croatia",73
"Moldova",122
"Georgia",57
"Eritrea",35
"Uruguay",19
"Bosnia and Herzegovina",64
"Mongolia",2
"Armenia",104
"Jamaica",273
"Qatar",248
"Albania",105
"Puerto Rico",322
"Lithuania",43
"Namibia",3
"Gambia",238
"Botswana",4
"Gabon",8
"Lesotho",70
"North Macedonia",82
"Slovenia",103
"Guinea-Bissau",69
"Latvia",30
"Bahrain",2238
"Equatorial Guinea",50
"Trinidad and Tobago",272
"Estonia",31
"Timor-Leste",88
"Mauritius",626
"Cyprus",130
"Eswatini",67
"Djibouti",42
"Fiji",49
"Réunion",358
"Comoros",467
"Guyana",3
"Bhutan",20
"Solomon Islands",24
"Macao",21644
"Montenegro",46
"Luxembourg",241
"Western Sahara",2
"Suriname",3
"Cabo Verde",137
"Maldives",1801
"Malta",1379
"Brunei",83
"Guadeloupe",236
"Belize",17
"Bahamas",39
"Martinique",354
"Iceland",3
"Vanuatu",25
"French Guiana",3
"Barbados",668
"New Caledonia",15
"French Polynesia",76
"Mayotte",727
"Sao Tome & Principe",228
"Samoa",70
"Saint Lucia",301
"Channel Islands",915
"Guam",312
"Curaçao",369
"Kiribati",147
"Micronesia",164
"Grenada",330
"St. Vincent & Grenadines",284
"Aruba",593
"Tonga",146
"U.S. Virgin Islands",298
"Seychelles",213
"Antigua and Barbuda",222
"Isle of Man",149
"Andorra",164
"Dominica",95
"Cayman Islands",273
"Bermuda",1245
"Marshall Islands",328
"Northern Mariana Islands",125
"Greenland",0
"American Samoa",275
"Saint Kitts & Nevis",204
"Faeroe Islands",35
"Sint Maarten",1261
"Monaco",39242
"Turks and Caicos",40
"Saint Martin",729
"Liechtenstein",238
"San Marino",565
"Gibraltar",3369
"British Virgin Islands",201
"Caribbean Netherlands",79
"Palau",39
"Cook Islands",73
"Anguilla",166
"Tuvalu",393
"Wallis & Futuna",80
"Nauru",541
"Saint Barthelemy",470
"Saint Helena",15
"Saint Pierre & Miquelon",25
"Montserrat",49
"Falkland Islands",0
"Niue",6
"Tokelau",135
