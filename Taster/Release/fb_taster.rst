                              1 ;--------------------------------------------------------
                              2 ; File Created by SDCC : free open source ANSI-C Compiler
                              3 ; Version 3.1.0 #7066 (Jun 14 2012) (Linux)
                              4 ; This file was generated Sat Oct 18 20:04:36 2014
                              5 ;--------------------------------------------------------
                              6 	.module fb_taster
                              7 	.optsdcc -mmcs51 --model-small
                              8 	
                              9 ;--------------------------------------------------------
                             10 ; Public variables in this module
                             11 ;--------------------------------------------------------
                             12 	.globl _main
                             13 	.globl _delay_timer
                             14 	.globl _switch_led
                             15 	.globl _port_changed
                             16 	.globl _restart_app
                             17 	.globl _process_tel
                             18 	.globl _restart_hw
                             19 	.globl _send_obj_value
                             20 	.globl _P3_1
                             21 	.globl _P3_0
                             22 	.globl _P1_7
                             23 	.globl _P1_6
                             24 	.globl _P1_5
                             25 	.globl _P1_4
                             26 	.globl _P1_3
                             27 	.globl _P1_2
                             28 	.globl _P1_1
                             29 	.globl _P1_0
                             30 	.globl _P0_7
                             31 	.globl _P0_6
                             32 	.globl _P0_5
                             33 	.globl _P0_4
                             34 	.globl _P0_3
                             35 	.globl _P0_2
                             36 	.globl _P0_1
                             37 	.globl _P0_0
                             38 	.globl _I2CON_0
                             39 	.globl _I2CON_2
                             40 	.globl _I2CON_3
                             41 	.globl _I2CON_4
                             42 	.globl _I2CON_5
                             43 	.globl _I2CON_6
                             44 	.globl _SCON_7
                             45 	.globl _SCON_6
                             46 	.globl _SCON_5
                             47 	.globl _SCON_4
                             48 	.globl _SCON_3
                             49 	.globl _SCON_2
                             50 	.globl _SCON_1
                             51 	.globl _SCON_0
                             52 	.globl _IP0_0
                             53 	.globl _IP0_1
                             54 	.globl _IP0_2
                             55 	.globl _IP0_3
                             56 	.globl _IP0_4
                             57 	.globl _IP0_5
                             58 	.globl _IP0_6
                             59 	.globl _IP1_0
                             60 	.globl _IP1_1
                             61 	.globl _IP1_2
                             62 	.globl _IP1_6
                             63 	.globl _IEN1_0
                             64 	.globl _IEN1_1
                             65 	.globl _IEN1_2
                             66 	.globl _IEN0_0
                             67 	.globl _IEN0_1
                             68 	.globl _IEN0_2
                             69 	.globl _IEN0_3
                             70 	.globl _IEN0_4
                             71 	.globl _IEN0_5
                             72 	.globl _IEN0_6
                             73 	.globl _IEN0_7
                             74 	.globl _TCON_0
                             75 	.globl _TCON_1
                             76 	.globl _TCON_2
                             77 	.globl _TCON_3
                             78 	.globl _TCON_4
                             79 	.globl _TCON_5
                             80 	.globl _TCON_6
                             81 	.globl _TCON_7
                             82 	.globl _PSW_7
                             83 	.globl _PSW_6
                             84 	.globl _PSW_5
                             85 	.globl _PSW_4
                             86 	.globl _PSW_3
                             87 	.globl _PSW_2
                             88 	.globl _PSW_1
                             89 	.globl _PSW_0
                             90 	.globl _IEN1
                             91 	.globl _IP0H
                             92 	.globl _WFEED2
                             93 	.globl _WFEED1
                             94 	.globl _WDL
                             95 	.globl _WDCON
                             96 	.globl _TRIM
                             97 	.globl _TAMOD
                             98 	.globl _SSTAT
                             99 	.globl _RTCL
                            100 	.globl _RTCH
                            101 	.globl _RTCCON
                            102 	.globl _RSTSRC
                            103 	.globl _PT0AD
                            104 	.globl _PCONA
                            105 	.globl _P3M2
                            106 	.globl _P3M1
                            107 	.globl _P1M2
                            108 	.globl _P1M1
                            109 	.globl _P0M2
                            110 	.globl _P0M1
                            111 	.globl _KBPATN
                            112 	.globl _KBMASK
                            113 	.globl _KBCON
                            114 	.globl _IP1H
                            115 	.globl _IP1
                            116 	.globl _I2STAT
                            117 	.globl _I2SCLL
                            118 	.globl _I2SCLH
                            119 	.globl _I2DAT
                            120 	.globl _I2CON
                            121 	.globl _I2ADR
                            122 	.globl _FMDATA
                            123 	.globl _FMCON
                            124 	.globl _FMADRL
                            125 	.globl _FMADRH
                            126 	.globl _DIVM
                            127 	.globl _CMP2
                            128 	.globl _CMP1
                            129 	.globl _BRGCON
                            130 	.globl _BRGR1
                            131 	.globl _BRGR0
                            132 	.globl _SADEN
                            133 	.globl _SADDR
                            134 	.globl _AUXR1
                            135 	.globl _SBUF
                            136 	.globl _SCON
                            137 	.globl _IP0
                            138 	.globl _IEN0
                            139 	.globl _TH1
                            140 	.globl _TH0
                            141 	.globl _TL1
                            142 	.globl _TL0
                            143 	.globl _TMOD
                            144 	.globl _TCON
                            145 	.globl _PCON
                            146 	.globl _DPH
                            147 	.globl _DPL
                            148 	.globl _SP
                            149 	.globl _B
                            150 	.globl _ACC
                            151 	.globl _PSW
                            152 	.globl _P3
                            153 	.globl _P1
                            154 	.globl _P0
                            155 	.globl _object_value
                            156 	.globl _RAM
                            157 ;--------------------------------------------------------
                            158 ; special function registers
                            159 ;--------------------------------------------------------
                            160 	.area RSEG    (ABS,DATA)
   0000                     161 	.org 0x0000
                    0080    162 G$P0$0$0 == 0x0080
                    0080    163 _P0	=	0x0080
                    0090    164 G$P1$0$0 == 0x0090
                    0090    165 _P1	=	0x0090
                    00B0    166 G$P3$0$0 == 0x00b0
                    00B0    167 _P3	=	0x00b0
                    00D0    168 G$PSW$0$0 == 0x00d0
                    00D0    169 _PSW	=	0x00d0
                    00E0    170 G$ACC$0$0 == 0x00e0
                    00E0    171 _ACC	=	0x00e0
                    00F0    172 G$B$0$0 == 0x00f0
                    00F0    173 _B	=	0x00f0
                    0081    174 G$SP$0$0 == 0x0081
                    0081    175 _SP	=	0x0081
                    0082    176 G$DPL$0$0 == 0x0082
                    0082    177 _DPL	=	0x0082
                    0083    178 G$DPH$0$0 == 0x0083
                    0083    179 _DPH	=	0x0083
                    0087    180 G$PCON$0$0 == 0x0087
                    0087    181 _PCON	=	0x0087
                    0088    182 G$TCON$0$0 == 0x0088
                    0088    183 _TCON	=	0x0088
                    0089    184 G$TMOD$0$0 == 0x0089
                    0089    185 _TMOD	=	0x0089
                    008A    186 G$TL0$0$0 == 0x008a
                    008A    187 _TL0	=	0x008a
                    008B    188 G$TL1$0$0 == 0x008b
                    008B    189 _TL1	=	0x008b
                    008C    190 G$TH0$0$0 == 0x008c
                    008C    191 _TH0	=	0x008c
                    008D    192 G$TH1$0$0 == 0x008d
                    008D    193 _TH1	=	0x008d
                    00A8    194 G$IEN0$0$0 == 0x00a8
                    00A8    195 _IEN0	=	0x00a8
                    00B8    196 G$IP0$0$0 == 0x00b8
                    00B8    197 _IP0	=	0x00b8
                    0098    198 G$SCON$0$0 == 0x0098
                    0098    199 _SCON	=	0x0098
                    0099    200 G$SBUF$0$0 == 0x0099
                    0099    201 _SBUF	=	0x0099
                    00A2    202 G$AUXR1$0$0 == 0x00a2
                    00A2    203 _AUXR1	=	0x00a2
                    00A9    204 G$SADDR$0$0 == 0x00a9
                    00A9    205 _SADDR	=	0x00a9
                    00B9    206 G$SADEN$0$0 == 0x00b9
                    00B9    207 _SADEN	=	0x00b9
                    00BE    208 G$BRGR0$0$0 == 0x00be
                    00BE    209 _BRGR0	=	0x00be
                    00BF    210 G$BRGR1$0$0 == 0x00bf
                    00BF    211 _BRGR1	=	0x00bf
                    00BD    212 G$BRGCON$0$0 == 0x00bd
                    00BD    213 _BRGCON	=	0x00bd
                    00AC    214 G$CMP1$0$0 == 0x00ac
                    00AC    215 _CMP1	=	0x00ac
                    00AD    216 G$CMP2$0$0 == 0x00ad
                    00AD    217 _CMP2	=	0x00ad
                    0095    218 G$DIVM$0$0 == 0x0095
                    0095    219 _DIVM	=	0x0095
                    00E7    220 G$FMADRH$0$0 == 0x00e7
                    00E7    221 _FMADRH	=	0x00e7
                    00E6    222 G$FMADRL$0$0 == 0x00e6
                    00E6    223 _FMADRL	=	0x00e6
                    00E4    224 G$FMCON$0$0 == 0x00e4
                    00E4    225 _FMCON	=	0x00e4
                    00E5    226 G$FMDATA$0$0 == 0x00e5
                    00E5    227 _FMDATA	=	0x00e5
                    00DB    228 G$I2ADR$0$0 == 0x00db
                    00DB    229 _I2ADR	=	0x00db
                    00D8    230 G$I2CON$0$0 == 0x00d8
                    00D8    231 _I2CON	=	0x00d8
                    00DA    232 G$I2DAT$0$0 == 0x00da
                    00DA    233 _I2DAT	=	0x00da
                    00DD    234 G$I2SCLH$0$0 == 0x00dd
                    00DD    235 _I2SCLH	=	0x00dd
                    00DC    236 G$I2SCLL$0$0 == 0x00dc
                    00DC    237 _I2SCLL	=	0x00dc
                    00D9    238 G$I2STAT$0$0 == 0x00d9
                    00D9    239 _I2STAT	=	0x00d9
                    00F8    240 G$IP1$0$0 == 0x00f8
                    00F8    241 _IP1	=	0x00f8
                    00F7    242 G$IP1H$0$0 == 0x00f7
                    00F7    243 _IP1H	=	0x00f7
                    0094    244 G$KBCON$0$0 == 0x0094
                    0094    245 _KBCON	=	0x0094
                    0086    246 G$KBMASK$0$0 == 0x0086
                    0086    247 _KBMASK	=	0x0086
                    0093    248 G$KBPATN$0$0 == 0x0093
                    0093    249 _KBPATN	=	0x0093
                    0084    250 G$P0M1$0$0 == 0x0084
                    0084    251 _P0M1	=	0x0084
                    0085    252 G$P0M2$0$0 == 0x0085
                    0085    253 _P0M2	=	0x0085
                    0091    254 G$P1M1$0$0 == 0x0091
                    0091    255 _P1M1	=	0x0091
                    0092    256 G$P1M2$0$0 == 0x0092
                    0092    257 _P1M2	=	0x0092
                    00B1    258 G$P3M1$0$0 == 0x00b1
                    00B1    259 _P3M1	=	0x00b1
                    00B2    260 G$P3M2$0$0 == 0x00b2
                    00B2    261 _P3M2	=	0x00b2
                    00B5    262 G$PCONA$0$0 == 0x00b5
                    00B5    263 _PCONA	=	0x00b5
                    00F6    264 G$PT0AD$0$0 == 0x00f6
                    00F6    265 _PT0AD	=	0x00f6
                    00DF    266 G$RSTSRC$0$0 == 0x00df
                    00DF    267 _RSTSRC	=	0x00df
                    00D1    268 G$RTCCON$0$0 == 0x00d1
                    00D1    269 _RTCCON	=	0x00d1
                    00D2    270 G$RTCH$0$0 == 0x00d2
                    00D2    271 _RTCH	=	0x00d2
                    00D3    272 G$RTCL$0$0 == 0x00d3
                    00D3    273 _RTCL	=	0x00d3
                    00BA    274 G$SSTAT$0$0 == 0x00ba
                    00BA    275 _SSTAT	=	0x00ba
                    008F    276 G$TAMOD$0$0 == 0x008f
                    008F    277 _TAMOD	=	0x008f
                    0096    278 G$TRIM$0$0 == 0x0096
                    0096    279 _TRIM	=	0x0096
                    00A7    280 G$WDCON$0$0 == 0x00a7
                    00A7    281 _WDCON	=	0x00a7
                    00C1    282 G$WDL$0$0 == 0x00c1
                    00C1    283 _WDL	=	0x00c1
                    00C2    284 G$WFEED1$0$0 == 0x00c2
                    00C2    285 _WFEED1	=	0x00c2
                    00C3    286 G$WFEED2$0$0 == 0x00c3
                    00C3    287 _WFEED2	=	0x00c3
                    00B7    288 G$IP0H$0$0 == 0x00b7
                    00B7    289 _IP0H	=	0x00b7
                    00E8    290 G$IEN1$0$0 == 0x00e8
                    00E8    291 _IEN1	=	0x00e8
                            292 ;--------------------------------------------------------
                            293 ; special function bits
                            294 ;--------------------------------------------------------
                            295 	.area RSEG    (ABS,DATA)
   0000                     296 	.org 0x0000
                    00D0    297 G$PSW_0$0$0 == 0x00d0
                    00D0    298 _PSW_0	=	0x00d0
                    00D1    299 G$PSW_1$0$0 == 0x00d1
                    00D1    300 _PSW_1	=	0x00d1
                    00D2    301 G$PSW_2$0$0 == 0x00d2
                    00D2    302 _PSW_2	=	0x00d2
                    00D3    303 G$PSW_3$0$0 == 0x00d3
                    00D3    304 _PSW_3	=	0x00d3
                    00D4    305 G$PSW_4$0$0 == 0x00d4
                    00D4    306 _PSW_4	=	0x00d4
                    00D5    307 G$PSW_5$0$0 == 0x00d5
                    00D5    308 _PSW_5	=	0x00d5
                    00D6    309 G$PSW_6$0$0 == 0x00d6
                    00D6    310 _PSW_6	=	0x00d6
                    00D7    311 G$PSW_7$0$0 == 0x00d7
                    00D7    312 _PSW_7	=	0x00d7
                    008F    313 G$TCON_7$0$0 == 0x008f
                    008F    314 _TCON_7	=	0x008f
                    008E    315 G$TCON_6$0$0 == 0x008e
                    008E    316 _TCON_6	=	0x008e
                    008D    317 G$TCON_5$0$0 == 0x008d
                    008D    318 _TCON_5	=	0x008d
                    008C    319 G$TCON_4$0$0 == 0x008c
                    008C    320 _TCON_4	=	0x008c
                    008B    321 G$TCON_3$0$0 == 0x008b
                    008B    322 _TCON_3	=	0x008b
                    008A    323 G$TCON_2$0$0 == 0x008a
                    008A    324 _TCON_2	=	0x008a
                    0089    325 G$TCON_1$0$0 == 0x0089
                    0089    326 _TCON_1	=	0x0089
                    0088    327 G$TCON_0$0$0 == 0x0088
                    0088    328 _TCON_0	=	0x0088
                    00AF    329 G$IEN0_7$0$0 == 0x00af
                    00AF    330 _IEN0_7	=	0x00af
                    00AE    331 G$IEN0_6$0$0 == 0x00ae
                    00AE    332 _IEN0_6	=	0x00ae
                    00AD    333 G$IEN0_5$0$0 == 0x00ad
                    00AD    334 _IEN0_5	=	0x00ad
                    00AC    335 G$IEN0_4$0$0 == 0x00ac
                    00AC    336 _IEN0_4	=	0x00ac
                    00AB    337 G$IEN0_3$0$0 == 0x00ab
                    00AB    338 _IEN0_3	=	0x00ab
                    00AA    339 G$IEN0_2$0$0 == 0x00aa
                    00AA    340 _IEN0_2	=	0x00aa
                    00A9    341 G$IEN0_1$0$0 == 0x00a9
                    00A9    342 _IEN0_1	=	0x00a9
                    00A8    343 G$IEN0_0$0$0 == 0x00a8
                    00A8    344 _IEN0_0	=	0x00a8
                    00EA    345 G$IEN1_2$0$0 == 0x00ea
                    00EA    346 _IEN1_2	=	0x00ea
                    00E9    347 G$IEN1_1$0$0 == 0x00e9
                    00E9    348 _IEN1_1	=	0x00e9
                    00E8    349 G$IEN1_0$0$0 == 0x00e8
                    00E8    350 _IEN1_0	=	0x00e8
                    00FE    351 G$IP1_6$0$0 == 0x00fe
                    00FE    352 _IP1_6	=	0x00fe
                    00FA    353 G$IP1_2$0$0 == 0x00fa
                    00FA    354 _IP1_2	=	0x00fa
                    00F9    355 G$IP1_1$0$0 == 0x00f9
                    00F9    356 _IP1_1	=	0x00f9
                    00F8    357 G$IP1_0$0$0 == 0x00f8
                    00F8    358 _IP1_0	=	0x00f8
                    00BE    359 G$IP0_6$0$0 == 0x00be
                    00BE    360 _IP0_6	=	0x00be
                    00BD    361 G$IP0_5$0$0 == 0x00bd
                    00BD    362 _IP0_5	=	0x00bd
                    00BC    363 G$IP0_4$0$0 == 0x00bc
                    00BC    364 _IP0_4	=	0x00bc
                    00BB    365 G$IP0_3$0$0 == 0x00bb
                    00BB    366 _IP0_3	=	0x00bb
                    00BA    367 G$IP0_2$0$0 == 0x00ba
                    00BA    368 _IP0_2	=	0x00ba
                    00B9    369 G$IP0_1$0$0 == 0x00b9
                    00B9    370 _IP0_1	=	0x00b9
                    00B8    371 G$IP0_0$0$0 == 0x00b8
                    00B8    372 _IP0_0	=	0x00b8
                    0098    373 G$SCON_0$0$0 == 0x0098
                    0098    374 _SCON_0	=	0x0098
                    0099    375 G$SCON_1$0$0 == 0x0099
                    0099    376 _SCON_1	=	0x0099
                    009A    377 G$SCON_2$0$0 == 0x009a
                    009A    378 _SCON_2	=	0x009a
                    009B    379 G$SCON_3$0$0 == 0x009b
                    009B    380 _SCON_3	=	0x009b
                    009C    381 G$SCON_4$0$0 == 0x009c
                    009C    382 _SCON_4	=	0x009c
                    009D    383 G$SCON_5$0$0 == 0x009d
                    009D    384 _SCON_5	=	0x009d
                    009E    385 G$SCON_6$0$0 == 0x009e
                    009E    386 _SCON_6	=	0x009e
                    009F    387 G$SCON_7$0$0 == 0x009f
                    009F    388 _SCON_7	=	0x009f
                    00DE    389 G$I2CON_6$0$0 == 0x00de
                    00DE    390 _I2CON_6	=	0x00de
                    00DD    391 G$I2CON_5$0$0 == 0x00dd
                    00DD    392 _I2CON_5	=	0x00dd
                    00DC    393 G$I2CON_4$0$0 == 0x00dc
                    00DC    394 _I2CON_4	=	0x00dc
                    00DB    395 G$I2CON_3$0$0 == 0x00db
                    00DB    396 _I2CON_3	=	0x00db
                    00DA    397 G$I2CON_2$0$0 == 0x00da
                    00DA    398 _I2CON_2	=	0x00da
                    00D8    399 G$I2CON_0$0$0 == 0x00d8
                    00D8    400 _I2CON_0	=	0x00d8
                    0080    401 G$P0_0$0$0 == 0x0080
                    0080    402 _P0_0	=	0x0080
                    0081    403 G$P0_1$0$0 == 0x0081
                    0081    404 _P0_1	=	0x0081
                    0082    405 G$P0_2$0$0 == 0x0082
                    0082    406 _P0_2	=	0x0082
                    0083    407 G$P0_3$0$0 == 0x0083
                    0083    408 _P0_3	=	0x0083
                    0084    409 G$P0_4$0$0 == 0x0084
                    0084    410 _P0_4	=	0x0084
                    0085    411 G$P0_5$0$0 == 0x0085
                    0085    412 _P0_5	=	0x0085
                    0086    413 G$P0_6$0$0 == 0x0086
                    0086    414 _P0_6	=	0x0086
                    0087    415 G$P0_7$0$0 == 0x0087
                    0087    416 _P0_7	=	0x0087
                    0090    417 G$P1_0$0$0 == 0x0090
                    0090    418 _P1_0	=	0x0090
                    0091    419 G$P1_1$0$0 == 0x0091
                    0091    420 _P1_1	=	0x0091
                    0092    421 G$P1_2$0$0 == 0x0092
                    0092    422 _P1_2	=	0x0092
                    0093    423 G$P1_3$0$0 == 0x0093
                    0093    424 _P1_3	=	0x0093
                    0094    425 G$P1_4$0$0 == 0x0094
                    0094    426 _P1_4	=	0x0094
                    0095    427 G$P1_5$0$0 == 0x0095
                    0095    428 _P1_5	=	0x0095
                    0096    429 G$P1_6$0$0 == 0x0096
                    0096    430 _P1_6	=	0x0096
                    0097    431 G$P1_7$0$0 == 0x0097
                    0097    432 _P1_7	=	0x0097
                    00B0    433 G$P3_0$0$0 == 0x00b0
                    00B0    434 _P3_0	=	0x00b0
                    00B1    435 G$P3_1$0$0 == 0x00b1
                    00B1    436 _P3_1	=	0x00b1
                            437 ;--------------------------------------------------------
                            438 ; overlayable register banks
                            439 ;--------------------------------------------------------
                            440 	.area REG_BANK_0	(REL,OVR,DATA)
   0000                     441 	.ds 8
                            442 ;--------------------------------------------------------
                            443 ; overlayable bit register bank
                            444 ;--------------------------------------------------------
                            445 	.area BIT_BANK	(REL,OVR,DATA)
   0023                     446 bits:
   0023                     447 	.ds 1
                    8000    448 	b0 = bits[0]
                    8100    449 	b1 = bits[1]
                    8200    450 	b2 = bits[2]
                    8300    451 	b3 = bits[3]
                    8400    452 	b4 = bits[4]
                    8500    453 	b5 = bits[5]
                    8600    454 	b6 = bits[6]
                    8700    455 	b7 = bits[7]
                            456 ;--------------------------------------------------------
                            457 ; internal ram data
                            458 ;--------------------------------------------------------
                            459 	.area DSEG    (DATA)
                    0000    460 G$RAM$0$0 == 0x0000
                    0000    461 _RAM	=	0x0000
                    0000    462 G$object_value$0$0==.
   0008                     463 _object_value::
   0008                     464 	.ds 12
                            465 ;--------------------------------------------------------
                            466 ; overlayable items in internal ram 
                            467 ;--------------------------------------------------------
                            468 	.area OSEG    (OVR,DATA)
                            469 ;--------------------------------------------------------
                            470 ; Stack segment in internal ram 
                            471 ;--------------------------------------------------------
                            472 	.area	SSEG	(DATA)
   0074                     473 __start__stack:
   0074                     474 	.ds	1
                            475 
                            476 ;--------------------------------------------------------
                            477 ; indirectly addressable internal ram data
                            478 ;--------------------------------------------------------
                            479 	.area ISEG    (DATA)
                            480 ;--------------------------------------------------------
                            481 ; absolute internal ram data
                            482 ;--------------------------------------------------------
                            483 	.area IABS    (ABS,DATA)
                            484 	.area IABS    (ABS,DATA)
                            485 ;--------------------------------------------------------
                            486 ; bit data
                            487 ;--------------------------------------------------------
                            488 	.area BSEG    (BIT)
                            489 ;--------------------------------------------------------
                            490 ; paged external ram data
                            491 ;--------------------------------------------------------
                            492 	.area PSEG    (PAG,XDATA)
                            493 ;--------------------------------------------------------
                            494 ; external ram data
                            495 ;--------------------------------------------------------
                            496 	.area XSEG    (XDATA)
                            497 ;--------------------------------------------------------
                            498 ; absolute external ram data
                            499 ;--------------------------------------------------------
                            500 	.area XABS    (ABS,XDATA)
                            501 ;--------------------------------------------------------
                            502 ; external initialized ram data
                            503 ;--------------------------------------------------------
                            504 	.area XISEG   (XDATA)
                            505 	.area HOME    (CODE)
                            506 	.area GSINIT0 (CODE)
                            507 	.area GSINIT1 (CODE)
                            508 	.area GSINIT2 (CODE)
                            509 	.area GSINIT3 (CODE)
                            510 	.area GSINIT4 (CODE)
                            511 	.area GSINIT5 (CODE)
                            512 	.area GSINIT  (CODE)
                            513 	.area GSFINAL (CODE)
                            514 	.area CSEG    (CODE)
                            515 ;--------------------------------------------------------
                            516 ; interrupt vector 
                            517 ;--------------------------------------------------------
                            518 	.area HOME    (CODE)
   0000                     519 __interrupt_vect:
   0000 02 00 23            520 	ljmp	__sdcc_gsinit_startup
   0003 32                  521 	reti
   0004                     522 	.ds	7
   000B 02 08 5A            523 	ljmp	_timer0_int
   000E                     524 	.ds	5
   0013 02 0E 17            525 	ljmp	_X1_int
   0016                     526 	.ds	5
   001B 02 0E 47            527 	ljmp	_T1_int
                            528 ;--------------------------------------------------------
                            529 ; global & static initialisations
                            530 ;--------------------------------------------------------
                            531 	.area HOME    (CODE)
                            532 	.area GSINIT  (CODE)
                            533 	.area GSFINAL (CODE)
                            534 	.area GSINIT  (CODE)
                            535 	.globl __sdcc_gsinit_startup
                            536 	.globl __sdcc_program_startup
                            537 	.globl __start__stack
                            538 	.globl __mcs51_genXINIT
                            539 	.globl __mcs51_genXRAMCLEAR
                            540 	.globl __mcs51_genRAMCLEAR
                            541 	.area GSFINAL (CODE)
   007C 02 00 1E            542 	ljmp	__sdcc_program_startup
                            543 ;--------------------------------------------------------
                            544 ; Home
                            545 ;--------------------------------------------------------
                            546 	.area HOME    (CODE)
                            547 	.area HOME    (CODE)
   001E                     548 __sdcc_program_startup:
   001E 12 00 7F            549 	lcall	_main
                            550 ;	return from main will lock up
   0021 80 FE               551 	sjmp .
                            552 ;--------------------------------------------------------
                            553 ; code
                            554 ;--------------------------------------------------------
                            555 	.area CSEG    (CODE)
                            556 ;------------------------------------------------------------
                            557 ;Allocation info for local variables in function 'main'
                            558 ;------------------------------------------------------------
                            559 ;n                         Allocated to registers r5 
                            560 ;LED                       Allocated to registers 
                            561 ;cmd                       Allocated to registers r5 
                            562 ;tasterpegel               Allocated to registers r7 
                            563 ;blink                     Allocated to registers 
                            564 ;verstell                  Allocated to registers b2 
                            565 ;verstellt                 Allocated to registers b1 
                            566 ;tastergetoggelt           Allocated to registers b0 
                            567 ;cal                       Allocated to registers r6 
                            568 ;buttonpattern             Allocated to registers 
                            569 ;wduf                      Allocated to registers b1 
                            570 ;------------------------------------------------------------
                    0000    571 	G$main$0$0 ==.
                    0000    572 	C$fb_taster.c$74$0$0 ==.
                            573 ;	../fb_taster.c:74: void main(void)
                            574 ;	-----------------------------------------
                            575 ;	 function main
                            576 ;	-----------------------------------------
   007F                     577 _main:
                    0007    578 	ar7 = 0x07
                    0006    579 	ar6 = 0x06
                    0005    580 	ar5 = 0x05
                    0004    581 	ar4 = 0x04
                    0003    582 	ar3 = 0x03
                    0002    583 	ar2 = 0x02
                    0001    584 	ar1 = 0x01
                    0000    585 	ar0 = 0x00
                    0000    586 	C$fb_taster.c$76$1$0 ==.
                            587 ;	../fb_taster.c:76: unsigned char n,LED,cmd,tasterpegel=0;
   007F 7F 00               588 	mov	r7,#0x00
                    0002    589 	C$fb_taster.c$77$1$0 ==.
                            590 ;	../fb_taster.c:77: __bit blink, verstell, verstellt,tastergetoggelt=0;
   0081 C2 18               591 	clr	b0
                    0004    592 	C$fb_taster.c$84$1$1 ==.
                            593 ;	../fb_taster.c:84: wduf=WDCON&0x02;
   0083 E5 A7               594 	mov	a,_WDCON
   0085 03                  595 	rr	a
   0086 54 01               596 	anl	a,#0x01
   0088 24 FF               597 	add	a,#0xff
   008A 92 19               598 	mov	b1,c
                    000D    599 	C$fb_taster.c$86$1$1 ==.
                            600 ;	../fb_taster.c:86: restart_hw();							// Hardware zuruecksetzen
   008C C0 07               601 	push	ar7
   008E C0 23               602 	push	bits
   0090 12 17 E4            603 	lcall	_restart_hw
   0093 D0 23               604 	pop	bits
   0095 D0 07               605 	pop	ar7
                    0018    606 	C$fb_taster.c$92$1$1 ==.
                            607 ;	../fb_taster.c:92: TASTER=1;
   0097 D2 97               608 	setb	_P1_7
                    001A    609 	C$fb_taster.c$93$1$1 ==.
                            610 ;	../fb_taster.c:93: if(!TASTER && wduf)cal=0;
   0099 20 97 07            611 	jb	_P1_7,00102$
   009C 30 19 04            612 	jnb	b1,00102$
   009F 7E 00               613 	mov	r6,#0x00
   00A1 80 07               614 	sjmp	00103$
   00A3                     615 00102$:
                    0024    616 	C$fb_taster.c$94$1$1 ==.
                            617 ;	../fb_taster.c:94: else cal=trimsave;
   00A3 90 1C FF            618 	mov	dptr,#_main_trimsave_1_1
   00A6 E4                  619 	clr	a
   00A7 93                  620 	movc	a,@a+dptr
   00A8 FD                  621 	mov	r5,a
   00A9 FE                  622 	mov	r6,a
   00AA                     623 00103$:
                    002B    624 	C$fb_taster.c$96$1$1 ==.
                            625 ;	../fb_taster.c:96: TRIM = (TRIM+trimsave);
   00AA 90 1C FF            626 	mov	dptr,#_main_trimsave_1_1
   00AD E4                  627 	clr	a
   00AE 93                  628 	movc	a,@a+dptr
   00AF AC 96               629 	mov	r4,_TRIM
   00B1 2C                  630 	add	a,r4
   00B2 FD                  631 	mov	r5,a
   00B3 8D 96               632 	mov	_TRIM,r5
                    0036    633 	C$fb_taster.c$97$1$1 ==.
                            634 ;	../fb_taster.c:97: TRIM &= 0x3F;//oberen 2 bits ausblenden
   00B5 53 96 3F            635 	anl	_TRIM,#0x3F
                    0039    636 	C$fb_taster.c$98$2$2 ==.
                            637 ;	../fb_taster.c:98: WATCHDOG_INIT
   00B8 75 C1 FF            638 	mov	_WDL,#0xFF
   00BB C2 AF               639 	clr	_IEN0_7
   00BD 75 A7 E5            640 	mov	_WDCON,#0xE5
   00C0 75 C2 A5            641 	mov	_WFEED1,#0xA5
   00C3 75 C3 5A            642 	mov	_WFEED2,#0x5A
   00C6 D2 AF               643 	setb	_IEN0_7
                    0049    644 	C$fb_taster.c$99$2$3 ==.
                            645 ;	../fb_taster.c:99: WATCHDOG_START
   00C8 C2 AF               646 	clr	_IEN0_7
   00CA 43 A7 04            647 	orl	_WDCON,#0x04
   00CD 75 C2 A5            648 	mov	_WFEED1,#0xA5
   00D0 75 C3 5A            649 	mov	_WFEED2,#0x5A
   00D3 D2 AF               650 	setb	_IEN0_7
                    0056    651 	C$fb_taster.c$100$1$1 ==.
                            652 ;	../fb_taster.c:100: TASTER=0;
   00D5 C2 97               653 	clr	_P1_7
                    0058    654 	C$fb_taster.c$101$1$1 ==.
                            655 ;	../fb_taster.c:101: for (n=0;n<50;n++) {
   00D7 7D 00               656 	mov	r5,#0x00
   00D9                     657 00187$:
   00D9 BD 32 00            658 	cjne	r5,#0x32,00250$
   00DC                     659 00250$:
   00DC 50 1A               660 	jnc	00190$
                    005F    661 	C$fb_taster.c$102$2$4 ==.
                            662 ;	../fb_taster.c:102: TR0=0;					// Timer 0 anhalten
   00DE C2 8C               663 	clr	_TCON_4
                    0061    664 	C$fb_taster.c$103$2$4 ==.
                            665 ;	../fb_taster.c:103: TH0=eeprom[ADDRTAB+1];	// Timer 0 setzen mit phys. Adr. damit Ger�te unterschiedlich beginnen zu senden
   00E0 90 1D 17            666 	mov	dptr,#(_eeprom + 0x0017)
   00E3 E4                  667 	clr	a
   00E4 93                  668 	movc	a,@a+dptr
   00E5 F5 8C               669 	mov	_TH0,a
                    0068    670 	C$fb_taster.c$104$2$4 ==.
                            671 ;	../fb_taster.c:104: TL0=eeprom[ADDRTAB+2];
   00E7 90 1D 18            672 	mov	dptr,#(_eeprom + 0x0018)
   00EA E4                  673 	clr	a
   00EB 93                  674 	movc	a,@a+dptr
   00EC F5 8A               675 	mov	_TL0,a
                    006F    676 	C$fb_taster.c$105$2$4 ==.
                            677 ;	../fb_taster.c:105: TF0=0;					// �berlauf-Flag zur�cksetzen
   00EE C2 8D               678 	clr	_TCON_5
                    0071    679 	C$fb_taster.c$106$2$4 ==.
                            680 ;	../fb_taster.c:106: TR0=1;					// Timer 0 starten
   00F0 D2 8C               681 	setb	_TCON_4
                    0073    682 	C$fb_taster.c$107$2$4 ==.
                            683 ;	../fb_taster.c:107: while(!TF0);
   00F2                     684 00105$:
   00F2 30 8D FD            685 	jnb	_TCON_5,00105$
                    0076    686 	C$fb_taster.c$101$1$1 ==.
                            687 ;	../fb_taster.c:101: for (n=0;n<50;n++) {
   00F5 0D                  688 	inc	r5
   00F6 80 E1               689 	sjmp	00187$
   00F8                     690 00190$:
                    0079    691 	C$fb_taster.c$109$1$1 ==.
                            692 ;	../fb_taster.c:109: restart_app();							// Anwendungsspezifische Einstellungen zuruecksetzen
   00F8 C0 07               693 	push	ar7
   00FA C0 06               694 	push	ar6
   00FC C0 23               695 	push	bits
   00FE 12 0D 40            696 	lcall	_restart_app
   0101 D0 23               697 	pop	bits
   0103 D0 06               698 	pop	ar6
   0105 D0 07               699 	pop	ar7
                    0088    700 	C$fb_taster.c$112$2$5 ==.
                            701 ;	../fb_taster.c:112: RS_INIT_600
   0107 53 BD FE            702 	anl	_BRGCON,#0xFE
   010A 75 98 50            703 	mov	_SCON,#0x50
   010D 43 BA E0            704 	orl	_SSTAT,#0xE0
   0110 43 BD 02            705 	orl	_BRGCON,#0x02
   0113 75 BF 2F            706 	mov	_BRGR1,#0x2F
   0116 75 BE F0            707 	mov	_BRGR0,#0xF0
   0119 43 BD 01            708 	orl	_BRGCON,#0x01
                    009D    709 	C$fb_taster.c$116$1$1 ==.
                            710 ;	../fb_taster.c:116: SBUF=0x55; // hiernach ist TI==1
   011C 75 99 55            711 	mov	_SBUF,#0x55
                    00A0    712 	C$fb_taster.c$118$1$1 ==.
                            713 ;	../fb_taster.c:118: for (n=0;n<4;n++) switch_led(n,0);	// Alle LEDs gemaess ihren Parametern setzen
   011F 7D 00               714 	mov	r5,#0x00
   0121                     715 00191$:
   0121 BD 04 00            716 	cjne	r5,#0x04,00253$
   0124                     717 00253$:
   0124 50 1D               718 	jnc	00194$
   0126 C2 F0               719 	clr	b[0]
   0128 C0 07               720 	push	ar7
   012A C0 06               721 	push	ar6
   012C C0 05               722 	push	ar5
   012E C0 23               723 	push	bits
   0130 85 F0 23            724 	mov	bits,b
   0133 8D 82               725 	mov	dpl,r5
   0135 12 07 BB            726 	lcall	_switch_led
   0138 D0 23               727 	pop	bits
   013A D0 05               728 	pop	ar5
   013C D0 06               729 	pop	ar6
   013E D0 07               730 	pop	ar7
   0140 0D                  731 	inc	r5
   0141 80 DE               732 	sjmp	00191$
   0143                     733 00194$:
                    00C4    734 	C$fb_taster.c$121$1$1 ==.
                            735 ;	../fb_taster.c:121: verstellt=0;
   0143 C2 19               736 	clr	b1
                    00C6    737 	C$fb_taster.c$122$1$1 ==.
                            738 ;	../fb_taster.c:122: dimmwert = LED_hell;
   0145 90 1C FE            739 	mov	dptr,#_main_LED_hell_1_1
   0148 E4                  740 	clr	a
   0149 93                  741 	movc	a,@a+dptr
   014A F5 2B               742 	mov	_dimmwert,a
                    00CD    743 	C$fb_taster.c$124$1$1 ==.
                            744 ;	../fb_taster.c:124: do  {
   014C                     745 00184$:
                    00CD    746 	C$fb_taster.c$125$3$7 ==.
                            747 ;	../fb_taster.c:125: WATCHDOG_FEED
   014C C2 AF               748 	clr	_IEN0_7
   014E 75 C2 A5            749 	mov	_WFEED1,#0xA5
   0151 75 C3 5A            750 	mov	_WFEED2,#0x5A
   0154 D2 AF               751 	setb	_IEN0_7
                    00D7    752 	C$fb_taster.c$126$2$6 ==.
                            753 ;	../fb_taster.c:126: if (RTCCON>=0x80)	// Realtime clock ueberlauf
   0156 74 80               754 	mov	a,#0x100 - 0x80
   0158 25 D1               755 	add	a,_RTCCON
   015A 50 33               756 	jnc	00115$
                    00DD    757 	C$fb_taster.c$128$3$8 ==.
                            758 ;	../fb_taster.c:128: RTCCON=0x61;// RTC flag l�schen
   015C 75 D1 61            759 	mov	_RTCCON,#0x61
                    00E0    760 	C$fb_taster.c$129$3$8 ==.
                            761 ;	../fb_taster.c:129: if(!connected)delay_timer();// die normal RTC Behandlung
   015F 20 0F 11            762 	jb	_connected,00112$
   0162 C0 07               763 	push	ar7
   0164 C0 06               764 	push	ar6
   0166 C0 23               765 	push	bits
   0168 12 08 79            766 	lcall	_delay_timer
   016B D0 23               767 	pop	bits
   016D D0 06               768 	pop	ar6
   016F D0 07               769 	pop	ar7
   0171 80 1C               770 	sjmp	00115$
   0173                     771 00112$:
                    00F4    772 	C$fb_taster.c$132$4$9 ==.
                            773 ;	../fb_taster.c:132: if(connected_timeout <= 110)// 11x 520ms --> ca 6 Sekunden
   0173 E5 73               774 	mov	a,_connected_timeout
   0175 24 91               775 	add	a,#0xff - 0x6E
   0177 40 04               776 	jc	00109$
                    00FA    777 	C$fb_taster.c$134$5$10 ==.
                            778 ;	../fb_taster.c:134: connected_timeout ++;
   0179 05 73               779 	inc	_connected_timeout
   017B 80 12               780 	sjmp	00115$
   017D                     781 00109$:
                    00FE    782 	C$fb_taster.c$136$4$9 ==.
                            783 ;	../fb_taster.c:136: else send_obj_value(T_DISCONNECT);// wenn timeout dann disconnect, flag und var wird in build_tel() gel�scht
   017D 75 82 85            784 	mov	dpl,#0x85
   0180 C0 07               785 	push	ar7
   0182 C0 06               786 	push	ar6
   0184 C0 23               787 	push	bits
   0186 12 14 82            788 	lcall	_send_obj_value
   0189 D0 23               789 	pop	bits
   018B D0 06               790 	pop	ar6
   018D D0 07               791 	pop	ar7
   018F                     792 00115$:
                    0110    793 	C$fb_taster.c$141$2$6 ==.
                            794 ;	../fb_taster.c:141: n=timer;
                    0110    795 	C$fb_taster.c$143$2$6 ==.
                            796 ;	../fb_taster.c:143: verstell=((n>>2) & 0x01);
   018F E5 24               797 	mov	a,_timer
   0191 FD                  798 	mov	r5,a
   0192 03                  799 	rr	a
   0193 03                  800 	rr	a
   0194 54 01               801 	anl	a,#0x01
   0196 FC                  802 	mov	r4,a
   0197 24 FF               803 	add	a,#0xff
                    011A    804 	C$fb_taster.c$145$2$6 ==.
                            805 ;	../fb_taster.c:145: if (verstell==0)verstellt=0;
   0199 92 1A               806 	mov	b2,c
   019B 40 02               807 	jc	00117$
   019D C2 19               808 	clr	b1
   019F                     809 00117$:
                    0120    810 	C$fb_taster.c$148$2$6 ==.
                            811 ;	../fb_taster.c:148: if (status60 & 0x01){			//wenn progmode aktiv ist...
   019F E5 72               812 	mov	a,_status60
   01A1 30 E0 3C            813 	jnb	acc.0,00137$
                    0125    814 	C$fb_taster.c$150$3$11 ==.
                            815 ;	../fb_taster.c:150: if ((PORT & 0x0F)==0x0E){	// Taste 1 gedr�ck
   01A4 74 0F               816 	mov	a,#0x0F
   01A6 55 80               817 	anl	a,_P0
   01A8 FC                  818 	mov	r4,a
   01A9 BC 0E 15            819 	cjne	r4,#0x0E,00123$
                    012D    820 	C$fb_taster.c$151$4$12 ==.
                            821 ;	../fb_taster.c:151: if ((dimmwert<254) && (verstell==1)&& verstellt==0){
   01AC 74 02               822 	mov	a,#0x100 - 0xFE
   01AE 25 2B               823 	add	a,_dimmwert
   01B0 40 0F               824 	jc	00123$
   01B2 A2 1A               825 	mov	c,b2
   01B4 E4                  826 	clr	a
   01B5 33                  827 	rlc	a
   01B6 FC                  828 	mov	r4,a
   01B7 BC 01 07            829 	cjne	r4,#0x01,00123$
   01BA 20 19 04            830 	jb	b1,00123$
                    013E    831 	C$fb_taster.c$152$5$13 ==.
                            832 ;	../fb_taster.c:152: dimmwert++;
   01BD 05 2B               833 	inc	_dimmwert
                    0140    834 	C$fb_taster.c$153$5$13 ==.
                            835 ;	../fb_taster.c:153: verstellt=1;
   01BF D2 19               836 	setb	b1
   01C1                     837 00123$:
                    0142    838 	C$fb_taster.c$156$3$11 ==.
                            839 ;	../fb_taster.c:156: if ((PORT & 0x0F)==0x0D){ // Taste 2 gedr�ckt
   01C1 74 0F               840 	mov	a,#0x0F
   01C3 55 80               841 	anl	a,_P0
   01C5 FC                  842 	mov	r4,a
   01C6 BC 0D 47            843 	cjne	r4,#0x0D,00138$
                    014A    844 	C$fb_taster.c$157$4$14 ==.
                            845 ;	../fb_taster.c:157: if ((dimmwert>1) && (verstell==1)&& verstellt==0){
   01C9 E5 2B               846 	mov	a,_dimmwert
   01CB 24 FE               847 	add	a,#0xff - 0x01
   01CD 50 41               848 	jnc	00138$
   01CF A2 1A               849 	mov	c,b2
   01D1 E4                  850 	clr	a
   01D2 33                  851 	rlc	a
   01D3 FC                  852 	mov	r4,a
   01D4 BC 01 39            853 	cjne	r4,#0x01,00138$
   01D7 20 19 36            854 	jb	b1,00138$
                    015B    855 	C$fb_taster.c$158$5$15 ==.
                            856 ;	../fb_taster.c:158: dimmwert--;
   01DA 15 2B               857 	dec	_dimmwert
                    015D    858 	C$fb_taster.c$159$5$15 ==.
                            859 ;	../fb_taster.c:159: verstellt=1;
   01DC D2 19               860 	setb	b1
   01DE 80 30               861 	sjmp	00138$
   01E0                     862 00137$:
                    0161    863 	C$fb_taster.c$166$3$16 ==.
                            864 ;	../fb_taster.c:166: if(APPLICATION_RUN)	{// nur wenn im Run modus und nicht connected
   01E0 90 1D 0D            865 	mov	dptr,#(_eeprom + 0x000d)
   01E3 E4                  866 	clr	a
   01E4 93                  867 	movc	a,@a+dptr
   01E5 FC                  868 	mov	r4,a
   01E6 BC FF 27            869 	cjne	r4,#0xFF,00138$
   01E9 20 0F 24            870 	jb	_connected,00138$
   01EC E5 72               871 	mov	a,_status60
   01EE 20 E0 1F            872 	jb	acc.0,00138$
                    0172    873 	C$fb_taster.c$167$4$17 ==.
                            874 ;	../fb_taster.c:167: if ((PORT & 0x0F) != button_buffer) port_changed(PORT & 0x0F);	// ein Taster wurde gedrueckt
   01F1 74 0F               875 	mov	a,#0x0F
   01F3 55 80               876 	anl	a,_P0
   01F5 FC                  877 	mov	r4,a
   01F6 B5 28 02            878 	cjne	a,_button_buffer,00276$
   01F9 80 15               879 	sjmp	00138$
   01FB                     880 00276$:
   01FB 74 0F               881 	mov	a,#0x0F
   01FD 55 80               882 	anl	a,_P0
   01FF F5 82               883 	mov	dpl,a
   0201 C0 07               884 	push	ar7
   0203 C0 06               885 	push	ar6
   0205 C0 23               886 	push	bits
   0207 12 02 C9            887 	lcall	_port_changed
   020A D0 23               888 	pop	bits
   020C D0 06               889 	pop	ar6
   020E D0 07               890 	pop	ar7
   0210                     891 00138$:
                    0191    892 	C$fb_taster.c$171$2$6 ==.
                            893 ;	../fb_taster.c:171: if (tel_arrived || tel_sent) {//
   0210 20 07 03            894 	jb	_tel_arrived,00139$
   0213 30 08 13            895 	jnb	_tel_sent,00140$
   0216                     896 00139$:
                    0197    897 	C$fb_taster.c$172$3$18 ==.
                            898 ;	../fb_taster.c:172: tel_sent=0;
   0216 C2 08               899 	clr	_tel_sent
                    0199    900 	C$fb_taster.c$173$3$18 ==.
                            901 ;	../fb_taster.c:173: process_tel();
   0218 C0 07               902 	push	ar7
   021A C0 06               903 	push	ar6
   021C C0 23               904 	push	bits
   021E 12 14 D5            905 	lcall	_process_tel
   0221 D0 23               906 	pop	bits
   0223 D0 06               907 	pop	ar6
   0225 D0 07               908 	pop	ar7
   0227 80 0A               909 	sjmp	00141$
   0229                     910 00140$:
                    01AA    911 	C$fb_taster.c$176$3$6 ==.
                            912 ;	../fb_taster.c:176: for(n=0;n<100;n++);
   0229 7D 64               913 	mov	r5,#0x64
   022B                     914 00197$:
   022B 8D 04               915 	mov	ar4,r5
   022D 1C                  916 	dec	r4
   022E 8C 05               917 	mov	ar5,r4
   0230 ED                  918 	mov	a,r5
   0231 70 F8               919 	jnz	00197$
   0233                     920 00141$:
                    01B4    921 	C$fb_taster.c$180$2$6 ==.
                            922 ;	../fb_taster.c:180: if (RI){
                    01B4    923 	C$fb_taster.c$181$3$20 ==.
                            924 ;	../fb_taster.c:181: RI=0;
   0233 10 98 02            925 	jbc	_SCON_0,00280$
   0236 80 4A               926 	sjmp	00167$
   0238                     927 00280$:
                    01B9    928 	C$fb_taster.c$182$3$20 ==.
                            929 ;	../fb_taster.c:182: cmd=SBUF;
   0238 AD 99               930 	mov	r5,_SBUF
                    01BB    931 	C$fb_taster.c$183$3$20 ==.
                            932 ;	../fb_taster.c:183: if(cmd=='c'){
   023A BD 63 08            933 	cjne	r5,#0x63,00147$
                    01BE    934 	C$fb_taster.c$184$4$21 ==.
                            935 ;	../fb_taster.c:184: while(!TI);
   023D                     936 00143$:
                    01BE    937 	C$fb_taster.c$185$4$21 ==.
                            938 ;	../fb_taster.c:185: TI=0;
   023D 10 99 02            939 	jbc	_SCON_1,00283$
   0240 80 FB               940 	sjmp	00143$
   0242                     941 00283$:
                    01C3    942 	C$fb_taster.c$186$4$21 ==.
                            943 ;	../fb_taster.c:186: SBUF=0x55;
   0242 75 99 55            944 	mov	_SBUF,#0x55
   0245                     945 00147$:
                    01C6    946 	C$fb_taster.c$188$3$20 ==.
                            947 ;	../fb_taster.c:188: if(cmd=='+'){
   0245 BD 2B 03            948 	cjne	r5,#0x2B,00149$
                    01C9    949 	C$fb_taster.c$189$4$22 ==.
                            950 ;	../fb_taster.c:189: TRIM--;
   0248 15 96               951 	dec	_TRIM
                    01CB    952 	C$fb_taster.c$190$4$22 ==.
                            953 ;	../fb_taster.c:190: cal--;
   024A 1E                  954 	dec	r6
   024B                     955 00149$:
                    01CC    956 	C$fb_taster.c$192$3$20 ==.
                            957 ;	../fb_taster.c:192: if(cmd=='-'){
   024B BD 2D 03            958 	cjne	r5,#0x2D,00151$
                    01CF    959 	C$fb_taster.c$193$4$23 ==.
                            960 ;	../fb_taster.c:193: TRIM++;
   024E 05 96               961 	inc	_TRIM
                    01D1    962 	C$fb_taster.c$194$4$23 ==.
                            963 ;	../fb_taster.c:194: cal++;
   0250 0E                  964 	inc	r6
   0251                     965 00151$:
                    01D2    966 	C$fb_taster.c$196$3$20 ==.
                            967 ;	../fb_taster.c:196: if(cmd=='w'){
   0251 BD 77 12            968 	cjne	r5,#0x77,00153$
                    01D5    969 	C$fb_taster.c$197$4$24 ==.
                            970 ;	../fb_taster.c:197: EA=0;
   0254 C2 AF               971 	clr	_IEN0_7
                    01D7    972 	C$fb_taster.c$198$4$24 ==.
                            973 ;	../fb_taster.c:198: START_WRITECYCLE;	//cal an 0x1cFF schreiben
   0256 75 E4 00            974 	mov	_FMCON,#0x00
                    01DA    975 	C$fb_taster.c$199$4$24 ==.
                            976 ;	../fb_taster.c:199: FMADRH= USERRAM_ADDR_H;
   0259 75 E7 1C            977 	mov	_FMADRH,#0x1C
                    01DD    978 	C$fb_taster.c$200$4$24 ==.
                            979 ;	../fb_taster.c:200: FMADRL= 0xFF;
   025C 75 E6 FF            980 	mov	_FMADRL,#0xFF
                    01E0    981 	C$fb_taster.c$201$4$24 ==.
                            982 ;	../fb_taster.c:201: FMDATA=	cal;
   025F 8E E5               983 	mov	_FMDATA,r6
                    01E2    984 	C$fb_taster.c$202$4$24 ==.
                            985 ;	../fb_taster.c:202: STOP_WRITECYCLE;
   0261 75 E4 68            986 	mov	_FMCON,#0x68
                    01E5    987 	C$fb_taster.c$203$4$24 ==.
                            988 ;	../fb_taster.c:203: EA=1;				//int wieder freigeben
   0264 D2 AF               989 	setb	_IEN0_7
   0266                     990 00153$:
                    01E7    991 	C$fb_taster.c$205$3$20 ==.
                            992 ;	../fb_taster.c:205: if(cmd=='p')status60^=0x81;	// Prog-Bit und Parity-Bit im system_state toggeln
   0266 BD 70 03            993 	cjne	r5,#0x70,00155$
   0269 63 72 81            994 	xrl	_status60,#0x81
   026C                     995 00155$:
                    01ED    996 	C$fb_taster.c$206$3$20 ==.
                            997 ;	../fb_taster.c:206: if(cmd=='v'){
   026C BD 76 08            998 	cjne	r5,#0x76,00160$
                    01F0    999 	C$fb_taster.c$207$4$25 ==.
                           1000 ;	../fb_taster.c:207: while(!TI);
   026F                    1001 00156$:
                    01F0   1002 	C$fb_taster.c$208$4$25 ==.
                           1003 ;	../fb_taster.c:208: TI=0;
   026F 10 99 02           1004 	jbc	_SCON_1,00294$
   0272 80 FB              1005 	sjmp	00156$
   0274                    1006 00294$:
                    01F5   1007 	C$fb_taster.c$209$4$25 ==.
                           1008 ;	../fb_taster.c:209: SBUF=VERSION;
   0274 75 99 6B           1009 	mov	_SBUF,#0x6B
   0277                    1010 00160$:
                    01F8   1011 	C$fb_taster.c$211$3$20 ==.
                           1012 ;	../fb_taster.c:211: if(cmd=='t'){
   0277 BD 74 08           1013 	cjne	r5,#0x74,00167$
                    01FB   1014 	C$fb_taster.c$212$4$26 ==.
                           1015 ;	../fb_taster.c:212: while(!TI);
   027A                    1016 00161$:
                    01FB   1017 	C$fb_taster.c$213$4$26 ==.
                           1018 ;	../fb_taster.c:213: TI=0;
   027A 10 99 02           1019 	jbc	_SCON_1,00297$
   027D 80 FB              1020 	sjmp	00161$
   027F                    1021 00297$:
                    0200   1022 	C$fb_taster.c$214$4$26 ==.
                           1023 ;	../fb_taster.c:214: SBUF=TYPE;
   027F 75 99 00           1024 	mov	_SBUF,#0x00
   0282                    1025 00167$:
                    0203   1026 	C$fb_taster.c$226$2$6 ==.
                           1027 ;	../fb_taster.c:226: TASTER=1;				        	// Pin als Eingang schalten um Programmiertaster abzufragen
   0282 D2 97              1028 	setb	_P1_7
                    0205   1029 	C$fb_taster.c$227$2$6 ==.
                           1030 ;	../fb_taster.c:227: if(!TASTER){ // Taster gedr�ckt
   0284 20 97 2A           1031 	jb	_P1_7,00179$
                    0208   1032 	C$fb_taster.c$228$3$27 ==.
                           1033 ;	../fb_taster.c:228: if(tasterpegel<255)	tasterpegel++;
   0287 BF FF 00           1034 	cjne	r7,#0xFF,00299$
   028A                    1035 00299$:
   028A 50 03              1036 	jnc	00173$
   028C 0F                 1037 	inc	r7
   028D 80 2A              1038 	sjmp	00180$
   028F                    1039 00173$:
                    0210   1040 	C$fb_taster.c$230$4$28 ==.
                           1041 ;	../fb_taster.c:230: if(!tastergetoggelt)status60^=0x81;	// Prog-Bit und Parity-Bit im system_state toggeln
   028F 20 18 03           1042 	jb	b0,00169$
   0292 63 72 81           1043 	xrl	_status60,#0x81
   0295                    1044 00169$:
                    0216   1045 	C$fb_taster.c$231$4$28 ==.
                           1046 ;	../fb_taster.c:231: tastergetoggelt=1;
   0295 D2 18              1047 	setb	b0
                    0218   1048 	C$fb_taster.c$232$4$28 ==.
                           1049 ;	../fb_taster.c:232: if((status60 & 0x01)==0){	//wenn ausgemacht, Dimmwert speichern
   0297 E5 72              1050 	mov	a,_status60
   0299 20 E0 1D           1051 	jb	acc.0,00180$
                    021D   1052 	C$fb_taster.c$233$5$29 ==.
                           1053 ;	../fb_taster.c:233: EA=0;
   029C C2 AF              1054 	clr	_IEN0_7
                    021F   1055 	C$fb_taster.c$234$5$29 ==.
                           1056 ;	../fb_taster.c:234: START_WRITECYCLE;
   029E 75 E4 00           1057 	mov	_FMCON,#0x00
                    0222   1058 	C$fb_taster.c$235$5$29 ==.
                           1059 ;	../fb_taster.c:235: FMADRH= USERRAM_ADDR_H; //0x1C
   02A1 75 E7 1C           1060 	mov	_FMADRH,#0x1C
                    0225   1061 	C$fb_taster.c$236$5$29 ==.
                           1062 ;	../fb_taster.c:236: FMADRL= 0xFE;
   02A4 75 E6 FE           1063 	mov	_FMADRL,#0xFE
                    0228   1064 	C$fb_taster.c$237$5$29 ==.
                           1065 ;	../fb_taster.c:237: FMDATA=	dimmwert;
   02A7 85 2B E5           1066 	mov	_FMDATA,_dimmwert
                    022B   1067 	C$fb_taster.c$238$5$29 ==.
                           1068 ;	../fb_taster.c:238: STOP_WRITECYCLE;
   02AA 75 E4 68           1069 	mov	_FMCON,#0x68
                    022E   1070 	C$fb_taster.c$239$5$29 ==.
                           1071 ;	../fb_taster.c:239: EA=1;
   02AD D2 AF              1072 	setb	_IEN0_7
   02AF 80 08              1073 	sjmp	00180$
   02B1                    1074 00179$:
                    0232   1075 	C$fb_taster.c$244$3$30 ==.
                           1076 ;	../fb_taster.c:244: if(tasterpegel>0) tasterpegel--;
   02B1 EF                 1077 	mov	a,r7
   02B2 60 03              1078 	jz	00176$
   02B4 1F                 1079 	dec	r7
   02B5 80 02              1080 	sjmp	00180$
   02B7                    1081 00176$:
                    0238   1082 	C$fb_taster.c$245$3$30 ==.
                           1083 ;	../fb_taster.c:245: else tastergetoggelt=0;
   02B7 C2 18              1084 	clr	b0
   02B9                    1085 00180$:
                    023A   1086 	C$fb_taster.c$278$2$6 ==.
                           1087 ;	../fb_taster.c:278: if (status60 & 0x01) TASTER = 0;		// LED leuchtet im Prog-Mode
   02B9 E5 72              1088 	mov	a,_status60
   02BB 30 E0 05           1089 	jnb	acc.0,00182$
   02BE C2 97              1090 	clr	_P1_7
   02C0 02 01 4C           1091 	ljmp	00184$
   02C3                    1092 00182$:
                    0244   1093 	C$fb_taster.c$279$2$6 ==.
                           1094 ;	../fb_taster.c:279: else TASTER = 1;						// LED aus
   02C3 D2 97              1095 	setb	_P1_7
                    0246   1096 	C$fb_taster.c$283$1$1 ==.
                           1097 ;	../fb_taster.c:283: }  while(1);
   02C5 02 01 4C           1098 	ljmp	00184$
                    0249   1099 	C$fb_taster.c$284$1$1 ==.
                    0249   1100 	XG$main$0$0 ==.
   02C8 22                 1101 	ret
                           1102 	.area CSEG    (CODE)
                           1103 	.area CONST   (CODE)
                    1CFF   1104 Lfb_taster.main$trimsave$1$1 == 0x1cff
                    1CFF   1105 _main_trimsave_1_1	=	0x1cff
                           1106 	.area XINIT   (CODE)
                           1107 	.area CABS    (ABS,CODE)
   1CFE                    1108 	.org 0x1CFE
                    1CFE   1109 Lfb_taster.main$LED_hell$1$1 == .
   1CFE                    1110 _main_LED_hell_1_1:
   1CFE FF                 1111 	.db #0xFF	; 255
