i have been mastering all my songs out of fl studio for years by just doing it all in one .flp file, by directly applying all my EQ and compression and filters and stuff right on the master channel in the same .flp file i made the song in. recently, i decided to look up some tutorials on mastering so i can try and make my songs sound a little bit better, more clean, and more professional. this is a guide showing what i learned so hopefully it can help somebody out there, why not! 

if you prefer to watch a video, i stole all this from this youtube video 😈  https://www.youtube.com/watch?v=OrCxnr0W5yY

i personally started caring about this more once i got a really nice subwoofer system in my car (humble brag) and i noticed all my songs sounded like pure unfettered ass, whereas professional songs sounded really good and clean no matter how loud i played them (usually). hence, i needed to learn about mastering. i could also buy some studio monitors like the KRK Rokit's which are highly recommended by most production nerds i know, but for now i like testing my mixes out in my car with my really nice subwoofer. the workflow isn't as smooth or hassle-free; but the feel of the wheel, the cool night breeze against my hair, white knuckling my way under the stars... bliss! 
# introduction & basic setup
---
first of all, stop mastering your songs in the same .flp file you made the song in **! !** do all your usual stuff that you would do while making a song, apply whatever effects or filters you want to your separate channels, etc., do all your automation, yada yada you get it. go make a song. all of those steps are part of your general song making and *mixing* portion of the process. **mastering** is what you'll want to do at the very end to finalize the song and prepare it for upload. 

if you want to improve your sound quality and you're currently just blindly exporting out .mp3 files without a care in the world, then just using the steps from this introduction will help a lot, and these steps are super easy.


1) so when you're done making a cool song and you want to start mastering it, first thing is export it out as a **.wav** file. i like to use these settings:

	![[Pasted image 20241112193913.png]]
	
	*you can change what you want to do with the Tail, but `32Bit WAV bit depth` and `512-point resampling sinc` are the key settings here for maximum sound quality. **the reason why you want to use a .wav file is because it is an uncompressed format**, whereas **.mp3 is compressed**. this is by design and you can check for yourself at any time by exporting the same exact song as a .wav file and an .mp3 file, you will immediately notice the file size difference between the two. mp3 was made with smaller file size in mind, back in '91 when even a 10 Mbps connection was considered godly, nowadays people sling around 100's of GBs of data daily without even noticing. nothing wrong with .mp3, its a great format, just that its a totally different tool than what we're after -- **which is maximum sound quality**, hence, **we need uncompressed data!** did i mention i also work in IT;;;

now what you want to do is start a new empty project .flp file and import that .wav file to it, then you will start doing your mastering from here. this has another benefit, you can clean-up any weird popping or clicking noises that often occur at the beginning or end of a track here before you notice them later. this always happens to me and its super annoying so i had to mention it here.

2) now we've got our .wav imported into an empty project, notice that the master track is totally empty for now:
   
	![[Pasted image 20241112193615.png]]

3) you can start off by normalizing the full song right off the bat, in many cases this small step will already make the song sound better:
 
	![[Pasted image 20241112193810.png]]

now that the basic set-up steps are done, we can start going into some details on mastering tools and practices. like i said previously, if you were just mastering all in one file and exporting out an .mp3, even just these simple steps of exporting it to .wav and normalizing it in a new empty project will already make your songs sound way better, which is pretty neat huh?

# EQ (Equalization)
---
you can think of EQ as "sculpting frequencies" with a collection of volume knobs, represented by the frequency bands they control. this probably sounds confusing, but basically you know what a volume knob is and what it does, so just imagine there are like 7 of them, and each of these 7 volume knobs controls a specific frequency range in your song (when you're thinking of frequencies, think of Hertz and Kilohertz -- i'll post a handy Hz guide at the bottom of this section).

there are always exceptions or different ways of doing things, but here are two general EQ tips i've learned:

* **it's better to cut than to boost:** for example you've got a part of your song where the bass is taking up the whole mix and it's hard to hear the nice higher pitched synths you so carefully crafted. instead of boosting the high end melodic parts, try cutting the bass a bit by EQ'ing the low end instead.
  
* **it's best to make very small adjustments:** if you just start cutting out like 20 dB of your mix, its going to sound very unnatural and likely bad.

1) **Fruity parametric EQ 2**
   *first tool best tool*

	![[Pasted image 20241112203458.png]]

* plop this bad boy right on the master track, and you can start with a built-in preset: **30Hz + 18kHz cut**, which will right off the bat help clean-up a lot of junk in the song. 
  
* why 30Hz for the low end (the left most knob)? well, most high end club systems cut off at about 35 Hz, most bass you will ever hear in even the nastiest dubstep basslines (sick bro) will cut off at around 41 Hz, so really by cutting the low end band at 30 Hz you're just preventing unnecessary muddy bass from ruining your sick new beat. you can adjust to your liking and your mix as needed, this is a "safe" range to play around in. i'll show you how to isolate specific frequencies below to test with.
  
* you can also play around with this by just listening to your song and sliding the little knobs around in EQ 2 and you'll get a good idea of what it's doing to your song. remember, its best to make very small adjustments! if you cut the low end at 25 Hz, or 35 Hz, its probably not a big deal. it might sound different from song to song too based on your mixing. just pay attention to the Hz in the top left corner as you're dragging stuff around in the EQ:

	![[Pasted image 20241112204039.png]]  

* ==*some more neat tricks -- isolate your frequencies:*==

	* **high end** - right click the right knob in EQ 2 and choose type > high pass:
	  
	  ![[Pasted image 20241112204803.png]]
	
	* this will let you hear what exactly you're cutting out, just be sure to switch it back to low pass when you're done. but this is really neat because its probably going to sound extremely tinny and terrible, so this is all the junk noise you're EQ'ing out and getting rid of!
	  
	* **low end** - you can do this same trick on the left knob, and switch it over to low pass:
	  ![[Pasted image 20241112205038.png]]![[Pasted image 20241112205106.png]]
	
	* as you drag the slider over, you will hear more and more audio start to pick up. this is the noise you're cutting out. obviously in my example above dragging it all the way over to 648 Hz is really bad, this is just a screenshot to show you the idea of dragging the sliders around to hear what you're going to be removing. again, be sure to switch this knob back to high pass when you're at a comfortable range to cut, probably between 20-40 Hz.

2) **Fruity Parametric EQ 2: Part Two**
   *a tool so nice, we had to use it twice*

* plop a second *Fruity Parametric EQ 2* onto the master track and pretend you're that guy who told George W. Bush that a second *Fruity Parametric EQ 2* has just hit the *Master Track* on *Septe-* okay you get where I'm going with this. this second EQ 2 will be what we in the biz (the 705k people who also watched the same youtube video as me) like to refer to as your **"enhancement EQ"**
	* ![[Pasted image 20241112211637.png]]

* **Bam!** *Anotha one!* how do i hold all these *Fruity Parametric EQ 2's*. the list of jokes, my friends, it does not stop here. except it does actually let's move on.
  
* with this second EQ 2, you'll want to mess around with the 4 knob mostly, and just kind of slide it around until it sounds so good, so nice. maybe move it up a little bit, who knows. something actually important here though, just make sure you aren't boosting anything in here above 2 dB in sound. maybe 3 dB if you're feeling dangerous. maybe meatball. no, no meatball, etc.
  
	* ![[Pasted image 20241112212002.png]]
	* *this little slider, with the red arrow pointing to it in our enhancement EQ, this is the dB slider. 
	  
	  *you can always check what something is doing in FL by looking in the top left corner, where i've strategically placed a second red arrow, called the "hint panel", to track the changes whatever knob you're sliding around is doing.*

* basically the idea here is, if you have to go above 2 dB to make something in your song sound good, its going to actually sound terrible once you get it into that cool car with the nice subwoofer we were talking about earlier. so go back and fix it in the mix and start this whole process over. good job. you ruined it.

3) **Patcher**

* ok this part is actually pure wizardry i would never have figured this out on my own, the EQ stuff and all that other bullshit from before meant nothing to me. this is actually nuts. check this out you're gonna love this.
  
* okay so add patcher and then click the presets button, which is literally the button that says presets on it (took me a second to find, you're welcome)
  ![[Pasted image 20241112212734.png]]

* find the preset called "Mid Side EQ" -- not just the one that says Mid Side ok, make sure it has those lucky two letters "EQ" in it:
  ![[Pasted image 20241112212851.png]]

* this part might honestly be easier to follow along in the video, around 969s / 5:37 mark. basically you want to click on the SIDE EQ in Patcher and move the 1 / Purple knob around until it sounds better. you can use the same tricks above to isolate the frequency and slide it around to hear what you're going to be cutting out with this SIDE EQ patch:
  ![[Pasted image 20241112213532.png]]
* you can right-click the little arrow coming out of the MID one to mute it while you tweak the side one, i circled it in red above 

* i actually couldn't get it to work at all in my example song but maybe its just because the song i picked is mixed really lightly, i just threw some old 50's rock song in my mix for examples, so there's not like a lot of dynamic range compression or any modern digital stuff going on. or maybe i'm just a big freakin idiot. anyway the patcher thing looks really cool to me so i mention.

---
here is that handy Hz guide i mentioned at the start of this section so many words ago -- source https://audient.com/tutorial/the-beginners-guide-to-eq/
## A quick guide to the frequency spectrum

Although any EQ processing will inevitably be highly dependent on the nature of the source material, there are some general rules to follow when it comes to cutting and boosting certain ‘standard’ frequency ranges.

**50-75Hz** - Boost to beef up kick drums and sub bass lines. Cut to reduce excessive low-end weight.

**80-200Hz** - Boost to add body to snares and guitars, punch to kick drums, roundness to bass, and general warmth. Cut to reduce low-end mud.
 
**200-500Hz** - Boost to ‘warm up’ vocals, guitars and synths, and add presence to basses. Cut to reduce muddiness.

**500-800Hz** - Boost (with care!) to bring out the tone of almost any instrument. Cut to reduce ‘honk’.
 
**2-5kHz** - Boost to give vocals, guitars, synths and strings clarity, definition and impact. Cut to reduce harshness.
 
**5-10kHz** - Boost to add presence and sheen to drums, cymbals and guitars. Cut to reduce scratchiness and sibilance.
 
**16kHz+** - Boost for brightness and ‘air’. Cut to reduce high-end fizz.

---
##### here is also a guide to human hearing range in Hz/kHz:

![[Pasted image 20241112205923.png]]

