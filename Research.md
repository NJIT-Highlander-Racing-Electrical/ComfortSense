https://www.sparkfun.com/datasheets/Sensors/Pressure/fsrguide.pdf
link to a guide on fsrs- they are expensive and can be finiky with retesting/calibration
my other idea was too use some type of velostat and make a mat like
https://hackaday.com/2017/10/29/hi-res-body-sized-pressure-sensor-mat/

FSR/Velostat mat
pro-
can make a really pretty matrix model to show force over the entire chair

con
expensive
can be finicky with set up or with weather/being outside
unsure with max weight-some said like 50 g



leaning toward bathroom scale bc its cheap and easy-
https://www.amazon.com/Half-bridge-Weighting-Sensor-Amplifier-Geekstory/dp/B079FTXR7Y/ref=asc_df_B079FTXR7Y/?tag=hyprod-20&linkCode=df0&hvadid=241927124583&hvpos=&hvnetw=g&hvrand=17094551c713363405239&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9003544&hvtargid=pla-426277064612&psc=1

20 pc mcnugs
https://www.amazon.com/dp/B09KGSGL18/ref=sspa_dk_detail_5?psc=1&pd_rd_i=B09KGSGL18&pd_rd_w=fNqa5&content-id=amzn1.sym.f734d1a2-0bf9-4a26-ad34-2e1b969a5a75&pf_rd_p=f734d1a2-0bf9-4a26-ad34-2e1b969a5a75&pf_rd_r=3EGD8T1Y3A7YGRS0SHNX&pd_rd_wg=ZmTqG&pd_rd_r=dab25b5e-46d8-44e1-82d6-65fd21bfd232&s=kitchen&sp_csd=d2lkZ2V0TmFtZT1zcF9kZXRhaWw

can wire up several sets of them to create a matrix of points
cheap and small so if one breaks its easier to swap
each cell can do 50 kg

might need HX711 AD if we want more specific readouts
each cell needs an amplifier to get a reading
bathroom scales combine 4 load cells to 1 amp to get 1 reading

https://www.amazon.com/CHENBO-Weighing-Dual-Channel-Precision-Pressure/dp/B01D1FECVI/ref=pd_bxgy_sccl_1/133-4782788-9217400?pd_rd_w=txPd2&content-id=amzn1.sym.21b577c4-6435-4581-8b53-49da41e27328&pf_rd_p=21b577c4-6435-4581-8b53-49da41e27328&pf_rd_r=7QH2TB9W1ESGWTV4RMJ1&pd_rd_wg=6fArm&pd_rd_r=9729d353-f7f2-438f-8cfc-4bbda5427ffc&pd_rd_i=B01D1FECVI&psc=1

https://cdn.sparkfun.com/assets/learn_tutorials/5/4/6/hx711F_EN.pdf?_gl=1*1ka14cx*_ga*NzU0MTQ4MDEzLjE2OTU2NzQzNTI.*_ga_T369JS7J9N*MTY5NjA5NDIwMy4yLjEuMTY5NjA5NTcwMS42MC4wLjA.



potential multiplex?
do overlapping wheatstone brisges into multiplex
6x6 matrix in canvas sandwich/quilt
use fabrivc glue/stitch sensor in place to keep them flat

https://www.aliexpress.us/item/3256805730336660.html?spm=a2g0o.productlist.main.11.2642tDfvtDfvS5&algo_pvid=02e34afe-7658-452d-abd0-6aa0b64624a9&algo_exp_id=02e34afe-7658-452d-abd0-6aa0b64624a9-5&pdp_npi=4%40dis%21USD%2111.27%2110.71%21%21%2111.27%21%21%40210313e916970541158781993e17ec%2112000034838587966%21sea%21US%210%21AB&curPageLogUid=cQXEl6BgZatw

https://www.aliexpress.us/item/3256805792961653.html?spm=a2g0o.detail.0.0.eb87dN0rdN0rIs&mp=1&gatewayAdapt=glo2usa




will need hx711 board
online ppl tried with just an op amp and failed (https://forum.arduino.cc/t/help-with-3-wire-load-cell/418197/2)
they recomended either instrumentation amp or just buy the hx711 circuit
https://www.ebay.com/itm/175038800753?_trkparms=amclksrc%3DITM%26aid%3D1110006%26algo%3DHOMESPLICE.SIM%26ao%3D1%26asc%3D20201210111314%26meid%3D60ccba6cca2145ec8cb8304d6cf5e6d8%26pid%3D101195%26rk%3D6%26rkt%3D12%26sd%3D163700015418%26itm%3D175038800753%26pmt%3D1%26noa%3D0%26pg%3D4429486%26algv%3DSimplAMLv11WebTrimmedV3MskuWithLambda85KnnRecallV1V2V4ItemNrtInQueryAndCassiniVisualRankerAndBertRecallWithVMEV3CPCAuto%26brand%3DUnbranded&_trksid=p4429486.c101195.m1851&amdata=cksum%3A17503880075360ccba6cca2145ec8cb8304d6cf5e6d8%7Cenc%3AAQAIAAABYObhgc4Nk8%252BdtAwOww4FKLaj%252FQ5qqgDlQCuqZA43WcPFUWDERCUugbbOk7XQv0JXlBfqCg2xKF3WcPghxGMFw2oSlXvfExEaMYr7I7LmrHcP6czY1wIMt0ORyKiCWt95xldincyyBx3g%252BNDW%252B%252FhWUgTaBhK6xAm%252BJIbCOMehu%252Bdw99K%252BVrcyuG2CVI%252B8GEM5yR340256FSLkc%252BFSxAdYGS%252BKown7hOnb8N%252B%252B6BI826UjcQOSRTVg7Iodk447hu%252BHkwWf7S7Gnr3gQIPeCgpNbnz6%252BgxaFRvdQGY%252FmOJrijjw5RNPq%252FaMeA0JOaukxt4Z0fZ78CT7B3V0zkmLqs%252BqRlGRH0%252FBcUKLw2IrhdLwWE3EAwlIknKrGtCHApmApfXkFvIep3SUFYufjR2ZbAC2h4Da5vs050chgShSVq2etCWvnBRL0e%252F%252BLrE1nf5x7S8LaqsNcKUyLB2W6EdThlXL8E4%253D%7Campid%3APL_CLK%7Cclp%3A4429486



