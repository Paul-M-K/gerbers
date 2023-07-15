# Preface

First off, thanks to Jon for doing all the work. 

None of this is my work; I have not changed any files, so 100% none is mine.

My goal for this fork is to help other noobies build their first keyboard. I have done enough research, and I want to pass on this knowledge to others if they stumble upon this guide.

# Step 1: Keyboard layout (optional read - good idea to read to learn about the keyboard).

Write stuff about the keyboard, maybe some history. Write about how this keyboard is for Choc switches; it is for hot swap only, and there is no spot for soldering. There is no top case either, so we will see.

Put some interesting links to add graphics or to reconfigure the board. 

# Step 2: Prerequisites
The first thing we will want to do is download the zip file from [JonMuller's Git](https://github.com/JonMuller/gerbers)

![image](https://github.com/Paul-M-K/gerbers/assets/20325116/afdcc6b4-2070-45e3-9d73-f1217421a74b)

We can then extract these files. Feel free to browse them and try to familiarize yourself with them.



# Chatper 2: Parts.

Jon was kind enough to include a BOM, but there are some missing information that you can find on his git. But for completeness' sake, I am adding my CSV plus the table you see below.

The table below shows the parts that you will buy from JLCPCB
| Part | Count | Description | Link | Notes |
| ------------- | ------------- |------------- | ------------- | ------------- |
| PCB | 1 | When Gerber is uploaded to JLCPCB it will create the left and right board | [JLCPCB](https://cart.jlcpcb.com/quote) | A minimum of 5 will be ordered at once |
|  Case - Right  |  1  |  use whatever material you want. However, I went with  8111X Resin, White  |  [JLCPCB](https://cart.jlcpcb.com/quote)   |  only one is created at a time   |
|  Case - Left  |  1  |  use whatever material you want. However, I went with  8111X Resin, White  |  [JLCPCB](https://cart.jlcpcb.com/quote)   |  only one is created at a time   |
|  Battery Connector  |  2  |  C505023 - Pico EZmate  | [JLCPCB](https://cart.jlcpcb.com/quote)  | you can check [LCSC}(https://www.lcsc.com/product-detail/Switching-Diode_Shenzhen-Jinkaisheng-Elec-1N4148SOD-323_C2972761.html) with this part number, but ultimately you will add this part to your PCBA and have the factory install it for you.  |
|  Diodes  |    |  C2972761 - diodes  | [JLCPCB](https://cart.jlcpcb.com/quote)  | you can check [LCSC}(https://www.lcsc.com/product-detail/Switching-Diode_Shenzhen-Jinkaisheng-Elec-1N4148SOD-323_C2972761.html) with this part number, but ultimately you will add this part to your PCBA and have the factory install it for you.  |

For the other parts, you will have to source from other places. You can source them yourself. Check CSV for more information.

# Chapter 3: Ordering.

Now that we are familiar with the parts of the keyboard, it is safe to start ordering them.








More pics to look at for guidance on building: https://imgur.com/a/QKp5wG5

Power switches: https://www.amazon.com/gp/product/B0826XVZ8M/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1

XIAO BLE: https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html

Batteries: https://www.amazon.com/HAC-006-BPJMX-C0-Battery-Nintendo-HAC-015-Controller/dp/B08L3FWXS4/ref=sr_1_4?crid=2YZOVGUSZ9RTX&keywords=HAC-006&qid=1679153921&s=electronics&sprefix=hac-006%2Celectronics%2C110&sr=1-4

Nice!View: https://typeractive.xyz/products/nice-view

Mill-Max pins (used on Nice!View): https://www.digikey.com/en/products/detail/mill-max-manufacturing-corp/3320-0-00-15-00-00-03-0/4147392?s=N4IgTCBcDaIKIBECMSDMAWAtAOQSAugL5A

Low profile sockets (used with Nice!View): https://www.digikey.com/en/products/detail/aries-electronics/40-0518-10/261892

03/12/23 added in ZMK starter files. These should go in the boards/sheilds directory of your ZMK branch. Then go in and modify the build.yml to include it.

If you get stuck on anything, the ZMK discord is very helpful. 

https://zmk.dev/

