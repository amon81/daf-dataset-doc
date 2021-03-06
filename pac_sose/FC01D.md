# SOSE: FC01D Comuni - Altri Servizi Generali - Fabbisogni, caratteristiche e prestazioni

## Descrizione del dataset


**Tipo di dataset:** standard/ordinary?

**Tipo di flusso:** batch

**Tipo di file:** CSV

**Scheda:** 

**Modalità di ingestion su DAF:** scarico su SFTP


## Elementi

| Nome | Tipo   | Descrizione                     |
|------|--------|---------------------------------|
| ANNO | number | Anno di analisi  |
| COMUNE_CAT_COD | string  | codice catastale del comune |
| CAT_DET_COD_1 |  | Popolazione residente
| CAT_DET_COD_2 |  | Morfologia e territorio
| CAT_DET_COD_3 |  | Prezzi degli input
| CAT_DET_COD_4 |  | Fattori esogeni di carico
| CAT_DET_COD_5 |  | Scelte organizzative
| COEFF_TEORICO |  | Coefficiente di Fabbisogno Standard per il Comune |
| IND1 |  | Spesa storica degli altri servizi generali per abitante(€)
| IND3 |  | Spesa storica vs fabbisogno standard(%)
| IND4 |  | Livello servizi offerti vs livello servizi standard(%)
| IND5 |  | Delibere per 1.000 abitanti(numero)
| IND6 |  | Sedute per 1.000 abitanti(numero)
| IND7 |  | Bollette servizi domanda individuale per 1.000 abitanti(numero)
| IND8 |  | Rinnovi e concessioni beni demaniali per 1.000 abitanti(numero)
| IND9 |  | Nuove cause per 1.000 abitanti(numero)
| IND10 |  | Contratti di lavoro dipendente per 1.000 abitanti(numero)
| LQP_COD_1 |  | Differenza tra spesa storica e fabbisogno standard in % rispetto al fabbisogno standard |
| LQP_COD_2 |  | Differenza tra livello dei servizi storico e livello dei servizi standard in % rispetto al livello dei servizi standard |
| LQP_COD_3 |  | Flag Comune non valutabile |
| LQP_COD_4 |  | Flag percentile anomalo (differenza % minore del 5^ percentile o maggiore del 95^ percentile) |
| LQP_COD_5 |  | Posizione del Comune rispetto alla spesa |
| LQP_COD_6 |  | Posizione del Comune rispetto al livello dei servizi |
| LQP_COD_S |  | Misura (da 0 a 10) della capacità del Comune di soddisfare la domanda di servizi espressa dai cittadini, tenendo conto della spesa e dei servizi offerti rispetto allo standard | 

## Esempio del flusso

```
"ANNO";"COMUNE_CAT_COD";"CAT_DET_COD_1";"CAT_DET_COD_2";"CAT_DET_COD_3";"CAT_DET_COD_4";"CAT_DET_COD_5";"COEFF_TEORICO";"IND1";"IND3";"IND4";"IND5";"IND6";"IND7";"IND8";"IND9";"IND10";"LQP_COD_1";"LQP_COD_2";"LQP_COD_3";"LQP_COD_4";"LQP_COD_5";"LQP_COD_6";"LQP_COD_S"
"2010";"A052";"0.131083788";"0.096739953";"0.443118107";"0.329058152";"0";"0.000319431";"117.9167234";"18.79283821";"-1.039833441";"15.40417624";"3.863269598";"40.09976038";"11.68761309";"1.320357964";"0.391217174";"18.79283821";"-1.039833441";"0";"0";"8";"5";"4.2"
"2010";"A146";"0.690440811";"0.029266629";"0.030336613";"0.249955947";"0";"1.4377E-05";"214.7374613";"-24.45952022";"-14.61055881";"201.183432";"68.04733728";"0";"0";"0";"0";"-24.45952022";"-14.61055881";"0";"0";"2";"3";"5.4"
"2010";"A182";"0.174695156";"0.062993495";"0.407741949";"0.3545694";"0";"0.001695795";"170.6677227";"49.66502016";"-12.52593872";"6.051533586";"4.586425455";"0";"0";"8.143028527";"1.295240522";"49.66502016";"-12.52593872";"0";"0";"10";"4";"2.8"
"2010";"A189";"0.557291505";"0.036201941";"0.081004744";"0.32550181";"0";"2.14301E-05";"165.8129534";"-6.470215771";"-6.100977778";"118.4895833";"33.85416667";"104.1666667";"10.41666667";"0";"0";"-6.470215771";"-6.100977778";"0";"0";"4";"4";"5.2"
"2010";"A197";"0.541619929";"0.053754491";"0.094699346";"0.309926235";"0";"2.19879E-05";"138.3078105";"-23.07789241";"3.553509822";"137.4045802";"50.89058524";"0";"0";"1.272264631";"0";"-23.07789241";"3.553509822";"0";"0";"2";"6";"7.2"
"2010";"A211";"0.587608713";"0.01348665";"0.122417763";"0.276486874";"0";"2.41511E-05";"140.501927";"-10.18291087";"-22.87075824";"66.86930091";"22.28976697";"0";"0";"0";"0";"-10.18291087";"-22.87075824";"0";"0";"4";"2";"4"
"2010";"A227";"0.620607276";"0.024626816";"0.109093219";"0.245672688";"0";"1.66296E-05";"218.4926877";"4.098063";"15.56093421";"189.0838207";"48.73294347";"0";"0";"0";"0";"4.098063";"15.56093421";"0";"0";"6";"8";"6.8"
"2010";"A245";"0.717316708";"0.006425886";"0.102414676";"0.17384273";"0";"1.49415E-05";"196.1358013";"-21.89402458";"1.725793543";"132.5966851";"48.80294659";"303.8674033";"0";"0";"0";"-21.89402458";"1.725793543";"0";"0";"2";"6";"7.2"
"2010";"A436";"0.16722803";"0.075176904";"0.26384259";"0.493752476";"0";"0.000104585";"115.6994888";"8.436062348";"2.340367278";"22.70884023";"11.19221411";"0";"1.459854015";"0";"0";"8.436062348";"2.340367278";"0";"0";"7";"6";"5.2"
"2010";"A523";"0.763061856";"0.028812856";"0.046234361";"0.161890927";"0";"1.27898E-05";"361.5218121";"31.8934048";"-11.07095944";"227.8911565";"85.03401361";"170.0680272";"0";"0";"3.401360544";"31.8934048";"-11.07095944";"0";"0";"9";"4";"3.2"
"2010";"A605";"0.460625716";"0.023851579";"0.18332578";"0.332196926";"0";"3.08721E-05";"161.8568118";"16.89935402";"16.52201821";"108.8765603";"25.65880721";"0";"6.93481276";"0";"0";"16.89935402";"16.52201821";"0";"0";"7";"8";"6.4"
"2010";"A689";"0.416408651";"0.039510202";"0.195236796";"0.34884435";"0";"3.91802E-05";"109.3030289";"-7.699747213";"-17.62117512";"48.24976348";"19.86754967";"0";"0";"0";"0.473036897";"-7.699747213";"-17.62117512";"0";"0";"4";"3";"4.6"
"2010";"A708";"0.39965278";"0.020660443";"0.222637134";"0.357049643";"0";"3.71991E-05";"150.8602709";"12.52375823";"18.40368964";"34.15453527";"15.6774916";"151.1758119";"0";"0";"0";"12.52375823";"18.40368964";"0";"0";"7";"8";"6.4"
"2010";"A738";"0.596643678";"0.0250591";"0.05754088";"0.320756342";"0";"1.80588E-05";"245.8397206";"6.791842197";"-0.64961065";"147.4358974";"38.46153846";"0";"0";"0";"0";"6.791842197";"-0.64961065";"0";"0";"6";"5";"5"
"2010";"A793";"0.586076236";"0.021868531";"0.100181447";"0.291873786";"0";"2.09945E-05";"252.3222926";"46.78549552";"27.47621413";"152.2012579";"62.26415094";"313.836478";"1.886792453";"0.628930818";"0";"46.78549552";"27.47621413";"0";"0";"9";"9";"6.2"
"2010";"A813";"0.753319075";"0.010203751";"0.025772917";"0.210704257";"0";"1.05184E-05";"356.0776471";"-9.888299527";"-34.60167891";"283.1325301";"102.4096386";"0";"0";"0";"0";"-9.888299527";"-34.60167891";"0";"0";"4";"1";"3.4"
"2010";"A889";"0.404208481";"0.041125502";"0.172250633";"0.382415383";"0";"3.88973E-05";"110.3252572";"-13.66458617";"60.62831563";"57.02436496";"17.6257128";"4976.671851";"1.036806636";"0";"0";"-13.66458617";"60.62831563";"0";"2";"3";"10";"9.2"
"2010";"A998";"0.376136191";"0.06737055";"0.128135269";"0.42835799";"0";"3.94217E-05";"140.0341463";"11.74178031";"8.794733346";"80.89330025";"23.82133995";"397.0223325";"0";"0";"0";"11.74178031";"8.794733346";"0";"0";"7";"7";"5.8"

```

