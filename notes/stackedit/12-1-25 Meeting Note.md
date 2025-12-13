


> Written with [StackEdit](https://stackedit.io/).
# 12-1-25 Meeting Note
![Horizontal Layout](https://raw.githubusercontent.com/happyandslow/cs_sdk/main/csl-extras-202505230211-4-d9070058/examples/demo/gemv-h2d-multiple-pes-two-tenants/gemv-h2d-two.png)

https://github.com/happyandslow/cs_sdk/tree/main/csl-extras-202505230211-4-d9070058/examples/demo/gemv-h2d-multiple-pes-two-tenants-horizonal

![Horizontal Layout](https://raw.githubusercontent.com/happyandslow/cs_sdk/main/csl-extras-202505230211-4-d9070058/examples/demo/gemv-h2d-multiple-pes-two-tenants/gemv-h2d-two-vertical.png)

https://github.com/happyandslow/cs_sdk/tree/main/csl-extras-202505230211-4-d9070058/examples/demo/gemv-h2d-multiple-pes-two-tenants


## Comparing 1*4 kernels side-by-side

### 2 Iterations with single memcpy and compute
Vertical Layout (2 Iterations)

    metric count mean stddev min p25 p50 p75 max
    ------------------------------------------------------------------------------------------------------------------------------------------  
    cycle_count 10  46761.4  10208.6  36295  38642.8  43995.5  51811.2  66195    
    cycles_per_second 10  16047.6  5693.57  10284.4  11218.1  14480.1  19286  25246.4    
    fabric_x 10  11  0  11  11  11  11  11    
    fabric_y 10  4  0  4  4  4  4  4   
    hwtile_count 10  22  0  22  22  22  22  22    
    idle_ce_cycles 10  24216.7  9535.46  14248  16674.2  22243.5  28409.8  42639    
    idle_wavelet_cycles 10  24252.7  9535.46  14284  16710.2  22279.5  28445.8  42675    
    init_time 10  0.0322554  0.0023908  0.029521  0.0306993  0.0311811  0.0329807  0.0366311    
    iotile_count 10  4  0  4  4  4  4  4    
    nodes 10  1  0  1  1  1  1  1    
    nultile_count 10  48  0  48  48  48  48  48    
    sim_time 10  3.04425  0.46249  2.39171  2.6894  2.9982  3.31186  3.78715    
    simulated_tile_count 10  26  0  26  26  26  26  26    
    sunset_count 10  0  0  0  0  0  0  0    
    threads 10  5  0  5  5  5  5  5    
    tile_count 10  74  0  74  74  74  74  74    
    tile_cycles_per_second 10  417236  148033  267394  291670  376482  501435  656406    
    tile_cycles_per_second_per_thread 10  83447.3  29606.6  53478.7  58333.9  75296.3  100287  131281   
    total_time 10  3.0765  0.462769  2.42123  2.72191  3.03185  3.34757  3.81781
        
        

Horizontal Layout (2 iterations)


    metric count mean stddev min p25 p50 p75 max    
    ------------------------------------------------------------------------------------------------------------------------------------------    
    cycle_count 10  46973.9  9032.91  37021  40133.8  44255  52892.5  63999    
    cycles_per_second 10  14203.7  4245.05  9039  11317.4  13517.3  16463.7  21244.4    
    fabric_x 10  15  0  15  15  15  15  15    
    fabric_y 10  3  0  3  3  3  3  3    
    hwtile_count 10  17  0  17  17  17  17  17    
    idle_ce_cycles 10  24212.3  8979.98  14918  17760  20836.5  30180  41510    
    idle_wavelet_cycles 10  24267.3  8979.98  14973  17815  20891.5  30235  41565    
    init_time 10  0.0283541  0.00164099  0.0264111  0.0271699  0.0278826  0.0297654  0.03069   
    iotile_count 10  4  0  4  4  4  4  4    
    nodes 10  1  0  1  1  1  1  1    
    nultile_count 10  60  0  60  60  60  60  60    
    sim_time 10  3.41647  0.470655  2.86544  3.03209  3.42082  3.66098  4.17313    
    simulated_tile_count 10  21  0  21  21  21  21  21    
    sunset_count 10  0  0  0  0  0  0  0    
    threads 10  5  0  5  5  5  5  5   
    tile_count 10  81  0  81  81  81  81  81    
    tile_cycles_per_second 10  298279  89146  189819  237666  283864  345737  446133    
    tile_cycles_per_second_per_thread 10  59655.7  17829.2  37963.8  47533.2  56772.7  69147.3  89226.6    
    total_time 10  3.44482  0.471059  2.89604  3.06081  3.44816  3.68816  4.20311


### 10 Iterations with single memcpy and compute


Vertical Layout (10 Iterations)

    metric                      count           mean         stddev            min            p25            p50            p75            max
    ------------------------------------------------------------------------------------------------------------------------------------------
    cycle_count                    10         125435        6920.86         116842         121031         125154         128450         140549
    cycles_per_second              10        10828.6         2037.6        7736.92        9274.07        10493.4        12163.3        13871.1
    fabric_x                       10             11              0             11             11             11             11             11
    fabric_y                       10              4              0              4              4              4              4              4
    hwtile_count                   10             22              0             22             22             22             22             22
    idle_ce_cycles                 10        23548.5        7149.74          15726        18401.5          22981        26423.8          39442
    idle_wavelet_cycles            10        23584.5        7149.74          15762        18437.5          23017        26459.8          39478
    init_time                      10      0.0693907      0.0166098      0.0303891      0.0658712       0.068144      0.0788336       0.089931
    iotile_count                   10              4              0              4              4              4              4              4
    nodes                          10              1              0              1              1              1              1              1
    nultile_count                  10             48              0             48             48             48             48             48
    sim_time                       10        11.8887        1.84913        9.12147        11.0402        11.8142         12.995        15.1019
    simulated_tile_count           10             26              0             26             26             26             26             26
    sunset_count                   10              0              0              0              0              0              0              0
    threads                        10              5              0              5              5              5              5              5
    tile_count                     10             74              0             74             74             74             74             74
    tile_cycles_per_second         10         281543        52977.6         201160         241126         272827         316245         360648
    tile_cycles_per_second_per_thread     10        56308.6        10595.5          40232        48225.2        54565.5        63249.1        72129.5
    total_time                     10         11.958        1.85909        9.18755        11.1099        11.8925         13.061        15.1897

Horizontal Layout (10 Iterations)

    metric                      count           mean         stddev            min            p25            p50            p75            max
    ------------------------------------------------------------------------------------------------------------------------------------------
    cycle_count                    10         130990        10830.2         119911         121688         128575         135322         149732
    cycles_per_second              10          10147         2837.8        7594.06        8277.59        9563.56          11133          17004
    fabric_x                       10             15              0             15             15             15             15             15
    fabric_y                       10              3              0              3              3              3              3              3
    hwtile_count                   10             17              0             17             17             17             17             17
    idle_ce_cycles                 10          25675        10677.6          14347        16815.5        23227.5        29955.8          43641
    idle_wavelet_cycles            10          25730        10677.6          14402        16870.5        23282.5        30010.8          43696
    init_time                      10       0.066142      0.0157478       0.031801      0.0591087      0.0676404      0.0789888       0.082206
    iotile_count                   10              4              0              4              4              4              4              4
    nodes                          10              1              0              1              1              1              1              1
    nultile_count                  10             60              0             60             60             60             60             60
    sim_time                       10        13.4398        2.16316        8.80571        12.4819        13.7572        14.8982        15.8689
    simulated_tile_count           10             21              0             21             21             21             21             21
    sunset_count                   10              0              0              0              0              0              0              0
    threads                        10              5              0              5              5              5              5              5
    tile_count                     10             81              0             81             81             81             81             81
    tile_cycles_per_second         10         213087        59593.7         159475         173829         200835         233792         357083
    tile_cycles_per_second_per_thread     10        42617.4        11918.7        31895.1        34765.9        40166.9        46758.5        71416.7
    total_time                     10        13.5059        2.16122        8.88524        12.5207        13.8348        14.9573         15.926


### 2 Iterations with single memcpy and 10 x compute

Vertical Layout

    metric                      count           mean         stddev            min            p25            p50            p75            max
    ------------------------------------------------------------------------------------------------------------------------------------------
    cycle_count                    10        52818.2        10225.7          44366          45959          47990        58884.5          74729
    cycles_per_second              10        12798.7        4484.03        8138.38        10123.6        11735.7        13142.1        23798.4
    fabric_x                       10             11              0             11             11             11             11             11
    fabric_y                       10              4              0              4              4              4              4              4
    hwtile_count                   10             22              0             22             22             22             22             22
    idle_ce_cycles                 10          21807        9669.41          14067        15049.5          17293          27304          42364
    idle_wavelet_cycles            10          21843        9669.41          14103        15085.5          17329          27340          42400
    init_time                      10      0.0406059      0.0103537       0.033648      0.0358059       0.036755       0.040313      0.0687821
    iotile_count                   10              4              0              4              4              4              4              4
    nodes                          10              1              0              1              1              1              1              1
    nultile_count                  10             48              0             48             48             48             48             48
    sim_time                       10        4.30005       0.660048        3.14009        3.84667        4.45663        4.63277        5.45145
    simulated_tile_count           10             26              0             26             26             26             26             26
    sunset_count                   10              0              0              0              0              0              0              0
    threads                        10              5              0              5              5              5              5              5
    tile_count                     10             74              0             74             74             74             74             74
    tile_cycles_per_second         10         332766         116585         211598         263215         305129         341694         618757
    tile_cycles_per_second_per_thread     10        66553.1          23317        42319.6        52642.9        61025.8        68338.9         123751
    total_time                     10        4.34065       0.657292        3.17687        3.89049        4.49558        4.67027        5.48642


Horizontal Layout

    metric                      count           mean         stddev            min            p25            p50            p75            max
    ------------------------------------------------------------------------------------------------------------------------------------------
    cycle_count                    10        55421.7        10357.6          45138        46344.2          53271        59809.2          73621
    cycles_per_second              10        11468.1        3787.58        7637.07        9016.43        10047.7        13227.2        18823.8
    fabric_x                       10             15              0             15             15             15             15             15
    fabric_y                       10              3              0              3              3              3              3              3
    hwtile_count                   10             17              0             17             17             17             17             17
    idle_ce_cycles                 10        24095.4        10124.7          14507        15631.5        21510.5          28366          42914
    idle_wavelet_cycles            10        24150.4        10124.7          14562        15686.5        21565.5          28421          42969
    init_time                      10      0.0400846      0.0130995      0.0309448      0.0326537      0.0374765      0.0400236      0.0757778
    iotile_count                   10              4              0              4              4              4              4              4
    nodes                          10              1              0              1              1              1              1              1
    nultile_count                  10             60              0             60             60             60             60             60
    sim_time                       10        5.02384       0.687986        3.77337        4.54604        5.01124        5.60599        5.91038
    simulated_tile_count           10             21              0             21             21             21             21             21
    sunset_count                   10              0              0              0              0              0              0              0
    threads                        10              5              0              5              5              5              5              5
    tile_count                     10             81              0             81             81             81             81             81
    tile_cycles_per_second         10         240830        79539.1         160378         189345         211001         277772         395299
    tile_cycles_per_second_per_thread     10          48166        15907.8        32075.7          37869        42200.1        55554.4        79059.8
    total_time                     10        5.06393       0.692825        3.80431        4.58548        5.04832        5.63884        5.98616


### 2 Iterations with single memcpy and 50 x compute

Vertical Layout

    metric                      count           mean         stddev            min            p25            p50            p75            max
    ------------------------------------------------------------------------------------------------------------------------------------------
    cycle_count                    10        93748.4        5242.77          85065          91060        95339.5          96506         102582
    cycles_per_second              10        10727.5        1714.83        7826.58        9394.24        10848.7          12077        12801.9
    fabric_x                       10             11              0             11             11             11             11             11
    fabric_y                       10              4              0              4              4              4              4              4
    hwtile_count                   10             22              0             22             22             22             22             22
    idle_ce_cycles                 10        24431.9        5313.73          15914        22064.5          25640        27515.8          33093
    idle_wavelet_cycles            10        24467.9        5313.73          15950        22100.5          25676        27551.8          33129
    init_time                      10       0.058961      0.0093474      0.0353189      0.0586743       0.059738       0.061956      0.0725899
    iotile_count                   10              4              0              4              4              4              4              4
    nodes                          10              1              0              1              1              1              1              1
    nultile_count                  10             48              0             48             48             48             48             48
    sim_time                       10        8.89136        1.07938        7.38655        8.17505         8.8842        9.57714        10.8687
    simulated_tile_count           10             26              0             26             26             26             26             26
    sunset_count                   10              0              0              0              0              0              0              0
    threads                        10              5              0              5              5              5              5              5
    tile_count                     10             74              0             74             74             74             74             74
    tile_cycles_per_second         10         278916        44585.5         203491         244250         282067         314003         332850
    tile_cycles_per_second_per_thread     10        55783.3         8917.1        40698.2        48850.1        56413.4        62800.5        66569.9
    total_time                     10        8.95032         1.0779        7.44884        8.23304        8.94613        9.64683        10.9282

Horizontal Layout

    metric                      count           mean         stddev            min            p25            p50            p75            max
    ------------------------------------------------------------------------------------------------------------------------------------------
    cycle_count                    10        97647.5        8022.51          87910        93995.5        95196.5        99443.8         117358
    cycles_per_second              10        9900.58         2260.3        8225.53        8506.79        9104.97        9779.21        15330.7
    fabric_x                       10             15              0             15             15             15             15             15
    fabric_y                       10              3              0              3              3              3              3              3
    hwtile_count                   10             17              0             17             17             17             17             17
    idle_ce_cycles                 10        27235.7        7630.04          17905        24340.5        24792.5        29402.2          45592
    idle_wavelet_cycles            10        27290.7        7630.04          17960        24395.5        24847.5        29457.2          45647
    init_time                      10      0.0603226      0.0126066      0.0365732      0.0535103      0.0601815      0.0650843       0.079649
    iotile_count                   10              4              0              4              4              4              4              4
    nodes                          10              1              0              1              1              1              1              1
    nultile_count                  10             60              0             60             60             60             60             60
    sim_time                       10        10.1091        1.27679         7.6551        9.83759        10.2127         11.199        11.4163
    simulated_tile_count           10             21              0             21             21             21             21             21
    sunset_count                   10              0              0              0              0              0              0              0
    threads                        10              5              0              5              5              5              5              5
    tile_count                     10             81              0             81             81             81             81             81
    tile_cycles_per_second         10         207912        47466.2         172736         178643         191204         205363         321945
    tile_cycles_per_second_per_thread     10        41582.5        9493.25        34547.2        35728.5        38240.9        41072.7          64389
    total_time                     10        10.1694        1.28014         7.7113         9.8906        10.2826        11.2573         11.496

## TODO

1. Move right 1x4 to the right bottom corner
2. Control + Data color

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTUwODc0MjU4MCwxNzk3NzA1OTUzXX0=
-->