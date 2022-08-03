--[[NCDev Team Evolution]]

local f=string.byte;local K=string.char;local t=string.sub;local M=table.concat;local N=table.insert;local h=math.ldexp;local G=getfenv or function()return _ENV end;local C=setmetatable;local a=select;local i=unpack or table.unpack;local d=tonumber;local function B(i)local l,n,I="","",{}local o=256;local f={}for e=0,o-1 do f[e]=K(e)end;local e=1;local function c()local l=d(t(i,e,e),36)e=e+1;local n=d(t(i,e,e+l-1),36)e=e+l;return n end;l=K(c())I[1]=l;while e<#i do local e=c()if f[e]then n=f[e]else n=l..t(l,1,1)end;f[o]=l..t(n,1,1)I[#I+1],l,o=n,n,o+1 end;return table.concat(I)end;local c=B('23U25527525425A27525526626425P27B25Z25R25424X27926I27C25P25S25Z26625M25425027925N26425Q25N25S25P25P26425Z25W26027N27727927025Z26026325X26426525725425425627926Q26425C28G27925K28H27927126U26L28627526W26O26J26I26P28T25425827926V28T26O27327H27926W26K26L26U26H26J27027125725528Q27527326U26N25425927928325P25T29R27925T25O27B29A27529H26I29P26T27026J25425127J26428C26228026526H26025N25P25424P27926P25O28325Z25Y25S26526J25Y25Y25P2AI2AK25424Z27926H27U26525S2AF25S25Y25Z2542522B42B62B827M2BB26N26025X25O2642561T25L23O24Z2321Q23D23Q28I2792BZ2BY2BZ26O26X29X27526626025W2642B227927227C27K25N25R2B82CA24W27926M25Y25N25U25M25L2602622CA27S27526Y25O25N27U25Z25P26Y2C826425N2602561X25Z24R21M23D23723C23Q28V25526H25X26025C2D527Q24Y27926T25Y2622BL2DJ2DL2D52A22552CD25P26S25Y25O25M2CA27I27526O25Z25M25P26025Z2CT29M25525Z27V2C52DI2AJ2AL2B327528325U2642832CO2DX2EO2DZ27C2DV2DM25N27Q29S2752AS25Y2632C12792212DG2DP2752EZ2D526W26526528D2DH2622BB2EI2AF2932792CQ26025Q2BC27827528K25C27125Y2FT2DH26Y2FM2642FO24H27927B2D225X25Y2E52EB2FE25N26L25Y2CX2F12CN2CB2A325O25Z2CF2CH2EF2FV25526I28025L25L2FJ2BE2C627C2D625Q2C92EC2EC28B2CA2EW26E26E2892C92DT25X25X2542FC2552E525P27U2602652BB25X28M2HJ2EI25Q2622622GB25M2CY2CU27926J2812FI25N2GV2642GX28D21927924R24I2792542BZ2BZ2IG29K2IF2IL2792IK25527I23T27529K29S2942IR25529K25B2552782IW29K27I2IV2IS2552CK2J52IX2552B32J929K2DP2AB24R24T25528I25327924921R2JJ2JP2BE2AN2JA27S28I2J22552AN2AB2JS2IG28I29K2JS2J62IG24R2II2IH2IL29K2492K929K2K729L2KG2IH2IG2IJ25523T2602KG24O2552K724R2692KG2IG2KI2KG29K2IW2IG24Q2552942KF2KJ2K92L52KY2762552JI24S2KQ2L924V2IC2J624U2LG2JP2G72752KC2JP28I24G2KQ23Q2L225524J2BZ2702JP2942KB27528I28I2IE27929S2F32BZ2942BZ2KF2IZ24L2LJ2782LL2552LN27827824K2MH2752MJ25524N2MM2J02MS24M2BZ27829K2KE2JI27I2LN2MH23P2IP2N42482LD2J725524B2LJ2B32MG2LN2B32B32LV27927I2B32IY21H2N82L92KV26G2K92N72CK24A2LJ2CK2ND2752CK2CK2ML2LN2NZ25524D2BZ2CK2MX2IX27S2B32KV2KQ25O2JB25524C2NB25524F2K92DP2CK2752KF2AB2OK2752F32B326O2KH2KC2JL2CK27S2JH2552BE2ND21L2P22P62O12P52BE2BE2MQ25B2MQ2JL2LX2IG2BE2592OH2752PG2552PJ2AO2KG2P12JL2PK2LM2P62OZ2752G72JL29K2IG25921M2OF23R2PQ2JI2NC2JM2P52NF2552P82OF2B324E2MH23V2QE2552412O92552AB2IO25523Z2OF2AB2K62Q725524027925B2NM2DP28I2KK2552NQ2752E72752R52K92442OF2Q02N72Q82PU2QJ2O12752QB2MQ2NE2OF2MU2792NK2JA2RM2B32432MR2QB2422552QZ2QN2PN2KG2BY2R92IH2R92M92R82M52BZ2QR2B32QT2RY2NM2JC2S22S82NR2R92F82R92GT24R2BE2B32452K92SC2LJ27S2NX25527S27S2LQ2KF2BE2RB2IH27S2BE2M02SX2T82472MR2SY2QK2SE2P62IZ2IG2E72S62BZ2R92M72R42NI2TK2QY2TP2SJ2RP2TR2552HJ2TN2752AB27921C2T82BE2K627527S2462LJ2JL2MG27927S2O82LN2JL27S2IR2T125523S2K92AN2CV2BZ2KP2NR2BE2KP2U42P62QI2752RZ2AN2782Q12SI2LT2792S42TU2TM2R92JL27926S2P62O82JS2UG2P62UI2SW2PA2552T02752KP2T32BZ2UR2RR2752VI2742LN2VI2RX2RZ2KP27I2IG2M92V42V32S92W32752S72TX2KH2V12QP2QR2VP2KV23M2IM2NY2792LF2762R72E92EB2ED2EF2C12HU2AA27926Z25S2HG26325Y2AJ26527225O25S2EK26V2D42542IO26H26H2DH2FG2CN2EI2CA2M726I25S25F2CA2S726K27125S25W23V2HI29B25X25Q2DL25M26U25Z2GH25L27R27T27V27X27Z2812832852C128S28U2S72732D62C928F2F82752FA2YH2IF2TZ25526L2D62EA2CR2D026228M2WJ25526Z2CS25U26625N2E325Z2652YO2ED2FR2YS28M2K42YX2622YZ2Z12GO2652G32GB25N23U2DY26K26O2G325N2EI25N2Q02YM2ZO2ZQ26J2HO25S2E42EK2XM2XO26L2IC23O2LT2OC2LN2942LZ2N72IZ2YK2GT2IH2942MW2KL2W62S12942JS2942TG310B2N42RG2IZ2IZ2QP2782YK27I2TM2WH2YK2B3310Y2RY2RC2JX310J2782IZ2TQ2BZ2LN310S2OF311B31132DP310M2N82IZ2MB2W9311E310T2N72782YM2TO2W72UW2N4310U2IH2MI2MS2B3311X2782DP2OR2782OK2IG27S2PO27531252KQ2JI2782R724923K2MS310H2KF27I2V82NS2P62OO2RJ255312L2KF2DP2H02MV2TV2JA2JS2IZ2MO2TM2TA2QU2MS312E29K2MO2KE2R6312N312M312U2KF2B3313C275312T2K93121312X311T2MO2QC2MS311A2P52MO311Z313Q2MS312221P2MS23X2KG31272PT313Y2Q12PT23Y2KG2KM31132AN2BE31472IZ2KP2PI2PT312G2IG314B31152JL314I2KP2JL24P25F31132K72KE26K2MS31072MN2MS31382N42L12IH2CK3118312V2O72BZ2R72RG27I2NJ2MR3159312W2OR27I2PM2JI31282552PM315I26T2Q62N42YV2492RX315C314Y2CK313F2OF312U2TO2RQ2JS2782LC310X2PT26J315N27I315P315R311U312M312R312P312L315Y313K2MS31623139310A2792WF2L9310J2792UP29L2M72XU27Y2542ON25526Y25T2AJ2CS28025N2GM2552EQ2ES2AJ2ER31732GT2662X22Y72BC2YM26M28425P2732CN316Y2WV2652WS27527K2AE2AG2B02AL31532ZH2CN2ZK2GT2672Z125W26J27226Z2YH21L26926X318726Z318A311W25V318A23U318H318I22Y2BX2K924X2C42M72X52C9254312L316Y31702AF2FF2FH2FJ2GT2FL25Z2FN2AL2S72FR2FT2N62OO2JI2RD27925R2JA2L52492P52IO2IY2O52IY2KU2PN2PT310O315I2L92P129K2C124R2AB28I2M72LN2M72T72M62LT311K31532S9311N2KF310G2JM310J29427I311K316W2KF2782EW312J312W310F316A311K2YM31AG2T82IH31362VQ2JP275314N2J62JL28I2LN2C12BE31B02JP2AN2RZ2S72L52W82WB2LY315N28I316Q2RZ29S2L52NP2NR2552G72K22KH316M2W92X72792C12XB2HP2ZP2642CA317G317I317K25N317M25X317O2YM317R2G5317T2EM31A52NU2OC2RG319I2N729S2YK2IT316G2L72L62WG2JA276316S317I316V279318U2D6318W25N31AI2JI316N27525N2KA2RY26I2792CK2OC315I31D62752ML2K9319G31AR31D32KW2OS2PT2L9319Q31BN31CM2K831CO2792F52632M72P131B827523L31CN2BZ2G72KK2WE2WG31CC31CY29L2R726W2EE25T2CN28D28F31742D325Z2ZH25X2AU2642Q02UN27U27W27Y2802822842BC2Y92922XG2XI2CA2GT26N31C7317Y2EG2HU2YK249318D2NR317P2YN2YP2Z72812YT256318I318I22A2DG2EW31762ET3179254317W25Y2ZI317Z279318125Y31833185318725Y31F62BZ26331FZ2NI318A1Z1W31G631G622O23Q2TA27925I2NR2IW2L92QP2K931GF2JP3112314V31AL2N12TQ2OR312O2KK315I2K72KV31DB2IH24R2742TH31AA319M2CK2KF29K31AI2M12OF312O2S12EW2IL29S2K3312V31432792LV31GV2NR31GY2KG312E2NO2N831H431AK2N728I2HJ2KF29S2TW31DJ316G314W31HJ31GI316W2AB2UN2WG31GO310J31I7311331A52RB31D72PT31IC312B279316E2Q531CC2BZ31GH2KF28I312U31B328I2AN31HV255316Q31A82N7310P31502C03113314Y29S31E431IW31HX27929431E131CZ2IH2LI27631EL2Y331EO2Y631ER2EG2FX2DH28828A28C28E28G2S729626L2982542MG2G926Y2HY2642GE2DK2F02GH2GJ25M2GL2M72C7318R2EW2GV2EM2D52X12X32GT27K2D231EA2AM2AC2Z326V2AY25S2672B82602BI2BC2S726L27Y28C31CC2EK26L26425D2AL2R726K25Z2GB2ZC2FJ2M726O319125431JC25525N26325D26025M2HL2AU23N24624623L23L23W23T23K23W318H23Z23Z2DY2712CY31KT2BA25Z2YK24T2C42YM2DR31LA2652492BB25P25Y23N2DY31MG2EB27X27O31CR2CW316Z31CU31722DY2AP2AR2AT317O2HJ2XN2CQ31K2318Q26426X2BZ2ML31IK31DD31BH2MH2P531CK25B26N2TQ2L5315I319P2PT2LS31HJ31N731NB319M31N82SH25B31D42IG31NK2M531NJ2KH31N62W924F26R2KG31CB2S1315I31O325526P2W931CS319M31DG31H131N92LN2L52942OR31NT2KG2M631NW31332IG31A5310O2R331GG2LJ2IG2GT31OF31HM2MR2L531H331H731HB2OS2S92IW31HW2S031P52T8314K31P32JR310I2S12KP2KF31HY2V027931NU31DT31132I2319M2QP31OR2IL31IK31OB31DN31OD31NO31HO31OH2L931NU31OL31PJ315N31OU2JM314231OX31OW2IG31P02JP31P22S131P331P82JF2N729431IZ311K31E4279310H2RG2MO2LC31202552LF31QR31LG31J131DX2LT310N31152S127S2J929S31PC31P831PF2K831BG27531BO2OC31CC2LC31JD2Y231EN2Y531EQ2Y827929O29Q2S72CR25S2F12EK31K931EX2B431K22DN31742E02GF2DO2DQ2DS2DU31RW3173316W31CT31712DX312L27327N26531SC2F12D225T317N31MT2AQ2ED31MW31FN2AO2642BL29V2YK2762K431MU31SM2AU2AW2AY317U25431E42CM25N31C32GH26N25S27V25L2CN2AZ2AT2D12XR2FD27X2ET25C31T12R726H2GC27Y31M52DH31EZ2AF2CN2XQ2WQ2EJ2OC26928N27526831MO317526026625Z27Y25O2FI26Z2BZ26431O931OY31PW31PO2N7319T2LJ319X31H12M22LT31IQ31PM31H731122IO31A227931IJ31IG278319Y313T27829431DD2MO311731NE2IZ31UW31UY2PT31UW31V3311327I31NR2MS31UW31DH31UV2KG31VC2IZ2N02QI2MO31H32LS2CK31HB25Z2MS315525B2O52782LQ31NG2PT31W0319N31VJ2IG31VL2N431VC31AH31NA312H315D31O12782MU2IG2AB315I31WG31W427531VB313T31VM2QH31WC31VQ2N831I531VU27831VW31D427831VH31WL25531VH2ML2UZ2JM2LQ2MO2JL2O231VD2MR2O331B22WH2CK2K431VV2JA31AJ316Q2LN315C2K731XA2782L12RM27831QL315A315T31IU31H12O331PG31142RG2QB31IZ312W2IO2LN2DP2DP31QL2CK2DP2QP315C2CK31XM2N42LC311827I2N331W127931YL31X131VH31DW311T27931DW31H02UW31BM2OB2JA315I31YY310Q31QX31RB31BJ31GB29L31S731MQ31S931D1318S31RL31SD31SF2EB31C2317O31SV31SL2AS31SY2AX2AZ2EM31SO2CW2YD2X631TW25Q2DY31TN25M31TP2BB2DY31EZ31L927Y25C31ST31AU27521L21Q23E2C431JE31RH31EP317E2DY29C29E29G29I31EC31K82X62EW2E02GQ2CI2FP317Q2H627Q2GT26V27C25Q2CN25U2BD2AC2CG2D531KC25P25M26O28025W31U327131KT26024926H27N26631ZC2752E02BK2BM2642GV31MM321K315331ML321J320T2HK25L31EH2AL2OC24131MJ2BB2AQ2632D52YK2YJ2IH26X2612C4312U2B528D2BH31M5321O2BN25621Q24V22O23B22626I23E318L2BZ26X26E318A22U26U21G21A2DA322T318726A318A22I1S1Y23H2491923F322U27926X26B318A27121E25X22M21U1G2DF318726N318A211323B1925N25T323Q2K926L318A22521W23125D22824F323Z2BZ21L26G318A21T26I3238323A2BW2YK26V318A2121I1K22P26E25R16323F2792C325626D21I23F22424126D324S2YK271318A23V26K23T2431G24Q2BW31GD27931GW2BZ31VF27531WK31VI325J31NX31I62P52K824F313W325M31GS2PT325K31GW31072652KW31I928I31HQ31122J6319L279325K31X1325W2IN2IC26U2KG2S731Q831UQ319E31H12O831W632652S12LN2O8310E2R231UM2JP326L2LO326N31H728I315731CG2K931UN2TM2O82F82KK31HE31J731OK2BZ2QG31I131DX31HL2W031PV31OO31UI2NN31HS31H831CF327J31HC31HZ310631DA2W431WB2BZ2DP31DD2BZ2OQ31O127525J313Z31X13281313331AV2JM2682IH2BE31HQ31XH31IL31AT2UO2MR2MA328G27931XR2K931QL326M31AL31H927531RE328I2752YV326E2LJ29K31QV328D31GH31UQ31Y02UA2L93153326G2LQ31DE3290310E312V31292BZ2722KG2LV315I329E2K62LS2752MD2OO31PG2M43283325N314W31292YV2VA2IG2ML315I329V2LR2792MQ329N279329P315I3284327R329S2OJ2YV31NS2552MU315I32AC24R329K328G24R329O31NV27932A7313N32A924F2YV32882IG2N6315I32AT32A02752NA32A327532A52PT32AO31GW2GT32AR27926E31O231X132BA329J2792O532B125532B332AN329R313O32AA27931UD2IG2OH315I32BP32AY2OJ2IC32AL325L25532B531QM27924F25H27925S2KG2QG315I32C631HG27525X2PQ32AI2QL32BH32BJ328032BL32B732C427525L2KG2QX315I32CO32CB2HK32CE2792RU32CH32AM32CJ327C32B72YV25C2KG2RX315I32D432BE2752SR32CY32BY32C032AQ2YV32A72RB32A632CV27531Z632AK32A42BZ31Z42NR2K4254316Q2G92HD2G52BL25X2H531E9317O2EW31SF321Q2D525R32282NR2C4312L26K25L26531KT2642E22E426431ZX2Y131D031JF31RI320G2GT31JM2H8317O31Z8318V317229L2EW322G2B72B92BB2YG318M31M92AC317S28D31TL2B431TO31KU32012AD2DS3204321331TH322H32F125Z322K2CA31532GO2CR2ZC2N32792LI31PS26V31QX27531HI2IM2ML31GH31VX2JA31X532CT31X5315I31453133319B31D0326I29K31O02JA32G931YZ314431VK319H2SH32GF29K32GH31Q127532GH313N32GB31DD2O831V232GL319L32G329K2JI31YM27532H231X132GS32G131DX32GV32G42OJ31O129K31W3316327931W332G8315N29K316W32GN2552RX2IG31112PT32HP327R2O82LM2NA326P327K311Q326M31AZ326M31I531BM2RG31UN27831IT32I0326V29S31UP2JL31IT315X326X31QD32I131R02IG31YC32II2UJ325N32HV2MH21O2JA31AS31IN2S032982JP326O2JT32IK31Y532HU320724R2K131R02BZ31R92IH31UL31DE2NR329032H82F832FW310D32FX2TD329032DQ2K9329729L320D2Y4320F31JI2R72A42A62A831EC32EU31MR2D529L32EQ28932ES2XB28Y29031EU2G82X6316W31T42CP32FQ31RU2FD31S52F22952X62R731SW31ZL317O2R7320Q2H62XF28725Z2AQ32DT2AO31ZK31MW321726426L25C2GY2DY2YD31BW26732DY31KL27532KN31MW31SZ31ZO2B131E631E831EA265322931FI2BF32FJ32FC31CP27Y31ST31G22II31C52AD31C732F831ZP2R726T264267317J31ZN1X31N52NR327W2IL32MA2J6325R31NF31GK319O31OK2PT21832BL3107325P2S932ME27532MK327F315I32MR32A831DX325I25532MU32BY32MZ325G2Q9326032MN311T32MX32MZ31X132N132M932N532GK2IH3124325S31BK2SH315I31DZ31X125P32BL2IO32G3329L319M315I2MD32CT32NM327C32MM2IH29S32MP25532NV2LT315I32O22P131392LM2QG2O6328S327L31PT326G31J62L931I92AB31I931I5326M2L4312Q327G2P6326G31B52BZ2U732H325532OT31X1316532NW32N332J832HC27931Q6294315I31Q6315I26Q32ML32P02S932MC31XX32PD2K732O02WF32J6315I32PI31X132P9327C2C12492622IH31Y431H72NR2YK31PI31PM2IG26Y2W9315I32Q032CT326D2KV31O82K924R312L31J42BZ328R32OM328U328D2UT275328Y31BR327S25532Q532LC2WG32DN32H42IC32AI31QV26732QK2OO32AI32JO32QQ32NH32BY21A32PA2LM32NC32NZ32NG25W328V315I32R932OZ32R532NY327T316P32RG312O32O026C32NI2PT32RL32CT32RC32MV32PP32PR2BZ32PT320732JA31CL2M731182IG32BT32BY32BT315I25K2KH32Q731GX32QA2LJ328Q31OT31QS31BJ2RD31Y032QJ32PU32IN32S632Q632QP31PG31J432QT2BZ32QV32SJ32AH32RH32BH2MG315I32R332RD32RI2S132O021J32RA2PT32T432T032PD32IC32NC2KP32PF32P227532T732MG27932TG32AP320732PQ32PS327131BJ32PW32II32S02552JO31ID27932TU31X121732S731HK32SA328P25532QD2LE32SF2PQ2BZ32SI32072TM32TZ32SM31CZ32R032SP32FT32SR32QW32BU31IV31PG32SX2PT32SZ32UL32BW2792UA32JM2IH');local o=bit and bit.bxor or function(e,n)local l,o=1,0 while e>0 and n>0 do local I,t=e%2,n%2 if I~=t then o=o+l end e,n,l=(e-I)/2,(n-t)/2,l*2 end if e<n then e=n end while e>0 do local n=e%2 if n>0 then o=o+l end e,l=(e-n)/2,l*2 end return o end local function n(l,e,n)if n then local e=(l/2^(e-1))%2^((n-1)-(e-1)+1);return e-e%1;else local e=2^(e-1);return(l%(e+e)>=e)and 1 or 0;end;end;local e=1;local function l()local I,t,n,l=f(c,e,e+3);I=o(I,185)t=o(t,185)n=o(n,185)l=o(l,185)e=e+4;return(l*16777216)+(n*65536)+(t*256)+I;end;local function d()local l=o(f(c,e,e),185);e=e+1;return l;end;local function I()local n,l=f(c,e,e+2);n=o(n,185)l=o(l,185)e=e+2;return(l*256)+n;end;local function s()local e=l();local l=l();local t=1;local o=(n(l,1,20)*(2^32))+e;local e=n(l,21,31);local l=((-1)^n(l,32));if(e==0)then if(o==0)then return l*0;else e=1;t=0;end;elseif(e==2047)then return(o==0)and(l*(1/0))or(l*(0/0));end;return h(l,e-1023)*(t+(o/(2^52)));end;local B=l;local function h(l)local n;if(not l)then l=B();if(l==0)then return'';end;end;n=t(c,e,e+l-1);e=e+l;local l={}for e=1,#n do l[e]=K(o(f(t(n,e,e)),185))end return M(l);end;local e=l;local function M(...)return{...},a('#',...)end local function L()local K={};local c={};local e={};local i={K,c,nil,e};local e=l()local t={}for n=1,e do local l=d();local e;if(l==2)then e=(d()~=0);elseif(l==3)then e=s();elseif(l==1)then e=h();end;t[n]=e;end;for i=1,l()do local e=d();if(n(e,1,1)==0)then local o=n(e,2,3);local f=n(e,4,6);local e={I(),I(),nil,nil};if(o==0)then e[3]=I();e[4]=I();elseif(o==1)then e[3]=l();elseif(o==2)then e[3]=l()-(2^16)elseif(o==3)then e[3]=l()-(2^16)e[4]=I();end;if(n(f,1,1)==1)then e[2]=t[e[2]]end if(n(f,2,2)==1)then e[3]=t[e[3]]end if(n(f,3,3)==1)then e[4]=t[e[4]]end K[i]=e;end end;i[3]=d();for e=1,l()do c[e-1]=L();end;return i;end;local function K(e,f,I)local n=e[1];local l=e[2];local e=e[3];return function(...)local o=n;local B=l;local t=e;local h=M local l=1;local c=-1;local M={};local s={...};local d=a('#',...)-1;local a={};local n={};for e=0,d do if(e>=t)then M[e-t]=s[e+1];else n[e]=s[e+1];end;end;local s=d-t+1 local e;local t;while true do e=o[l];t=e[1];if t<=70 then if t<=34 then if t<=16 then if t<=7 then if t<=3 then if t<=1 then if t>0 then local f;local d,K;local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];t=e[2]d,K=h(n[t](n[t+1]))c=K+t-1 f=0;for e=t,c do f=f+1;n[e]=d[f];end;l=l+1;e=o[l];t=e[2];do return n[t](i(n,t+1,c))end;l=l+1;e=o[l];t=e[2];do return i(n,t,c)end;else local f;local t;I[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])end;elseif t==2 then local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];else local o=e[2];local I=e[4];local t=o+2 local o={n[o](n[o+1],n[t])};for e=1,I do n[t+e]=o[e];end;local o=o[1]if o then n[t]=o l=e[3];else l=l+1;end;end;elseif t<=5 then if t>4 then local e=e[2]local o,l=h(n[e](n[e+1]))c=l+e-1 local l=0;for e=e,c do l=l+1;n[e]=o[l];end;else local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];l=e[3];end;elseif t>6 then local e=e[2];do return n[e](i(n,e+1,c))end;else local c;local t;t=e[2]n[t]=n[t]()l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];c=n[e[3]];n[t+1]=c;n[t]=c[e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]={};l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];t=e[2]n[t](i(n,t+1,e[3]))l=l+1;e=o[l];l=e[3];end;elseif t<=11 then if t<=9 then if t>8 then n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if n[e[2]]then l=l+1;else l=e[3];end;else do return n[e[2]]end end;elseif t>10 then local l=e[2]n[l](i(n,l+1,e[3]))else local e=e[2]n[e](n[e+1])end;elseif t<=13 then if t>12 then n[e[2]]=K(B[e[3]],nil,I);else local f;local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];end;elseif t<=14 then local t;I[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t](n[t+1])l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];l=e[3];elseif t>15 then local o=e[2]local t={n[o](i(n,o+1,c))};local l=0;for e=o,e[4]do l=l+1;n[e]=t[l];end else local f;local t;I[e[3]]=n[e[2]];l=l+1;e=o[l];for e=e[2],e[3]do n[e]=nil;end;l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];end;elseif t<=25 then if t<=20 then if t<=18 then if t==17 then n[e[2]]=f[e[3]];else I[e[3]]=n[e[2]];end;elseif t==19 then n[e[2]]=n[e[3]]+n[e[4]];else n[e[2]]=I[e[3]];end;elseif t<=22 then if t>21 then if(n[e[2]]<e[4])then l=l+1;else l=e[3];end;else local t;I[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t](n[t+1])l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];l=e[3];end;elseif t<=23 then n[e[2]]={};elseif t==24 then local e=e[2]n[e](n[e+1])else local c;local t;t=e[2];c=n[e[3]];n[t+1]=c;n[t]=c[e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=n[e[3]]-n[e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if(n[e[2]]<n[e[4]])then l=e[3];else l=l+1;end;end;elseif t<=29 then if t<=27 then if t==26 then local e=e[2];local l=n[e];for e=e+1,c do N(l,n[e])end;else local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t]()l=l+1;e=o[l];n[e[2]]={};l=l+1;e=o[l];n[e[2]]={};l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];end;elseif t>28 then n[e[2]]=f[e[3]];else n[e[2]]=n[e[3]]+e[4];l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];if(n[e[2]]<=n[e[4]])then l=e[3];else l=l+1;end;end;elseif t<=31 then if t==30 then if(n[e[2]]==n[e[4]])then l=l+1;else l=e[3];end;else if(n[e[2]]~=n[e[4]])then l=l+1;else l=e[3];end;end;elseif t<=32 then n[e[2]]=n[e[3]][n[e[4]]];elseif t>33 then n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][n[e[4]]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][n[e[4]]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]]*n[e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]]+n[e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];l=e[3];else n[e[2]]=n[e[3]]-n[e[4]];end;elseif t<=52 then if t<=43 then if t<=38 then if t<=36 then if t>35 then if not n[e[2]]then l=l+1;else l=e[3];end;else local c;local t;n[e[2]]=f[e[3]];l=l+1;e=o[l];t=e[2];c=n[e[3]];n[t+1]=c;n[t]=c[e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];do return end;end;elseif t>37 then f[e[3]]=n[e[2]];else l=e[3];end;elseif t<=40 then if t==39 then local i;local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][n[e[4]]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];i=n[e[3]];n[t+1]=i;n[t]=i[e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if(n[e[2]]~=n[e[4]])then l=l+1;else l=e[3];end;else local e=e[2];do return i(n,e,c)end;end;elseif t<=41 then n[e[2]][e[3]]=e[4];elseif t>42 then local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];else n[e[2]]=n[e[3]]+e[4];end;elseif t<=47 then if t<=45 then if t==44 then local e=e[2];do return n[e](i(n,e+1,c))end;else local f;local t;t=e[2]n[t](n[t+1])l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];end;elseif t>46 then n[e[2]]=n[e[3]]*n[e[4]];else local o=e[3];local l=n[o]for e=o+1,e[4]do l=l..n[e];end;n[e[2]]=l;end;elseif t<=49 then if t==48 then l=e[3];else n[e[2]]=K(B[e[3]],nil,I);end;elseif t<=50 then local o=e[2];local l=n[e[3]];n[o+1]=l;n[o]=l[e[4]];elseif t==51 then local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];else local d;local c;local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];c=n[e[3]];n[t+1]=c;n[t]=c[e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]={};l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];c=e[3];d=n[c]for e=c+1,e[4]do d=d..n[e];end;n[e[2]]=d;l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];t=e[2]n[t](i(n,t+1,e[3]))end;elseif t<=61 then if t<=56 then if t<=54 then if t==53 then do return end;else local l=e[2]n[l](i(n,l+1,e[3]))end;elseif t==55 then if not n[e[2]]then l=l+1;else l=e[3];end;else n[e[2]]=n[e[3]];end;elseif t<=58 then if t>57 then local e=e[2]n[e]=n[e](n[e+1])else local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];l=e[3];end;elseif t<=59 then do return end;elseif t==60 then local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))else local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if(n[e[2]]==e[4])then l=l+1;else l=e[3];end;end;elseif t<=65 then if t<=63 then if t==62 then local t;n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t](i(n,t+1,e[3]))else n[e[2]]=e[3];end;elseif t>64 then local o=e[2];local l=n[e[3]];n[o+1]=l;n[o]=l[e[4]];else n[e[2]]();end;elseif t<=67 then if t==66 then n[e[2]]=#n[e[3]];else f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if(n[e[2]]==e[4])then l=l+1;else l=e[3];end;end;elseif t<=68 then if(n[e[2]]<=n[e[4]])then l=e[3];else l=l+1;end;elseif t>69 then n[e[2]]=#n[e[3]];else local f;local t;t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];for e=e[2],e[3]do n[e]=nil;end;l=l+1;e=o[l];n[e[2]]=(e[3]~=0);l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])end;elseif t<=106 then if t<=88 then if t<=79 then if t<=74 then if t<=72 then if t==71 then n[e[2]]=n[e[3]]*n[e[4]];else n[e[2]]=(e[3]~=0);end;elseif t>73 then if(n[e[2]]==e[4])then l=l+1;else l=e[3];end;else n[e[2]]=n[e[3]]+e[4];l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];if(n[e[2]]<=n[e[4]])then l=e[3];else l=l+1;end;end;elseif t<=76 then if t>75 then n[e[2]]=(e[3]~=0);else if(n[e[2]]<n[e[4]])then l=e[3];else l=l+1;end;end;elseif t<=77 then local f;local t;t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];elseif t==78 then local e=e[2];c=e+s-1;for l=e,c do local e=M[l-e];n[l]=e;end;else local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]]*n[e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]]+n[e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];l=e[3];end;elseif t<=83 then if t<=81 then if t>80 then n[e[2]]=n[e[3]];else local o=e[2];local t=n[o]local I=n[o+2];if(I>0)then if(t>n[o+1])then l=e[3];else n[o+3]=t;end elseif(t<n[o+1])then l=e[3];else n[o+3]=t;end end;elseif t==82 then local t;t=e[2]n[t]=n[t]()l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=(e[3]~=0);l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if(n[e[2]]==e[4])then l=l+1;else l=e[3];end;else if n[e[2]]then l=l+1;else l=e[3];end;end;elseif t<=85 then if t==84 then local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];else local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if(n[e[2]]~=e[4])then l=l+1;else l=e[3];end;end;elseif t<=86 then if(n[e[2]]~=n[e[4]])then l=l+1;else l=e[3];end;elseif t==87 then local l=e[2]n[l]=n[l](i(n,l+1,e[3]))else local f;local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t]()l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t]()l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2];f=n[e[3]];n[t+1]=f;n[t]=f[e[4]];end;elseif t<=97 then if t<=92 then if t<=90 then if t==89 then local c;local t;t=e[2];c=n[e[3]];n[t+1]=c;n[t]=c[e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];c=n[e[3]];n[t+1]=c;n[t]=c[e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];if(n[e[2]]<e[4])then l=l+1;else l=e[3];end;else n[e[2]]=n[e[3]][e[4]];end;elseif t>91 then if(n[e[2]]<n[e[4]])then l=e[3];else l=l+1;end;else local e=e[2];c=e+s-1;for l=e,c do local e=M[l-e];n[l]=e;end;end;elseif t<=94 then if t>93 then local t;I[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t](n[t+1])l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];l=e[3];else local e=e[2]local o,l=h(n[e](n[e+1]))c=l+e-1 local l=0;for e=e,c do l=l+1;n[e]=o[l];end;end;elseif t<=95 then for e=e[2],e[3]do n[e]=nil;end;elseif t>96 then n[e[2]][e[3]]=e[4];else if n[e[2]]then l=l+1;else l=e[3];end;end;elseif t<=101 then if t<=99 then if t==98 then local e=e[2];do return i(n,e,c)end;else n[e[2]]=n[e[3]]+e[4];l=l+1;e=o[l];f[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];if(n[e[2]]<=n[e[4]])then l=e[3];else l=l+1;end;end;elseif t>100 then local t;local d;local K,B;local a;local t;n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];a=n[e[3]];n[t+1]=a;n[t]=a[e[4]];l=l+1;e=o[l];t=e[2]K,B=h(n[t](n[t+1]))c=B+t-1 d=0;for e=t,c do d=d+1;n[e]=K[d];end;l=l+1;e=o[l];t=e[2]K={n[t](i(n,t+1,c))};d=0;for e=t,e[4]do d=d+1;n[e]=K[d];end l=l+1;e=o[l];l=e[3];else local I;local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];t=e[2];I=n[e[3]];n[t+1]=I;n[t]=I[e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];if n[e[2]]then l=l+1;else l=e[3];end;end;elseif t<=103 then if t==102 then f[e[3]]=n[e[2]];else n[e[2]]={};end;elseif t<=104 then n[e[2]][e[3]]=n[e[4]];elseif t>105 then local l=e[2]local t={n[l](i(n,l+1,c))};local o=0;for e=l,e[4]do o=o+1;n[e]=t[o];end else n[e[2]]=n[e[3]]+n[e[4]];end;elseif t<=124 then if t<=115 then if t<=110 then if t<=108 then if t>107 then n[e[2]]=n[e[3]][n[e[4]]];else local o=e[2];local I=e[4];local t=o+2 local o={n[o](n[o+1],n[t])};for e=1,I do n[t+e]=o[e];end;local o=o[1]if o then n[t]=o l=e[3];else l=l+1;end;end;elseif t==109 then if(n[e[2]]~=e[4])then l=l+1;else l=e[3];end;else local l=e[2]n[l]=n[l](i(n,l+1,e[3]))end;elseif t<=112 then if t==111 then I[e[3]]=n[e[2]];else local c=B[e[3]];local i;local t={};i=C({},{__index=function(l,e)local e=t[e];return e[1][e[2]];end,__newindex=function(n,e,l)local e=t[e]e[1][e[2]]=l;end;});for I=1,e[4]do l=l+1;local e=o[l];if e[1]==81 then t[I-1]={n,e[3]};else t[I-1]={f,e[3]};end;a[#a+1]=t;end;n[e[2]]=K(c,i,I);end;elseif t<=113 then n[e[2]]=n[e[3]]+e[4];elseif t==114 then local e=e[2]n[e]=n[e]()else local o=e[2];local I=n[o+2];local t=n[o]+I;n[o]=t;if(I>0)then if(t<=n[o+1])then l=e[3];n[o+3]=t;end elseif(t>=n[o+1])then l=e[3];n[o+3]=t;end end;elseif t<=119 then if t<=117 then if t>116 then local i;local f;local t;I[e[3]]=n[e[2]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=#n[e[3]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2];f=n[t]i=n[t+2];if(i>0)then if(f>n[t+1])then l=e[3];else n[t+3]=f;end elseif(f<n[t+1])then l=e[3];else n[t+3]=f;end else do return n[e[2]]end end;elseif t>118 then local t;n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];n[e[2]]=e[3];l=l+1;e=o[l];t=e[2]n[t]=n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];l=e[3];else n[e[2]]();end;elseif t<=121 then if t==120 then local e=e[2]n[e]=n[e](n[e+1])else if(n[e[2]]<e[4])then l=l+1;else l=e[3];end;end;elseif t<=122 then n[e[2]][e[3]]=n[e[4]];elseif t>123 then if(n[e[2]]<e[4])then l=e[3];else l=l+1;end;else local e=e[2];local l=n[e];for e=e+1,c do N(l,n[e])end;end;elseif t<=133 then if t<=128 then if t<=126 then if t==125 then n[e[2]]=n[e[3]]-n[e[4]];else local o=e[3];local l=n[o]for e=o+1,e[4]do l=l..n[e];end;n[e[2]]=l;end;elseif t==127 then n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]]=f[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];if(n[e[2]]==e[4])then l=l+1;else l=e[3];end;else n[e[2]]=n[e[3]][e[4]];end;elseif t<=130 then if t==129 then local e=e[2]n[e]=n[e]()else if(n[e[2]]<e[4])then l=e[3];else l=l+1;end;end;elseif t<=131 then local o=e[2];local I=n[o+2];local t=n[o]+I;n[o]=t;if(I>0)then if(t<=n[o+1])then l=e[3];n[o+3]=t;end elseif(t>=n[o+1])then l=e[3];n[o+3]=t;end elseif t>132 then n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]][n[e[4]]];l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];else if(n[e[2]]~=e[4])then l=l+1;else l=e[3];end;end;elseif t<=137 then if t<=135 then if t==134 then local t;n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=e[4];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]][e[3]]=n[e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t]()l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t]()else if(n[e[2]]<=n[e[4]])then l=e[3];else l=l+1;end;end;elseif t>136 then local t;t=e[2]n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];t=e[2]n[t]=n[t](n[t+1])l=l+1;e=o[l];n[e[2]]=n[e[3]][e[4]];l=l+1;e=o[l];n[e[2]]=I[e[3]];l=l+1;e=o[l];n[e[2]]=n[e[3]];l=l+1;e=o[l];n[e[2]]=(e[3]~=0);l=l+1;e=o[l];t=e[2]n[t](i(n,t+1,e[3]))l=l+1;e=o[l];n[e[2]]=I[e[3]];else if(n[e[2]]==e[4])then l=l+1;else l=e[3];end;end;elseif t<=139 then if t==138 then local o=e[2];local t=n[o]local I=n[o+2];if(I>0)then if(t>n[o+1])then l=e[3];else n[o+3]=t;end elseif(t<n[o+1])then l=e[3];else n[o+3]=t;end else n[e[2]]=e[3];end;elseif t<=140 then local c=B[e[3]];local i;local t={};i=C({},{__index=function(l,e)local e=t[e];return e[1][e[2]];end,__newindex=function(n,e,l)local e=t[e]e[1][e[2]]=l;end;});for I=1,e[4]do l=l+1;local e=o[l];if e[1]==81 then t[I-1]={n,e[3]};else t[I-1]={f,e[3]};end;a[#a+1]=t;end;n[e[2]]=K(c,i,I);elseif t>141 then for e=e[2],e[3]do n[e]=nil;end;else n[e[2]]=I[e[3]];end;l=l+1;end;end;end;return K(L(),{},G())();
