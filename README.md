<h1>Rebuilding and Upgrading a Thinkpad T480 Laptop</h1>
<p>
I started this project because I needed an affordable laptop for study, work, and projects. The Thinkpad series of laptops has a stellar reputation for durability, serviceability and performance. Let's rebuild a laptop together from the ground up!
</p>
<img src=https://i.imgur.com/WD57YW3.jpg/>

<h2>Goals for this Project</h2>
<p>
Ultimately I want a solid laptop with good battery life, enough performace for smooth web browsing and office productivity(Word, Excel etc.) I also need the machine to perform IT related tasks such as local virtualization, scripting/programming and other basic Windows/Linux functions such as BASH, Powershell, RDP etc.
</p>
<h3>Additionally we will need to:</h3>

  - Install missing hardware into used laptop
  - Dual boot Ubuntu Linux and Windows 10 on the same hard drive
  - Keep costs to a minimum

<h2>Barebones T480 Specs</h2>
<p>
As you can see below there isn't much included in this used T480 I found on ebay. However, the price was relatively low and it gives us a chance to rebuild the system to our own specifications.
</p>

  - Display: 14" - Unknown resolution
  - No Charger
  - HDD: None
  - RAM: None
  - No operating system
  - CPU: Intel i5-8250u
  - No External Battery(The T480 has both an internal 24wh battery and an external hot swappable battery)
  - Total Cost: $126

<img src=https://i.imgur.com/TSbkNdI.png/>

<h2>Components Purchased for the Upgrade </h2>

  - 24wh Internal Battery Relacement
  - 72wh Swappable External Battery Replacement
  - 16GB(2x8gb) DDR4 2400MHz RAM
  - 1TB NVME M.2 SSD
  - 65W USB-C Charger
  - Thermal Paste
  - iFixit Electronics Toolkit
  - Total Cost: $197.79

<img src=https://i.imgur.com/iBZW1kK.jpg/>

<h3>Step 1:Cleaning the Laptop</h3>
<p>
This laptop came to me pretty dirty, first thing I'd like to do is clean it up.
</p>
<img src=https://i.imgur.com/ONIocXC.jpg/>
<p>
I removed the stickers and cleaned all the surfaces thoroughly.
</p>
<img src=https://i.imgur.com/ENZsQRT.jpg/>

<h3>Step 2: Remove the Back Cover</h3>
<p>
Next we need to loosen each of the 6 screws holding the back cover on.
</p>
<img src=https://i.imgur.com/juzStXS.jpg/>
<p>
Then pry the back cover off.
</p>
<img src=https://i.imgur.com/3rrZBP7.jpg/>

<h3>Step 3: Install the RAM</h3>
<p>
When installing SODIMM, be sure to line up the indentation, push in slightly, then push down until the RAM locks into place.
</p>
<img src=https://i.imgur.com/r2Kf06h.jpg/>

<h3>Step 4: Remove and Install the Internal Battery</h3>
<p>
There are two small screws holding the internal battery into place. After removing them, unplug the small connector near the CPU fan. The installation is the reverse process. I used a pair of forceps to push in the connector.
</p>
<img src=https://i.imgur.com/FBcAGdp.jpg/>

<h3>Step 5: Install the M.2 NVME SSD</h3>
<p>
Remove the SSD enclosure by pulling up, it will pop out. Remove the two screws holding the metal piece covering the SSD slot, then remove the screw used for securing the SSD. 
</p>
<img src=https://i.imgur.com/h1LsNn8.jpg/>
<p>
Installing the SSD is similar to the RAM, push in slightly, then use the provided screw to very gently tighten the SSD to the enclosure, be cautious not to overtighten. Reinstall enclosure.
</p>
<img src=https://i.imgur.com/a3vaWvO.jpg/>



<h3>Step 6: Remove and Install the CPU Fan</h3>
<p>
There are 4 screws holding down the CPU cooler. Remove these 4 screws and unplug the fan. Clean all the old thermal paste with isopropyl alcohol. Reapply a very small amount of thermal paste to the CPU. Make sure when tightening the 4 CPU screws that you tighten evenely, preferably in a criss-cross pattern, this ensures the cooler exerts pressure evenly. Plug The fan able back into the motherboard
</p>
<img src=/>

<h3>Step 7: Reinstall Bottom Cover</h3>
<p>
Click the cover back on and tighten scrws until snug. Install the new external battery by simply sliding it into the slot
</p>
<img src=/>

<h3>Step 8: Check the Laptop will Boot to BIOS</h3>
<p>
Before installing an operating system, we should check if the PC will boot to the BIOS and there are no catastrophic hardware failures. On start up I've recieved a message the third party party I purchased is not compatible. To check which battery is the problem, I removed the larger external battery and tried starting the computer again. There was no error messages, so the external battery seems to be the problem. I'll have to remove the new external battery and return it for now. Although the internal battery is small, I will be able to use the laptop, just with a reduced battery life.
</p>
<img src=/>

<h3>Step 9: Run Hardware Diagnostics in the BIOS</h3>
<p>
Press the power button, when the Lenovo screen pops up press enter -> F10 to Diagnose Hardware -> Run All -> Deselect Extended -> All my tests passed
</p>
<img src=/>

<h3>Step 10: Install Windows 10</h3>
<p>
Let's try installing Windows 10. Insert the SD card into the T480's reader slot. The PC should reach a 
</p>
<img src=/>


<h3>Step 1: Windows 10 Installation</h3>
<p>
We need a portable storage device to install our operating systems. I had a 32gb SD card laying around, so I decided to use that. We will start with Windows 10. On my other laptop that has an SD card reader, I downloaded the Windows Media Creation Tool. Run the program -> Accept -> Create installation media -> Next -> 64-bit Windows 10 -> USB Flash Drive -> Select the drive for the removable storage (D:) -> Next -> The program may take a significant amount of time to run
</p>
<img src=/>
