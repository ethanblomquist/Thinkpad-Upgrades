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
There are 4 screws holding down the CPU cooler. Remove these 4 screws and unplug the fan. 
</p>
<img src=https://i.imgur.com/ImVEfpC.jpg/>
<p>
Clean all the old thermal paste with isopropyl alcohol. Reapply a very small amount of thermal paste to the CPU. Make sure when tightening the 4 CPU screws that you tighten evenely, preferably in a criss-cross pattern, this ensures the cooler exerts pressure evenly. Plug The fan able back into the motherboard
</p>
<img src=https://i.imgur.com/asUhN3j.jpg/>

<h3>Step 7: Reinstall Bottom Cover</h3>
<p>
Click the cover back on and tighten scrws until snug. Install the new external battery by simply sliding it into the slot
</p>
<img src=https://i.imgur.com/0PnXOOm.jpg/>

<h3>Step 8: Boot to BIOS</h3>
<p>
Before installing an operating system, we should check if the PC will boot to the BIOS and there are no catastrophic hardware failures.
</p>
<img src=https://i.imgur.com/cN6hJKJ.jpeg/>
<p>
Let's run some diagnostics to make sure the hardware we purchased and the old hardware is running without issues. Press the power button, when the Lenovo screen pops up press enter -> F10 to Diagnose Hardware 
</p>
<img src=https://i.imgur.com/WI4xBZz.jpg/>
<p>
-> Run All
</p>
<img src=https://i.imgur.com/lxqj4W2.jpg/>
<p>
-> Deselect Extended
</p>
<img src=https://i.imgur.com/V4GWpHL.jpg/>
<p>
-> All tests passed
</p>
<img src=https://i.imgur.com/ZUBv94G.jpg/>

<h3>Step 9: Create a Linux Bootable USB</h3>
<p>
  
To prepare for the OS installation, we will need two USB drives. On a seperate PC, download [Ubuntu Linux](https://ubuntu.com/download/desktop) -> Download [balenaEtcher](https://etcher.balena.io/#download-etcher) -> Open balenaEtcher -> Flash from file -> Select the Ubuntu iso file -> Select desired USB drive -> Eject drive when finished
</p>
<img src=https://i.imgur.com/KOB5zwH.png/>

<h3>Step 11: Install Window</h3>
<p>
  
Insert the USB drive into a different PC and download the [Windows Media Creation Tool.](https://www.microsoft.com/en-us/software-download/windows10)
<p>
<img src=https://i.imgur.com/U3R7AWu.png/>
</p>
<p>
Run the program -> Accept -> Create installation media -> Next -> 64-bit Windows 10 -> USB Flash Drive -> Select the drive for the removable storage (D:) -> Next -> The program may take a significant amount of time to run. -> When the tool finishes, eject the drive -> Insert the USB drive into the T480 and power on -> The computer shoula automatically boot to the Windows 10 installer -> Install now -> Enter product key or select "I don't have a product key" if yout T480 came with a Windows liscence -> Select which edition of Windows you want to install -> Custom -> Select our drive -> New -> We can now designate how much of our hard drive we want to alloacate to windows. I have a 1TB SSD, I'm going to split it up in half between Linux and Windows, allocating 450,000MB to Windows. -> This leaves us with 492.1GB for our Linux OS -> Select a region and a wireless network
</p>



<h3>Step 9: Check for BIOS</h3>
<p>
The T480 had an issue in earlier BIOS versions in which the USB-C charging connection would sometimes burn out. Since this connection is soldered to the motherboard, if it did break the entire motherboard would have to be replaced. Looks like evrything is good so far.
</p>
<img src=https://i.imgur.com/MiH00Rg.jpeg/>
<p>
<h3>Step 11: Install Linux</h3>
<p>

</p>
<img src=/>

<h3>Step 12: </h3>
<p>

</p>
<img src=/>

<h3>Step 13: </h3>
<p>

</p>
<img src=/>
