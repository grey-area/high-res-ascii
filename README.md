Tool to create high resolution ascii art.

Usage: python ascii.py <image filename> <horizontal resolution>

If horizontal resolution is not specified, it defaults to the smallest of 400 and the original image horizontal resolution.

The image is downsampled, and each pixel is replaced with the printable character closest in brightness to the original pixel, after normalization. Character brightnesses were previously calculated by, for each character, producing an image containing only that character and calculating the mean pixel brightness.






<table border="0" style="background-color:#ffffff;border-collapse:collapse;border:0px solid #ffffff;color:#000000;width:100%" cellpadding="0" cellspacing="-10">

<tr>
<td><pre>HGUU08$dD8DD8#g8#)**==***====**rr)))))cLLcL[C{{{Fy{zxtxtzttfIywVypG$HUUdUUUa5ShUEEd&$p&$HUdUpUUaUU&a</pre></td></tr>
<tr><td><pre>Gap08d$8#QQgggR#&*====***==+=*))))))))cLLv7tC{{{y{fztjtztYx{F4VFwydd$$UPUGqUppUaddE$Ed$AD&GUqHUUpUdU</pre></td></tr>
<tr><td><pre>Udd$D&RRR#RRRRRR*=====***=+==<)?)))?))cLLL[tz1f{fCCCztfftY7Cyww4Vy3h$&EShpApUUAAdpaGdD&0dAHppGAPaU&0</pre></td></tr>
<tr><td><pre>UdD88RRRRRRgRgQ)======******)?*.....*......?7CCz%xxttttzxjjC{FIhI{%hdD$$UpAdGhHUUUpEddD&&$&dqqpp5UUd</pre></td></tr>
<tr><td><pre>5pDDRRRRRR#RRRR**=+===*****) .....:P.:...:...~ft7[jt[tttxL[t{{Ih3fLfhd8d&hUp$EppGUGqqU8Q$QDHEUpdpEG&</pre></td></tr>
<tr><td><pre>0A88RRRRRRRRR#****_+=*****....=:*..:.:.........~LljjxjjY[[xf{{ISV{Lv{h&8&Ep5d$$dpdAUp&Sd$$&$&dp&UppU</pre></td></tr>
<tr><td><pre>d&QRRRRWNRRRRN)*=+_+=*)*.:::?.:..,:::,:a:.:.:.: ,.1j[7Ljjtt{yywhV{jxlyUE$8dUUpE$aUpqHd&AU888$DGAH5Uq</pre></td></tr>
<tr><td><pre>d0gRRRWRWR#gRf***=++*)`.,:_L.,::::::!:.:\h^:*** .?.)t[jL7t1yyyFIh{LlL7VGE8$&pG&$&EDdUqH#pU$A$888GHUa</pre></td></tr>
<tr><td><pre>H8#RRWRWNRDRR=*<**=*).)tr.:::::__^~::~..~._...:~y ..:t7L7Yfy{{y33{Lv7cLIpA0pEGPdH$$D&$p$8pp$8p88E&E&</pre></td></tr>
<tr><td><pre>8QgRRNRRRRRRg)))***_:~:.,_.:::::::..,:~..*x::..~ ..~.~tjLYC{{fFhh{Lcllc{aGdqpUpH$$DHHEHdGd&AGDD0HAd$</pre></td></tr>
<tr><td><pre>DQRRRWNRR#RRt<))\*\::^=:~!..:::_.::.:~...)...,..!..,`.:Ll[1{{z{hh{lcc?L[GaUAahUaGH0888D&&0DA&$DA$ppd</pre></td></tr>
<tr><td><pre>8QRRRRWRRRRg*))??):;;:^:)$..)::::::::~..............^`:;Ljz1ft{hh{Lcc??j{hqGGS5aAGHH#RgR$0&88$p8$Ddd</pre></td></tr>
<tr><td><pre>8#RRRWRRRRRR))))c:__^;^::7.:_::::::::::.5h,....::..=.)::)jxtt[{4h{Lc??))fGahUUPhUUE8$QQWRR#&#8&&$gQ8</pre></td></tr>
<tr><td><pre>8gRgRRRRRRRg)))l+__=^:;:.*..::_;::;:::~.=_)~...:..~`..I^*v7[jj{V4{Lv??))lUUhSSUpGGA&8&R88RR8dD8EHHDR</pre></td></tr>
<tr><td><pre>8#RRRRRRgRRy???=^!=^::)V*:)r?::=::::::t_+:.^~..~:.. ``?___LLlL{43{Ll)???)S333UahUUdE$RQRRRRg#U#\([0-9]+?\)&$D</pre></td></tr>
<tr><td><pre>888RggRRgRR\)??C^__::R3:~:.\3c_:^:::?=.)`4;::..:::....^~::*cLL{3Vfvccl)cc{3c{UpaUqq&888RQgRRW#G88$DQ</pre></td></tr>
<tr><td><pre>08ggR#RggRR)??cz::))8.::::::_^v:$)_7...:.7L....,*:::~:.hhy+clL{3I1vcl???cL))fIhUpd&$88gRRgRQRR8pQd&D</pre></td></tr>
<tr><td><pre>&#gRRgRRgR8*))__trVP{^=_+.::...t.:~::*... )~..:::_::;,+*:_a)cL{3IzccLc??)?*)tVhSD&&$HRgRRRNRRQ8dHd&U</pre></td></tr>
<tr><td><pre>88##Q8DRRR*<):=^=t;:+_==::yl^: ).....:..:`)w:::*;::*:_I^^;++lj{3ytccfc)))))t%I5GddD8#8#gRRRRNRggH#p&</pre></td></tr>
<tr><td><pre>#8QQRR8RRD*)):__*y*_**___::_c`.),:,=;......UG:**^^_:_Ih:^^;_j[{3y%cvL?)vj))tywhAH08#gRWRR##RRR8DdH#$</pre></td></tr>
<tr><td><pre>8888Q8gQR*)))*+_*{+**_);=I+::.~5`..`.:  `..~Uy)_;;:;_)F:_;^!*j{IyYc?7??)??ltyaVGHD##WRRRRNNNRWN0$&#8</pre></td></tr>
<tr><td><pre>&8Q88D888))):==*c.===r?!!*:::.:H...... `.:.:<*+::::_*5:_____)x{3FYcc?Lcj?LfFy3UUH088#RRRRRNRWNgN$$$R</pre></td></tr>
<tr><td><pre>p$88H0p#<)?):_+*f=+**=*+c*_~::.*;.....`......)yU$AADDL:;;;_=+t{Iyjccv?cLL?L3ShGq$8D8RRRRRRNWRRRRRp$R</pre></td></tr>
<tr><td><pre>d88D$D8R))));:?hy**?1_=*;_;:..:_...,^.:.;...aL.`.,r==I+:!_=+*j{3wYct??ttj1f{hGU&$8RRRRWWWRNNRWRNR8$0</pre></td></tr>
<tr><td><pre>D8$88&Hp))c*^:*)8*?h++*+__._.::^C.:~:.... .;{{:,..l:,*y!!_;*\?{Iyj)xyctc){3Vh5AA$8#RRRRRRWRRNNRRRRHQ</pre></td></tr>
<tr><td><pre>H$8D&Hd7???=:_)L?<t)*+=_:^:.::_*c..:..:..` {=..`.`,)_:y=___=)?{Iylc[4Lf{yhPaq&pdGHRRRRRRNNNNRWNRRRQ8</pre></td></tr>
<tr><td><pre>HD#$H0&wLLl_==))la*c*!+__):: ;:?x:..~.`...3jL . ....::.t_+=*L?j{{CC{yIhhU5aGdA0D$$8Q$RRRNNNNNRNNRRRg</pre></td></tr>
<tr><td><pre>$88DD&h3{zt==r??Ldl)*+=!=_::P=U...)?)I _ j&SWRgG)))*:..?*+*)h))Y{llwfGVpD0dUH$D$D$D88QRWRNNNNNRNNg##</pre></td></tr>
<tr><td><pre>$Q8D8H53Iy{_)lv)p)&t\)=*_:^h)=)=*?+:=UyU)3=wpGhpqpp#RHRU*=<y;ULzctyIUISH8D$0D$8Q8888#Q8#RNNNNBWRRNQR</pre></td></tr>
<tr><td><pre>8888$EUVhI1rr{LV)c)c&y)*=;Fz**{gR8&DH8R?8{FtwU{h$UPhSd$V)hH)_{?ccv1hh8d&HpDH88RgRRWRRR8RRNNNNNNRRRWg</pre></td></tr>
<tr><td><pre>88#8Q&dhhhC)vt&??)L<+=gH)h{WBNR8q$EApURRNc{&RRRaG$Uhh4&pp_?=^_Lt??VpPh5dp08RggQ#RWWWRRNRWRRNWNNNQRWN</pre></td></tr>
<tr><td><pre>8#RQD8HU4hh<tt))?)**))):hqNB8H&d&NRRAa8gRD4NgRh?ChAhSVGq$RBN${v3w{yEUHUdH&&$R88QWRRRRWNRWWNNRRRNWgRW</pre></td></tr>
<tr><td><pre>8gRRQ88Ga{wAV8l?c)??r*+{?DB$UU8EaRRRRp&H$$a34{f*)3U55haGUDUNNNpwV1VD0$D&p$H8HD#RggRRRRNWNNWNNRRRNQRR</pre></td></tr>
<tr><td><pre>8RRRRR8d0ww7&LL)??)*\*:={BQdUddyv7V4{SGdHpS)\))Lh3PUS3UPqR&&Ngh*)wSa8H#gp$&&H#RggRRRRNRWNNRNNRRNNNRQ</pre></td></tr>
<tr><td><pre>8gRRRR8ApqFjIlj??x))**)[HNdqppUIc?))cyaSGhhaI3aqhhGUhPUGGp$UNU{Rd:IHRgg8D&G&DD$DRRRRWNNNNNNRRWRRNWg8</pre></td></tr>
<tr><td><pre>gRRRggQD#&htyy[Llcc)=*cFNR$0ApGU3{hFF5h3hI3{IIIyFA5UhhaUGDRERUU8$#p<~N8R$H&&Qp88#RRRWWNNNNNNRRRRgNRR</pre></td></tr>
<tr><td><pre>RRRR#g#88Ha3C8Lt?c<\==LyNRH&UGpUdhhahIIIVIFyy{yFaa4wIShqpUDHpHfV43hVh:`P8$Q8ED$8gRRNNNNNNNNNWWggQRRR</pre></td></tr>
<tr><td><pre>QgRRRR#R$$Uh{Hyyj))<**rc<D&&5aAaqwShya4w{{tIFV{IyhSUhS35aU#$UR$I{YhtwU4=+88pHH8DgNRRWNNNNNRWRRR#RRWR</pre></td></tr>
<tr><td><pre>RRRNRRR88&EawSyyt))**){1N8dAUGUSaUhhwIwtL7tYtLIVaISpUPaaqE$Q$$R$Y{{y{G3A.g&H$D$#gRRRNNNNNNWNNRRgRgRR</pre></td></tr>
<tr><td><pre>RRRRRRRRAE$d3aayCv)r*faNRQ0pAqApGF3pa[7{l%taRC3lSSdPUUVpAd8$d0gd{FL1Ip%U :&8888RRWRRNBBBBNBNRRNRRRRQ</pre></td></tr>
<tr><td><pre>#RRRRRRgQ&$$3a8htv)))LwNg$pqGpU&&G35ztGRR{l#qhpcfhaDpphq0&$D0p8dLwC{Gptwy !R888gW#RNNNNBBBNNRRWRQWQR</pre></td></tr>
<tr><td><pre>#RRRRRWR880UhPUFy)1G$NNRdAAq&qEGPV$y[1{URRpHt7jL?1U&d&UpppE$8$QSySwIhIIEy+*t8gRNgRRNNNNNNBBBNRRRRWRR</pre></td></tr>
<tr><td><pre>#RR#RRRRQDD&A4U);18RBNW#&8dpqGI$adwj=ay%yfItcv?j\LyPE&Ud&&R8#EH843ya3{3SUc=_=gWRRRNNNNNNNNBBRNRRRRRR</pre></td></tr>
<tr><td><pre>#RRRR#RRRQQ$&p#l?hHBBNRD&8HddEpGUSF)vv)*?)l)+)v)=c1hp&ppd&888DQ8hU)?hhFyI*4R#&:NgRNBNBNNNNNRNRgR88gN</pre></td></tr>
<tr><td><pre>gR#RRgRNRR#8g&QL?=NNNNR8$D0&d$&GqSt?)l)*)))*?)*_*)t{U$Udd8888#8H$7))?{{x{ypRRpj3+RNNNNBBBNNNNRWDgggR</pre></td></tr>
<tr><td><pre>#RRRRRRNWRRRR$$7)RNNWW#88$$8$&U&pIzL*<))))*)?)_+*)%yI&UE$DQRDQ88&dxL?Lxy{FH&#G)qacNNBNNBNNBNNNRRRQRR</pre></td></tr>
<tr><td><pre>ggRRRRWNWRRNW8hc)WNNRNRR88EDH8pHP3{vr+_*====<_=)*ctyh$0$&&RR#Qg8$Fq))?cLy5cfgUtI3FcWNBNBNNNNWNgWR##g</pre></td></tr>
<tr><td><pre>ggRgRgRRNNRRNN{t?BNNRWNR8D8D&HD$IVF{)*===*)+*?)*cc?L{0DdD#QR#$#8HqIUL)y&8yGCUphyyyy=RNNNNNNRNRRRRRDg</pre></td></tr>
<tr><td><pre>8#RR#RWNBNRNNNIyyBWNRNNNgQ8$E88$hVhIxc***c))=**)c)L{yEQ&$RgRQ8QR8#pUpDfYtS8Rq8IftjtL:NBBNNNNNWWRRN$R</pre></td></tr>
<tr><td><pre>RQ#RRRWNNNRNNNwyIBNNWRNNRR8D&8#8UVwzvv)??))LyapGqUVhG&808RRR88g8RD#ahF&URRUadhDF%Lcxf_NNNNRNWNRRRR88</pre></td></tr>
<tr><td><pre>R8gRRgRNWWNNWhh{hNBNWQRNNRQ88#Rgd3Cc?)ljIUpERNNNNQR$HDDD0RQR88$$R885{LRUx%%yyGaQyLcc7LNNNNRWRNRRggR8</pre></td></tr>
<tr><td><pre>8RRRRRRNNNNNBt5{{$BWNQRNNRQgQRNREadaUUd$#NBBNWWR#4j{hQD$D8Q888$DQQ8RA$*))?)cLt%{&tLcLf)NNNRNRRRNWRR8</pre></td></tr>
<tr><td><pre>#RRRRRWNNWNNBGqFf{BNWRRWNNR8QRNN843yfj?))cL7Ll?))?1hE#D$RR#QQD$&88$8UD))\)))Scf{$&qaIdyNNWNNRRNWNRgD</pre></td></tr>
<tr><td><pre>gRRRRRWNNNWBWGSI{zNNWNRRRNR#$gNRgh5qS3yjc))))))c1yqU$#8RR#8#80$H08R8d$))\c)8U)?%hva?*7RNNNRNWRRRRRR#</pre></td></tr>
<tr><td><pre>gRRRRWWNNWNN$pVyyYUWNNRQRNWgH#NW#paIa&08qUat1Ihh$8Ep#R8g8R#$D&8$$88Q8$L)**Ij)?)cha!fU==WWNWRNRRNRR#R</pre></td></tr>
<tr><td><pre>RRRWWWNNNNNN$hwwItvNNNQRR#WR88NR88Uhh$&D8gRR8$gR#$EHRQ$8gR8$$H&DH&88R0fc<*r))))cEHNHa$chRNNNNRRNRR8R</pre></td></tr>
<tr><td><pre>RRRNRNNNNNNNj$wyY7LaWWRg##gR88RQRDdpEdEHD8$gRggg8888H$pQR0$D8pEDDpD$QHSc))**<))?URwlcLhhNRNNRgWRRR8R</pre></td></tr>
<tr><td><pre>RRRNWNNNRR8cLpUfF{CLhRWR#W#R8H0RgRH08$8DpE0#QgRRQg#880&8Q&$&Hq5Ud&H&8$&)*\)****pxRvtv??U7NNNNRRRR8RR</pre></td></tr>
<tr><td><pre>RRRRWWNNNNLcLLpD&p$$HWWRQ#R#RpA88#DE888&88D8R##gQ888&&H$A$8p&GPVqddHE8A${*=***=jya))\)?C=RNNNRRNR8Rg</pre></td></tr>
<tr><td><pre>gRRWNNNNWR?lG))LL??rIaNRg$R88$p8QHR$D$#888AHg#RRRg88$Hdddqp&UPpa&pdpA#8w3CGU)?5FR*))<))?)NNNNNRRWER8</pre></td></tr>
<tr><td><pre>RRRRNWNNRR)c8l<)**+=_CRg8##RQ$pQ8D#888#8#8pD$D8Q#QHA$0dqdUGGUSUUAEApd8$8Rz{C=+&3c*+=**)))WNNNRRWRdR#</pre></td></tr>
<tr><td><pre>gRRWRRNRWRl&l)*==+=+*lB88gR#8880$$gg8#RRNR#gRNRNRQ80$&G&SSpdUySSGpp&HHQ5{p$RtLL&_++=**\)*1NNRWRRW8pR</pre></td></tr>
<tr><td><pre>RRRRNRNWWNch?1___=::t8N$#R$RRg8DQ88RNNNBBBBNNNBNNR8&HDEEaSIaVFyIUGHp&0##y*=z$R?d=!;!+=**)*NWNRRRRH&R</pre></td></tr>
<tr><td><pre>RRRRWRNRRQ4??[*_:::~aWR8$RDRggQ8888WWNNNBNNNNWRWRR8&&qpGpUPhI353ha$p5H8$aL*+=5lL)+__!++))*NNNNRRR&#R</pre></td></tr>
<tr><td><pre>RgRRRR{t7Ihfvc*::~:~NQ8Q&E#RR#R8Q#RgRRWNRR8$DDD&8DDdaSwhVGPphSUUAA$$EEH88{r+!zy)y__+_=+=))NNNNWRRU8N</pre></td></tr>
<tr><td><pre>RR#&I8V{Y&7Lc)++.::BNHD$A5HR#R8880#RR88Q80pPpdqUhyqSa{Iy&A5GqIaapdpdS&E&pRS==)E)U___::_!))NNNRRRRUpW</pre></td></tr>
<tr><td><pre>5{3I4I{wPcFjL\)r)CBNNN$HhpUd8g8#8$D0H&hGd0UAU3S[hywhh{Sxy{f%PSa3VUUpGdUH$p8$+_3)h*^;::+_t?NRNNRRRU5R</pre></td></tr>
<tr><td><pre>yyIh3VU8&)L%c)**+pNBRRR8d0IUU88$DHHpEUS3{IIh{ht?%hhjlfCl?l{j{4haSaIUGP0dHH&RN+?c));_^;+=hBNNNWgR8p&R</pre></td></tr>
<tr><td><pre>{hRgpI&aVqUtc?*)<$BNR&&E08ppdEUHd&A5a3Ih4Lccy{c?lvftLlcLccv{y5IFUFhdUppEdUa#N8)S*cl?crt3?RNNNN8#ga&R</pre></td></tr>
<tr><td><pre>IfLYyL[cp8cly)==h8NNg8HE8$SUSGU&U4{tc{Lfy%lL)?[yjCt??vc)c{Iy4a1UVaaapaAqGphI8R8tI5IVq3GaRNWWNNRpgSD#</pre></td></tr>
<tr><td><pre>L1LIxjc)*UI77)+rvGNRR88p&$Ah3Fy{{Lc[t{LLfxvyYv7fvvv[v?l1LF{Vhh{zj1vYyh{UV5USh8R#wRNS)ER#NNNNNNR8#aHG</pre></td></tr>
<tr><td><pre>[x{j%l?)*?$LjryyRNN8$88&&HpIq{yyIStLLl?fl?)?j?tv)jx{xyjcc1cI{fCLCy%yy3{yttFywhHgUhNNBNNNNWRRNNNqDpgF</pre></td></tr>
<tr><td><pre>wf%t7?)))*yydSNNNW#$U8dUd5SUhywwhI{lLcjIwt7?lcL?)twLLLlhSSVI4h%yyh{ft{4j{Y{z?y3Q&UgBNNNNWWNWRWRG$$Qa</pre></td></tr>
<tr><td><pre>1ztjv?)**)\v8NWRR8Hh&GEdhF4IhAVtIVFwF{lfLyL{?v[tyllzVfPUpFAaS{xUaIvfC1II{LljlLYU8UENNNNBNNNNRNREUhdH</pre></td></tr>
<tr><td><pre>tLLLv))<*)W&#88$8HqqHEph5GwFCytIShG3hIwhVUhLyh{tvLyhIyUaypUUG{1yU1z{jttyIzvftc{4SEUQBNNNNNNNNR85UhI$</pre></td></tr>
<tr><td><pre>77lL?)**yNRA$Sdp&d{daIha4ISyaa3hhyLIaaGUI4ap3FwwVIVaSAH&hISGGE5aIy{f{[f{Itfxf?j%1Iy{{3WBNRRRRRyFU0ph</pre></td></tr>
<tr><td><pre>lLvc?)cRR8FUhhh3UphpUVISFVh{UFUhUU&UqyUGd00AGUUGUUp&#&&$G&&q3dUhhVwyywyyIIy{x?{cxyF{xlLNWRRNRW&GH80y</pre></td></tr>
<tr><td><pre>vcvc)#WgqU{yhfFfSVyyhIFy{V343yVV&8H&H&UAUppGAd8DDRQ$&dE$8$pApdUSa5ah4hIyhSV{x?))tIL{ywGNRQQ##pUh)yS=</pre></td></tr>
<tr><td><pre>vlcLNNHUh3w5[Lthy4F{yw3{fyhhPUHAUH0&p&D0ddH8$g#RRRRWWRRRNRRQQ8&pUUUaShI33hFy{[jl?fyCF8NNR&R&&wd5UH0)</pre></td></tr>
<tr><td><pre>tc1RNQ3VIyh[tyLlyhh1y{hyhyyaUUpEE808#8dQNNNNR8#RRRNBWRNBNNNNRRQHGAUahhUUaI3fyftvL[))lwpNWpRGdhGpF$V)</pre></td></tr>
<tr><td><pre></pre></td></tr>

</table>
