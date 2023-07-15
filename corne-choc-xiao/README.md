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



# Step 3: Parts.

Jon was kind enough to include a BOM, but there is some missing information that you can find on his git. But for completeness' sake, I am adding my CSV plus the table you see below.

The table below shows the parts that you will buy from JLCPCB
| Part | Count | Description | Link | Notes |
| ------------- | ------------- |------------- | ------------- | ------------- |
| PCB | 2 | When Gerber is uploaded to JLCPCB it will create 1 board and show the top and bottom. | [JLCPCB](https://cart.jlcpcb.com/quote) | A minimum of 5 will be ordered at once |
|  Case - Right  |  1  |  use whatever material you want. However, I went with  8111X Resin, White  |  [JLCPCB](https://cart.jlcpcb.com/quote)   |  only one is created at a time   |
|  Case - Left  |  1  |  use whatever material you want. However, I went with  8111X Resin, White  |  [JLCPCB](https://cart.jlcpcb.com/quote)   |  only one is created at a time   |
|  Battery Connector  |  2  |  C505023 - Pico EZmate  | [JLCPCB](https://cart.jlcpcb.com/quote)  | you can check [LCSC}(https://www.lcsc.com/product-detail/Switching-Diode_Shenzhen-Jinkaisheng-Elec-1N4148SOD-323_C2972761.html) with this part number, but ultimately you will add this part to your PCBA and have the factory install it for you.  |
|  Diodes  |    |  C2972761 - diodes  | [JLCPCB](https://cart.jlcpcb.com/quote)  | you can check [LCSC}(https://www.lcsc.com/product-detail/Switching-Diode_Shenzhen-Jinkaisheng-Elec-1N4148SOD-323_C2972761.html) with this part number, but ultimately you will add this part to your PCBA and have the factory install it for you.  |

For the other parts, you will have to source from other places. You can source them yourself. Check CSV for more information.

# Chapter 3: Ordering.

Ordering the PCB and Case where the hardest thing for me to understand. I was a little nervous at first, but after some research, I am pretty confident in what needs to be done. I don't know what is best, but I will update this if I find something better. 

### Order PCB + Diodes + Battery Connector

1) Alright, so first, let's hop on over to [JLCPCB](https://cart.jlcpcb.com/quote)
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/41f950fa-5e14-4b72-8d7f-43001f7bc285)

2) Click and open the Zip file. This file holds the Gerber file that the manufacturer needs to create the PCB.  
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/0c1a2e8c-52cb-4fba-8954-12816eb1ba09)

3) Here is the list of items I selected for my build. Feel free to pick whatever colour you want. Just note that the price will change with HASL Lead-Free for certain colours.
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/66bd125a-fdf0-4272-9673-b825222c4c38)

5) Click on the PCB Assembly and add these settings, and click confirm.
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/2aab36fc-1278-4f44-8f6c-f87c531e9098)

6) upload BOM and CPL Files. click confirm
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/ae5c99b0-dc83-41bf-a8fe-fea4b5aae710)
add BOM 
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/808ba121-1573-43d0-aa83-78b6466dfa88)
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/25e521ff-f653-437b-8aae-584e2d228d45)
add CPL
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/d9c30c97-732e-4510-85c6-31a1eb3bd4fa)
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/9b0f8885-91e3-4fc1-95ca-27cfc0392b43)
click process BOM and CPL
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/c15b9a56-1508-4902-b9ff-636e6ca73b0b)

7) Search for parts. In Jon's guide, he does have the part numbers, but they are in the issues section, so its not that easy to find.
first, we can add the power connector
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/dc88c641-60ee-4316-b6ae-5ba909735c8a)
next, we can add the diodes
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/c8daaca7-0fa6-4d91-a149-268ad0587170)
once added, we can hit next
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/3f7961f0-c3c1-426f-be32-b67d9f101b89)
we can inspect everything by looking at the 3d render and we can click next
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/18ff9d9a-1cc4-4c2e-a1e8-05401e577bfc)
inspect your build, add a description and hit add to cart.
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/2ec4a01d-75b0-45b3-aa35-23dfe2403841)

### Order Case
1) now we need to head back to [JLCPCB](https://cart.jlcpcb.com/quote) and click on 3D printing and add the Case Right and Left file.
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/392708b2-c185-4535-a20b-8cda15ef86c9)
add the Left stl file and then the right stl file. 
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/08a7aa2d-df76-404f-8739-54176de6fde4)
after adding both STL files you will see something like this. Note that I am adding 2 cases for both right and left, this is not needed. I want two just incase I mess something up.
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/cc200d0a-f707-4e8d-9c40-6523bb367d83)

### Buy PCB and Case
1) As a final check here is what I have. Now you should be able to checkout and get you PCB ordered!
![image](https://github.com/Paul-M-K/gerbers/assets/20325116/ea48899d-1091-4580-8b00-42eae382cd95)



























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

