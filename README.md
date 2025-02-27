# Build Notes for the Fysetc Doron Velta kit

I had been talking with my friend Jason about the Doron Velta, as we are both interested in Delta printers.  I explained to him that I wasn't interested in building one because I already had a FLSun V400 that has a much bigger build area.  The experience with my V400 hasn't been the best.  When it works, it's great, but it goes from working great to completely broken without any notice.

I decided to build a Doron Velta from the [Fysetc kit](https://www.fysetc.com/products/3d-printer-doron-velta?_pos=1&_sid=952f69bd9&_ss=r), simply because they had a coupon code that brought the price down to around $380 USD shipped.  For that price I figured it could be something fun to build, if I needed it or not.

For printed parts I used the [Fabreeko Github](https://github.com/Fabreeko/Doron-Velta/tree/main) as they have the files named for if they are primary or accent colors, gives the option of using 2 accent colors.

As I didn't find a build guide similar to the ones for Vorons, I am primarily using this [video](https://www.youtube.com/watch?v=-V6F0aNnRW4).  

## What was purchased?

As mentioned above, the actual kit, obviously.  However for various reasons that will be covered throughout this document, I did purchase some additional stuff.  A complete list is [Here](extras.md) of all the things I purchased or used in addition to the Fysetc kit to complete my build.

Before I even started the build, I read on Discord of some people having issues with the MCU that is included in the Fysetc kit, so I purchased the [BTT SKR Pico](https://www.amazon.com/dp/B09MYKL9MP?ref_=ppx_hzsearch_conn_dt_b_fed_asin_title_1&th=1) that is called for in the original [BOM](https://github.com/rogerlz/Doron-Velta/blob/main/BOM.md) from Rogerio Goncalves the designer of the Doron Velta.

The Fysetc kit does not come with a Raspberry Pi, so you will need one of those.  I ended up going with a [2GB Raspberry Pi 5](https://www.pishop.us/product/raspberry-pi-5-2gb/), and since I have heard that the RPI5 does get hotter than the RPI4 did, I went ahead and got the [active cooler](https://www.pishop.us/product/raspberry-pi-active-cooler/).

While I have not yet found the modified printed parts (or created my own), I do want to add a touch screen like on my Vorons, so I ordered a [BTT TFT4.3](https://www.amazon.com/dp/B09791ZG1B?ref_=ppx_hzsearch_conn_dt_b_fed_asin_title_1&th=1).  Hopefully I will figure out a good way to mount that before I finish my build.

For the filament for the printed parts, I choose [Ambrosia Matte ABS](https://west3d.com/products/ambrosia-abs-matte-filament-of-the-gods-1kg-bambu-ams-friendly-cardboard-spools-premium-3d-printing-filament) in Black and British Racing Green.  I used about 2kg of each color, mainly due to some issues with the printer I was printing them on having a few issues and having to restart many prints.

## The build

As I started installing the heat set inserts, I noticed the Effector is different in the parts I printed than the one used in this video.  The video uses heat sets for where the rods attach, whereas the one I printed uses captured nuts.  It appears that the captured nuts would be square nuts, but I did not find any in the kit.  When I get to that part of the build, I will verify if it in fact needs square nuts, and if the nuts are provided or not.

The video only shows placing heat set inserts in two of the skirts, however all skirts had places for heat set inserts.  There were not enough 3mm heat set inserts to put them in all of the skirts.  The Effector and the printed part for Klicky use 2mm heat set inserts and there appears to be more than enough of those.

Speaking of the heat set inserts, I didn't notice a heat set insert tool in the kit.  The [printed part](https://github.com/FYSETC/FYSETC-Doron_Velta/blob/main/STLs/Extrude%20the%20head/printed_part.STL) for Klicky wasn't in the Fabreeko STLs, but was in the [Fysetc github](https://github.com/FYSETC/FYSETC-Doron_Velta/tree/main), so I printed that as well.

At approximately 20 minutes into the video, they show placing the pulleys on the stepper motors.  I highly recommend using some blue Loctite on the set screws to prevent them from working loose.  This is mentioned in build guides for Voron printers, and also mentions they are the source of a lot of problems, so go ahead and use some Loctite, and you shouldn't have to worry about motor pulleys coming loose.  Also ensure that one of the two set screws per pulley is located on the flat spot of the motor shaft.

During installation of the motors, you could easily allow the limit switch wiring to go between the top panel and the motor.  If you do this, there is a risk it will interfere with the belt once installed.  There appears to be just enough clearance to run the wire between the motor mount and the corner printed part.

![Motor](images/motor.png)

So as you get more to the wiring, there appears to be a lot left out of the video I followed.  The kit does include a thermal fuse for the bed, but that is never shown in the video.  Simply bolt the fuse to one of the open threaded holes on the bottom of the bed, and connect the wired.

![Thermal Fuse](images/thermal_fuse.png)

The one thing I noticed that is missing from this kit, is there is no ground wire to the heat bed.  This is recommended when using an AC powered bed heater.
