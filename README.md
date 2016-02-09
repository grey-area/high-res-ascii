Tool to create high resolution ascii art.

Usage: python ascii.py <image filename> <horizontal resolution>

If horizontal resolution is not specified, it defaults to the smallest of 400 and the original image horizontal resolution.

The image is downsampled, and each pixel is replaced with the printable character closest in brightness to the original pixel, after normalization. Character brightnesses were previously calculated by, for each character, producing an image containing only that character and calculating the mean pixel brightness.

```
<pre><sub><sup><sub><sup>
HGUU08$dD8DD8#g8#)**==***====**rr)))))cLLcL[C{{{Fy{zxtxtzttfIywVypG$HUUdUUUa5ShUEEd&amp;$p&amp;$HUdUpUUaUU&amp;a
Gap08d$8#QQgggR#&amp;*====***==+=*))))))))cLLv7tC{{{y{fztjtztYx{F4VFwydd$$UPUGqUppUaddE$Ed$AD&amp;GUqHUUpUdU
Udd$D&amp;RRR#RRRRRR*=====***=+==&amp;lt;)?)))?))cLLL[tz1f{fCCCztfftY7Cyww4Vy3h$&amp;EShpApUUAAdpaGdD&amp;0dAHppGAPaU&amp;0
UdD88RRRRRRgRgQ)======******)?*.....*......?7CCz%xxttttzxjjC{FIhI{%hdD$$UpAdGhHUUUpEddD&amp;&amp;$&amp;dqqpp5UUd
5pDDRRRRRR#RRRR**=+===*****) .....:P.:...:...~ft7[jt[tttxL[t{{Ih3fLfhd8d&amp;hUp$EppGUGqqU8Q$QDHEUpdpEG&amp;
0A88RRRRRRRRR#****_+=*****....=:*..:.:.........~LljjxjjY[[xf{{ISV{Lv{h&amp;8&amp;Ep5d$$dpdAUp&amp;Sd$$&amp;$&amp;dp&amp;UppU
d&amp;QRRRRWNRRRRN)*=+_+=*)*.:::?.:..,:::,:a:.:.:.: ,.1j[7Ljjtt{yywhV{jxlyUE$8dUUpE$aUpqHd&amp;AU888$DGAH5Uq
d0gRRRWRWR#gRf***=++*)`.,:_L.,::::::!:.:\h^:*** .?.)t[jL7t1yyyFIh{LlL7VGE8$&amp;pG&amp;$&amp;EDdUqH#pU$A$888GHUa
H8#RRWRWNRDRR=*&amp;lt;**=*).)tr.:::::__^~::~..~._...:~y ..:t7L7Yfy{{y33{Lv7cLIpA0pEGPdH$$D&amp;$p$8pp$8p88E&amp;E&amp;
8QgRRNRRRRRRg)))***_:~:.,_.:::::::..,:~..*x::..~ ..~.~tjLYC{{fFhh{Lcllc{aGdqpUpH$$DHHEHdGd&amp;AGDD0HAd$
DQRRRWNRR#RRt&amp;lt;))\*\::^=:~!..:::_.::.:~...)...,..!..,`.:Ll[1{{z{hh{lcc?L[GaUAahUaGH0888D&amp;&amp;0DA&amp;$DA$ppd
8QRRRRWRRRRg*))??):;;:^:)$..)::::::::~..............^`:;Ljz1ft{hh{Lcc??j{hqGGS5aAGHH#RgR$0&amp;88$p8$Ddd
8#RRRWRRRRRR))))c:__^;^::7.:_::::::::::.5h,....::..=.)::)jxtt[{4h{Lc??))fGahUUPhUUE8$QQWRR#&amp;#8&amp;&amp;$gQ8
8gRgRRRRRRRg)))l+__=^:;:.*..::_;::;:::~.=_)~...:..~`..I^*v7[jj{V4{Lv??))lUUhSSUpGGA&amp;8&amp;R88RR8dD8EHHDR
8#RRRRRRgRRy???=^!=^::)V*:)r?::=::::::t_+:.^~..~:.. ``?___LLlL{43{Ll)???)S333UahUUdE$RQRRRRg#U#\([0-9]+?\)&amp;$D
888RggRRgRR\)??C^__::R3:~:.\3c_:^:::?=.)`4;::..:::....^~::*cLL{3Vfvccl)cc{3c{UpaUqq&amp;888RQgRRW#G88$DQ
08ggR#RggRR)??cz::))8.::::::_^v:$)_7...:.7L....,*:::~:.hhy+clL{3I1vcl???cL))fIhUpd&amp;$88gRRgRQRR8pQd&amp;D
&amp;#gRRgRRgR8*))__trVP{^=_+.::...t.:~::*... )~..:::_::;,+*:_a)cL{3IzccLc??)?*)tVhSD&amp;&amp;$HRgRRRNRRQ8dHd&amp;U
88##Q8DRRR*&amp;lt;):=^=t;:+_==::yl^: ).....:..:`)w:::*;::*:_I^^;++lj{3ytccfc)))))t%I5GddD8#8#gRRRRNRggH#p&amp;
#8QQRR8RRD*)):__*y*_**___::_c`.),:,=;......UG:**^^_:_Ih:^^;_j[{3y%cvL?)vj))tywhAH08#gRWRR##RRR8DdH#$
8888Q8gQR*)))*+_*{+**_);=I+::.~5`..`.:  `..~Uy)_;;:;_)F:_;^!*j{IyYc?7??)??ltyaVGHD##WRRRRNNNRWN0$&amp;#8
&amp;8Q88D888))):==*c.===r?!!*:::.:H...... `.:.:&amp;lt;*+::::_*5:_____)x{3FYcc?Lcj?LfFy3UUH088#RRRRRNRWNgN$$$R
p$88H0p#&amp;lt;)?):_+*f=+**=*+c*_~::.*;.....`......)yU$AADDL:;;;_=+t{Iyjccv?cLL?L3ShGq$8D8RRRRRRNWRRRRRp$R
d88D$D8R))));:?hy**?1_=*;_;:..:_...,^.:.;...aL.`.,r==I+:!_=+*j{3wYct??ttj1f{hGU&amp;$8RRRRWWWRNNRWRNR8$0
D8$88&amp;Hp))c*^:*)8*?h++*+__._.::^C.:~:.... .;{{:,..l:,*y!!_;*\?{Iyj)xyctc){3Vh5AA$8#RRRRRRWRRNNRRRRHQ
H$8D&amp;Hd7???=:_)L?&amp;lt;t)*+=_:^:.::_*c..:..:..` {=..`.`,)_:y=___=)?{Iylc[4Lf{yhPaq&amp;pdGHRRRRRRNNNNRWNRRRQ8
HD#$H0&amp;wLLl_==))la*c*!+__):: ;:?x:..~.`...3jL . ....::.t_+=*L?j{{CC{yIhhU5aGdA0D$$8Q$RRRNNNNNRNNRRRg
$88DD&amp;h3{zt==r??Ldl)*+=!=_::P=U...)?)I _ j&amp;SWRgG)))*:..?*+*)h))Y{llwfGVpD0dUH$D$D$D88QRWRNNNNNRNNg##
$Q8D8H53Iy{_)lv)p)&amp;t\)=*_:^h)=)=*?+:=UyU)3=wpGhpqpp#RHRU*=&amp;lt;y;ULzctyIUISH8D$0D$8Q8888#Q8#RNNNNBWRRNQR
8888$EUVhI1rr{LV)c)c&amp;y)*=;Fz**{gR8&amp;DH8R?8{FtwU{h$UPhSd$V)hH)_{?ccv1hh8d&amp;HpDH88RgRRWRRR8RRNNNNNNRRRWg
88#8Q&amp;dhhhC)vt&amp;??)L&amp;lt;+=gH)h{WBNR8q$EApURRNc{&amp;RRRaG$Uhh4&amp;pp_?=^_Lt??VpPh5dp08RggQ#RWWWRRNRWRRNWNNNQRWN
8#RQD8HU4hh&amp;lt;tt))?)**))):hqNB8H&amp;d&amp;NRRAa8gRD4NgRh?ChAhSVGq$RBN${v3w{yEUHUdH&amp;&amp;$R88QWRRRRWNRWWNNRRRNWgRW
8gRRQ88Ga{wAV8l?c)??r*+{?DB$UU8EaRRRRp&amp;H$$a34{f*)3U55haGUDUNNNpwV1VD0$D&amp;p$H8HD#RggRRRRNWNNWNNRRRNQRR
8RRRRR8d0ww7&amp;LL)??)*\*:={BQdUddyv7V4{SGdHpS)\))Lh3PUS3UPqR&amp;&amp;Ngh*)wSa8H#gp$&amp;&amp;H#RggRRRRNRWNNRNNRRNNNRQ
8gRRRR8ApqFjIlj??x))**)[HNdqppUIc?))cyaSGhhaI3aqhhGUhPUGGp$UNU{Rd:IHRgg8D&amp;G&amp;DD$DRRRRWNNNNNNRRWRRNWg8
gRRRggQD#&amp;htyy[Llcc)=*cFNR$0ApGU3{hFF5h3hI3{IIIyFA5UhhaUGDRERUU8$#p&amp;lt;~N8R$H&amp;&amp;Qp88#RRRWWNNNNNNRRRRgNRR
RRRR#g#88Ha3C8Lt?c&amp;lt;\==LyNRH&amp;UGpUdhhahIIIVIFyy{yFaa4wIShqpUDHpHfV43hVh:`P8$Q8ED$8gRRNNNNNNNNNWWggQRRR
QgRRRR#R$$Uh{Hyyj))&amp;lt;**rc&amp;lt;D&amp;&amp;5aAaqwShya4w{{tIFV{IyhSUhS35aU#$UR$I{YhtwU4=+88pHH8DgNRRWNNNNNRWRRR#RRWR
RRRNRRR88&amp;EawSyyt))**){1N8dAUGUSaUhhwIwtL7tYtLIVaISpUPaaqE$Q$$R$Y{{y{G3A.g&amp;H$D$#gRRRNNNNNNWNNRRgRgRR
RRRRRRRRAE$d3aayCv)r*faNRQ0pAqApGF3pa[7{l%taRC3lSSdPUUVpAd8$d0gd{FL1Ip%U :&amp;8888RRWRRNBBBBNBNRRNRRRRQ
#RRRRRRgQ&amp;$$3a8htv)))LwNg$pqGpU&amp;&amp;G35ztGRR{l#qhpcfhaDpphq0&amp;$D0p8dLwC{Gptwy !R888gW#RNNNNBBBNNRRWRQWQR
#RRRRRWR880UhPUFy)1G$NNRdAAq&amp;qEGPV$y[1{URRpHt7jL?1U&amp;d&amp;UpppE$8$QSySwIhIIEy+*t8gRNgRRNNNNNNBBBNRRRRWRR
#RR#RRRRQDD&amp;A4U);18RBNW#&amp;8dpqGI$adwj=ay%yfItcv?j\LyPE&amp;Ud&amp;&amp;R8#EH843ya3{3SUc=_=gWRRRNNNNNNNNBBRNRRRRRR
#RRRR#RRRQQ$&amp;p#l?hHBBNRD&amp;8HddEpGUSF)vv)*?)l)+)v)=c1hp&amp;ppd&amp;888DQ8hU)?hhFyI*4R#&amp;:NgRNBNBNNNNNRNRgR88gN
gR#RRgRNRR#8g&amp;QL?=NNNNR8$D0&amp;d$&amp;GqSt?)l)*)))*?)*_*)t{U$Udd8888#8H$7))?{{x{ypRRpj3+RNNNNBBBNNNNRWDgggR
#RRRRRRNWRRRR$$7)RNNWW#88$$8$&amp;U&amp;pIzL*&amp;lt;))))*)?)_+*)%yI&amp;UE$DQRDQ88&amp;dxL?Lxy{FH&amp;#G)qacNNBNNBNNBNNNRRRQRR
ggRRRRWNWRRNW8hc)WNNRNRR88EDH8pHP3{vr+_*====&amp;lt;_=)*ctyh$0$&amp;&amp;RR#Qg8$Fq))?cLy5cfgUtI3FcWNBNBNNNNWNgWR##g
ggRgRgRRNNRRNN{t?BNNRWNR8D8D&amp;HD$IVF{)*===*)+*?)*cc?L{0DdD#QR#$#8HqIUL)y&amp;8yGCUphyyyy=RNNNNNNRNRRRRRDg
8#RR#RWNBNRNNNIyyBWNRNNNgQ8$E88$hVhIxc***c))=**)c)L{yEQ&amp;$RgRQ8QR8#pUpDfYtS8Rq8IftjtL:NBBNNNNNWWRRN$R
RQ#RRRWNNNRNNNwyIBNNWRNNRR8D&amp;8#8UVwzvv)??))LyapGqUVhG&amp;808RRR88g8RD#ahF&amp;URRUadhDF%Lcxf_NNNNRNWNRRRR88
R8gRRgRNWWNNWhh{hNBNWQRNNRQ88#Rgd3Cc?)ljIUpERNNNNQR$HDDD0RQR88$$R885{LRUx%%yyGaQyLcc7LNNNNRWRNRRggR8
8RRRRRRNNNNNBt5{{$BWNQRNNRQgQRNREadaUUd$#NBBNWWR#4j{hQD$D8Q888$DQQ8RA$*))?)cLt%{&amp;tLcLf)NNNRNRRRNWRR8
#RRRRRWNNWNNBGqFf{BNWRRWNNR8QRNN843yfj?))cL7Ll?))?1hE#D$RR#QQD$&amp;88$8UD))\)))Scf{$&amp;qaIdyNNWNNRRNWNRgD
gRRRRRWNNNWBWGSI{zNNWNRRRNR#$gNRgh5qS3yjc))))))c1yqU$#8RR#8#80$H08R8d$))\c)8U)?%hva?*7RNNNRNWRRRRRR#
gRRRRWWNNWNN$pVyyYUWNNRQRNWgH#NW#paIa&amp;08qUat1Ihh$8Ep#R8g8R#$D&amp;8$$88Q8$L)**Ij)?)cha!fU==WWNWRNRRNRR#R
RRRWWWNNNNNN$hwwItvNNNQRR#WR88NR88Uhh$&amp;D8gRR8$gR#$EHRQ$8gR8$$H&amp;DH&amp;88R0fc&amp;lt;*r))))cEHNHa$chRNNNNRRNRR8R
RRRNRNNNNNNNj$wyY7LaWWRg##gR88RQRDdpEdEHD8$gRggg8888H$pQR0$D8pEDDpD$QHSc))**&amp;lt;))?URwlcLhhNRNNRgWRRR8R
RRRNWNNNRR8cLpUfF{CLhRWR#W#R8H0RgRH08$8DpE0#QgRRQg#880&amp;8Q&amp;$&amp;Hq5Ud&amp;H&amp;8$&amp;)*\)****pxRvtv??U7NNNNRRRR8RR
RRRRWWNNNNLcLLpD&amp;p$$HWWRQ#R#RpA88#DE888&amp;88D8R##gQ888&amp;&amp;H$A$8p&amp;GPVqddHE8A${*=***=jya))\)?C=RNNNRRNR8Rg
gRRWNNNNWR?lG))LL??rIaNRg$R88$p8QHR$D$#888AHg#RRRg88$Hdddqp&amp;UPpa&amp;pdpA#8w3CGU)?5FR*))&amp;lt;))?)NNNNNRRWER8
RRRRNWNNRR)c8l&amp;lt;)**+=_CRg8##RQ$pQ8D#888#8#8pD$D8Q#QHA$0dqdUGGUSUUAEApd8$8Rz{C=+&amp;3c*+=**)))WNNNRRWRdR#
gRRWRRNRWRl&amp;l)*==+=+*lB88gR#8880$$gg8#RRNR#gRNRNRQ80$&amp;G&amp;SSpdUySSGpp&amp;HHQ5{p$RtLL&amp;_++=**\)*1NNRWRRW8pR
RRRRNRNWWNch?1___=::t8N$#R$RRg8DQ88RNNNBBBBNNNBNNR8&amp;HDEEaSIaVFyIUGHp&amp;0##y*=z$R?d=!;!+=**)*NWNRRRRH&amp;R
RRRRWRNRRQ4??[*_:::~aWR8$RDRggQ8888WWNNNBNNNNWRWRR8&amp;&amp;qpGpUPhI353ha$p5H8$aL*+=5lL)+__!++))*NNNNRRR&amp;#R
RgRRRR{t7Ihfvc*::~:~NQ8Q&amp;E#RR#R8Q#RgRRWNRR8$DDD&amp;8DDdaSwhVGPphSUUAA$$EEH88{r+!zy)y__+_=+=))NNNNWRRU8N
RR#&amp;I8V{Y&amp;7Lc)++.::BNHD$A5HR#R8880#RR88Q80pPpdqUhyqSa{Iy&amp;A5GqIaapdpdS&amp;E&amp;pRS==)E)U___::_!))NNNRRRRUpW
5{3I4I{wPcFjL\)r)CBNNN$HhpUd8g8#8$D0H&amp;hGd0UAU3S[hywhh{Sxy{f%PSa3VUUpGdUH$p8$+_3)h*^;::+_t?NRNNRRRU5R
yyIh3VU8&amp;)L%c)**+pNBRRR8d0IUU88$DHHpEUS3{IIh{ht?%hhjlfCl?l{j{4haSaIUGP0dHH&amp;RN+?c));_^;+=hBNNNWgR8p&amp;R
{hRgpI&amp;aVqUtc?*)&amp;lt;$BNR&amp;&amp;E08ppdEUHd&amp;A5a3Ih4Lccy{c?lvftLlcLccv{y5IFUFhdUppEdUa#N8)S*cl?crt3?RNNNN8#ga&amp;R
IfLYyL[cp8cly)==h8NNg8HE8$SUSGU&amp;U4{tc{Lfy%lL)?[yjCt??vc)c{Iy4a1UVaaapaAqGphI8R8tI5IVq3GaRNWWNNRpgSD#
L1LIxjc)*UI77)+rvGNRR88p&amp;$Ah3Fy{{Lc[t{LLfxvyYv7fvvv[v?l1LF{Vhh{zj1vYyh{UV5USh8R#wRNS)ER#NNNNNNR8#aHG
[x{j%l?)*?$LjryyRNN8$88&amp;&amp;HpIq{yyIStLLl?fl?)?j?tv)jx{xyjcc1cI{fCLCy%yy3{yttFywhHgUhNNBNNNNWRRNNNqDpgF
wf%t7?)))*yydSNNNW#$U8dUd5SUhywwhI{lLcjIwt7?lcL?)twLLLlhSSVI4h%yyh{ft{4j{Y{z?y3Q&amp;UgBNNNNWWNWRWRG$$Qa
1ztjv?)**)\v8NWRR8Hh&amp;GEdhF4IhAVtIVFwF{lfLyL{?v[tyllzVfPUpFAaS{xUaIvfC1II{LljlLYU8UENNNNBNNNNRNREUhdH
tLLLv))&amp;lt;*)W&amp;#88$8HqqHEph5GwFCytIShG3hIwhVUhLyh{tvLyhIyUaypUUG{1yU1z{jttyIzvftc{4SEUQBNNNNNNNNR85UhI$
77lL?)**yNRA$Sdp&amp;d{daIha4ISyaa3hhyLIaaGUI4ap3FwwVIVaSAH&amp;hISGGE5aIy{f{[f{Itfxf?j%1Iy{{3WBNRRRRRyFU0ph
lLvc?)cRR8FUhhh3UphpUVISFVh{UFUhUU&amp;UqyUGd00AGUUGUUp&amp;#&amp;&amp;$G&amp;&amp;q3dUhhVwyywyyIIy{x?{cxyF{xlLNWRRNRW&amp;GH80y
vcvc)#WgqU{yhfFfSVyyhIFy{V343yVV&amp;8H&amp;H&amp;UAUppGAd8DDRQ$&amp;dE$8$pApdUSa5ah4hIyhSV{x?))tIL{ywGNRQQ##pUh)yS=
vlcLNNHUh3w5[Lthy4F{yw3{fyhhPUHAUH0&amp;p&amp;D0ddH8$g#RRRRWWRRRNRRQQ8&amp;pUUUaShI33hFy{[jl?fyCF8NNR&amp;R&amp;&amp;wd5UH0)
tc1RNQ3VIyh[tyLlyhh1y{hyhyyaUUpEE808#8dQNNNNR8#RRRNBWRNBNNNNRRQHGAUahhUUaI3fyftvL[))lwpNWpRGdhGpF$V)
</sup></sub></sup></sub></pre>
```
