# **I strongly recommend you to read this before getting started**

# Acrylic_3D_KB
This is a 44 key 3D keyboard made by laser cut acrylic, designed by @kobakos32(twitter), u/kobakos32(reddit)

I assume that most people who read this has basic knowledge on building keyboards,like key matrix and firmwares,so i will just write about something specific on this keyboard.
This keyboard is really tall, so an wrist rest is recommended to type properly.(You can make this shorter by cutting off the 2nd pinky column and the bottom thumb key).

In this guide, I will call the red colored part 'plate section', and the gray part 'bottom section'.
![case structure](/readme_images/irowake.png)

# What you'll need
- keyswitches:44
- diodes:44
- random wire(I used junk LAN cable):appropriate amount
- pro micro:2
- plate mount trs jack which is capable of 3mm thick plate:2
- solvents to stick the acrylics:appropriate amount
- brush or syringe

# About the laser cut path data
This data was made to fit into an A4 size sheet(297mm* 210mm). please follow the format of where you order your acrylics to.
If you want this to be in a different format or modify this, you can do that easily using graphic softwares such as inkscape.
Please use an 3mm thick sheet for this keyboard.

# Rough procedure

## Temporaly assembling the case
The first step is toy temporary assemble the case before glueing the acrylics together. You have to do this because even a minor error can add up to a major error, which will make the plate section unable to fit the bottom section. 
First assemble the bottom section, using these images as a reference. The rectangler shaped acrylic with slits(which is omitted in the image) is for mounting the pro micro so it is not necessary for you to assemble it here.
(If you want to take a closer look at these images,please look at the original images in the images folder in this repository.)
Don't place the switches at this point.
![case structure](/readme_images/bottom_bunnkai.png)
![case structure](/readme_images/bottom_bunnkai_2.png)
Then, assemble the plate section, using these images as a reference and insert it to the bottom section.
![case structure](/readme_images/top_bunnkai_maue.png)
![case structure](/readme_images/top_bunnkai_naname.png)
![case structure](/readme_images/top_bunnkai_sita.png)
The plate part and the bottom part will intersect like this.
![case structure](/readme_images/top_bottom_intersect.png)
![case structure](/readme_images/top_bottom_intersect-2.png)
![case structure](/readme_images/top_bottom_interset_3.png)

## Glueing the plate section
After temporary assmebling the case, glue only the plate section, since you wil have to solder the switches, and it will be hard to insert the plate section to the bottom section with the switches on, when you also glue the bottom section(Because of my bad design...). Put solvent such as dichloromethane in a syringe or brush, and pour the solvent onto the acrylic bonding surface. Apply pressure(not too strong) to the bonding surface, and wait for tens of seconds to glue the acrylics. This is pretty hard to do it so also check some tutorials on how to bond acrylics with solvents. You'll need to wait for a day for the acrylics to stick completely, but you can move on to the next step.
Dicloromethane is not an safe material, so be careful when handling it.
When handling dichloromethane, use the following safety precautions:
- Wear protective clothing. Footwear should cover the entire foot.
- Always wear PPE such as chemical splash goggles and safety gloves.
- Work in a well-ventilated area (preferably in an environment with a fume extraction system).
source:[MSDSonline](https://www.msdsonline.com/2015/02/20/dichloromethane-methylene-chloride-hazards-safety-information/)
I recommend you to at least put on gloves and ventilate the working area.

## Wiring and setting up firmwares
Wiring are the same as other keyboards. Please refer to [hand wiring guide](https://beta.docs.qmk.fm/using-qmk/guides/keyboard-building/hand_wire) and [split keyboard guide](https://beta.docs.qmk.fm/using-qmk/hardware-features/feature_split_keyboard) from qmk.
Don't wire any rows or cols to the D0 port(PD0) if you are going to use the default settings of QMK's split keyboard.
The original version mounted the pro micro with a pcb called [ProMicroSocket](https://booth.pm/ja/items/1073313) and standoffs, but since it is hard to get it in countries other than Japan, this version uses a small piece of acrylic to mount the pro micro, as mentioned before. The pro micro will be glued to the acrylic part like the below image.
![promicro mount](/readme_images/promicro_mount.png)
![promicro mount](/readme_images/promicro_mount_2.png)
The trs jack will be mounted here.
![place of trs jack](/readme_images/trs_jack_place.png)

## Operation verification
Check if the keyboard works properly since you won't be able to access some of the part of this keyboard once you adhere the whole case.
Check if...
- each key is responsive.
- there is any soldering defect.
- the communication between the left side and the right side is working properly.

## Glueing the whole case
If it seems like there are no errors, insert the plate section to the bottom section and adhere the whole case, including pro micro and you're done!
