stock tool kit mastering with fl studio

# introduction & basic setup
---

1) when you're done making a song and you want to start mastering it, first you should export it  as a **.wav** file. i like to use these settings:

	![[Pasted image 20241112193913.png]]
	
	* `32Bit WAV bit depth` and `512-point resampling sinc` are the key settings here for the highest sound quality. **the reason why you want to use a wav file is because it is an uncompressed format**, whereas **mp3 is compressed**. just compare the file sizes between the same song in mp3 and wav format and you'll see the difference.

next, drop the wav file into a new empty project to begin mastering.

2) now we've got our wav imported into an empty project, notice that the master track is totally empty for now:
   
	![[Pasted image 20241112193615.png]]

3) you can start off by normalizing the full song right off the bat, in many cases this small step will already make the song sound better:
 
	![[Pasted image 20241112193810.png]]

now that the basic set-up steps are done, we can start going into some details on mastering tools and practices, even just these simple steps will already make your songs sound way better, next we will look into some more tools to take our master to the next level.

# EQ (Equalization)
---
EQ is how you'll sculpt your song's sound frequencies using a series of virtual volume controls, each tied to a specific frequency range. imagine a set of seven volume knobs, but instead of controlling the overall volume of the track they each adjust the volume of a particular frequency range within the sound (measured in Hz and kHz). one knob might control sub bass tones, another would handle crispy high frequencies. EQ will allow you to emphasize or cut out certain parts of the mix, making a more polished and well balanced mix in the end. check out the handy Hz guide at the bottom of this section for a better sense of which frequencies correspond to different sounds. 

there are always exceptions or different ways of doing things, but here are two general EQ tips i've learned:

* **it's better to cut than to boost:** for example you've got a part of your song where the bass is taking up the whole mix and it's hard to hear the nice higher pitched synths you so carefully crafted. instead of boosting the high end melodic parts, try cutting the bass a bit by EQ'ing the low end instead.

* **it's best to make very small adjustments:** if you just start cutting out like 20 dB of your mix, its going to sound very unnatural and likely bad. stick to 1-2 dB adjustments at a time and hear how it plays.

---

**tools**:

1) **Fruity parametric EQ 2**
   *first tool best tool*

	![[Pasted image 20241112203458.png]]

* plop this right on the master track, and you can start with a built-in preset: **30Hz + 18kHz cut**, which will help clean-up a lot of junk in the song by cutting out anything below 30Hz and anything above 18kHz.
  
* why 30Hz for the low end? from what i've heard, most club systems cut off at about 35 Hz, most bass you will hear in even the most bass heavy music will cut off at around 41 Hz, its up to you to pick what ranges you want to keep in your mix or not, but 30 Hz feels like a safe range to me. in my own experience you can really feel and hear the difference on a nice sound system, which in my case is my car with its aftermarket sound system. i'll show you how to isolate specific frequencies below to test with.
  
* you can check the Hz in the top left corner as you're dragging stuff around in the EQ, this is called the "hint panel" in FL, and usually it tells you what any knob you're adjusting is doing:

	![[Pasted image 20241112204039.png]]  

* *how to: isolate your frequencies:*

	* **high end** - right click the right knob in EQ 2 and choose type > high pass:
	  
	  ![[FL64_fZbldvo2XR.gif]]
	
	* this will let you hear what exactly you're cutting out, just be sure to switch it back to low pass when you're done.  this is really neat, you can hear all the junk noise you're EQ'ing out and getting rid of.
	  
	* **low end** - you can do this same trick on the left knob, and switch it over to low pass:
	  
	  ![[FL64_hmT3S5SlOp.gif]]
	
	* as you drag the slider over, you will hear more and more audio start to pick up. this is the noise you're cutting out from the low end. again, be sure to switch this knob back to high pass when you're at a comfortable range to cut, probably between 20-40 Hz.

2) **Fruity Parametric EQ 2: Part Two**
   *a tool so nice, we had to use it twice*

* plop a second *Fruity Parametric EQ 2* onto the master track, we can call this the **"enhancement EQ"**, because you will use this one to focus on enhancing different parts of your song.
	* ![[Pasted image 20241112211637.png]]

  
* with this second EQ 2, you'll want to move the knobs around until your song sounds better, typically the mid range knobs (3-5) need a little boost from here. keep your master levels in mind and don't boost the dB so much that you start clipping the audio, try to keep the master level at 0.
  
	* ![[Pasted image 20241112212002.png]]
	
	* the hint panel is displaying 2.0 dB, and we can see that i've raised the yellow 4 knob to that amount.


* basically the idea here is, if you have to go above 2 dB to make something in your song sound good, its probably not going to sound good on different sound systems. so go back to your song's main flp and fix it in the mix and start this whole process over.

3) **Patcher**
 
* add patcher to the master track and then click the presets button:

  ![[Pasted image 20241112212734.png]]

* find the preset called "Mid Side EQ" -- not just the one that says "Mid Side", make sure it has those lucky two letters "EQ" in it:
  
  ![[Pasted image 20241112212851.png]]

* basically you want to click on the SIDE EQ in Patcher and move the 1 / Purple knob around until it sounds better. you can use the same tricks above to isolate the frequency and slide it around to hear what you're going to be cutting out with this SIDE EQ patch:
  ![[Pasted image 20241112213532.png]]

* you can right-click the little arrow coming out of the MID one to mute it while you tweak the side one, i circled it in red above. just be sure to unmute it when you're done.


---

here is that handy Hz guide i mentioned at the start of this section so many words ago
## A quick guide to the frequency spectrum

**50-75Hz** - Boost to beef up kick drums and sub bass lines. Cut to reduce excessive low-end weight.

**80-200Hz** - Boost to add body to snares and guitars, punch to kick drums, roundness to bass, and general warmth. Cut to reduce low-end mud.
 
**200-500Hz** - Boost to ‘warm up’ vocals, guitars and synths, and add presence to basses. Cut to reduce muddiness.

**500-800Hz** - Boost (with care!) to bring out the tone of almost any instrument. Cut to reduce ‘honk’.
 
**2-5kHz** - Boost to give vocals, guitars, synths and strings clarity, definition and impact. Cut to reduce harshness.
 
**5-10kHz** - Boost to add presence and sheen to drums, cymbals and guitars. Cut to reduce scratchiness and sibilance.
 
**16kHz+** - Boost for brightness and ‘air’. Cut to reduce high-end fizz.

---
##### human hearing range in Hz/kHz:

![[Pasted image 20241112205923.png]]

