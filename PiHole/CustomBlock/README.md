# Custom block page

The original Pi-Hole code has been modified, first modified 26/06/2018. [License](https://github.com/pi-hole/pi-hole/blob/master/LICENSE).

Info/steps on my custom Pi-Hole block page. It's not finished yet I don't think, but I hope this works as a helpful guide for others.   
Thanks to Pi-Hole (Original code [here](https://github.com/pi-hole/pi-hole), site [here](https://pi-hole.net/)) for being awesome and WaLLy3K for providing [the idea and direction](https://github.com/WaLLy3K/Pi-hole-Block-Page).

![](blockpageExample.jpg)   
Custom dark theme of Pi-Hole's blockpage for your sleepy eyes.

---

# 1. Back-up  
Copy the pihole directory to wherever you want to back-it-up to. E.g: from root, **cp -r /var/www/html/pihole/ home/pi/**  
Don't blame me if your Pi-Hole blows up.

# 2. Shuffle around files  
Rename the original block page in /var/www/html/pihole/. Doesn't matter what to, I just used ORIG_blockingpage.css.

Move the background you want into /var/www/html/admin/img/. The one I used is up there, bg.png.


# 3. Custom blockpage  
Move blockingpage.css into /var/www/html/pihole/.

Run **sudo service lighttpd force-reload** and you're done! 

---

In the CSS file, search for the following if you want to modify specific parts and are a noob at CSS like me.

**Flag1** - Change the background picture.   
**Flag2** - The header bar colour and rounded corners. Go 2 code blocks down for header font.   
**Flag3** - The "Why am I here?" box of the header that brings up the pop-up box.   
**Flag4** - Inside of the above pop-up box.   
**Flag5** - The actual blockpage background colour, font, whatever.   
**Flag6** - Button details.   
**Flag7** - Footer details.   
