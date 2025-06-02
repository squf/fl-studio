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

	![[Pasted image 20241112203458.png]]

* plop this right on the master track, and you can start with a built-in preset: **30Hz + 18kHz cut**, which will help clean-up a lot of junk in the song by cutting out anything below 30Hz and anything above 18kHz.
  
* why 30Hz for the low end? from what i've heard, most club systems cut off at about 35 Hz, most bass you will hear in even the most bass heavy music will cut off at around 41 Hz, its up to you to pick what ranges you want to keep in your mix or not, but 30 Hz feels like a safe range to me. in my own experience you can really feel and hear the difference on a nice sound system, which in my case is my car with its aftermarket sound system. i'll show you how to isolate specific frequencies below to test with.

* you can check the Hz in the top left corner as you're dragging stuff around in the EQ, this is called the "hint panel" in FL, and usually it tells you what any knob you're adjusting is doing:

	![[Pasted image 20241112204039.png]]  

* *how to isolate your frequencies:*
 
	* **high end** - right click the right knob in EQ 2 and choose type > high pass:
	  
	  ![FL64_fZbldvo2XR](https://github.com/user-attachments/assets/540e54ed-4cfa-4862-aca9-df7dd38aecc3)

	
	* this will let you hear what exactly you're cutting out, **just be sure to switch it back to low pass when you're done**.  this is really neat, you can hear all the junk noise you're EQ'ing out and getting rid of.
	  
	* **low end** - you can do this same trick on the left knob, and switch it over to low pass:
	  
	  ![[FL64_hmT3S5SlOp.gif]]
	
	* as you drag the slider over, you will hear more and more audio start to pick up. this is the noise you're cutting out from the low end. **be sure to switch this knob back to high pass when you're finished**.

2) **Fruity Parametric EQ 2: Part Two**


* plop a second *Fruity Parametric EQ 2* onto the master track, we can consider this as an **"enhancement EQ"**, because you will use this one to focus on enhancing different parts of your song.
  
	* ![[Pasted image 20241112211637.png]]

  
* with this second EQ, you'll want to move the knobs around until your song sounds better, typically the mid range knobs (3-5) need a little boost from here. keep your master levels in mind and don't boost the dB so much that you start clipping the audio, try to keep the master level at 0.

  
	* ![[Pasted image 20241112212002.png]]
	
	* *the hint panel is displaying 2.0 dB, and we can see that i've raised the yellow 4 knob to that amount.*


* basically the idea here is, if you have to go above 2 dB to make something in your song sound good, its probably not going to sound good on different sound systems. so go back to your song's main flp and fix it in the mix and start this whole process over.

3) **Patcher**
 
* add patcher to the master track and then click the presets button:


  ![[Pasted image 20241112212734.png]]

* find the preset called *"Mid Side EQ"* -- not just the one that says "Mid Side", make sure it has those lucky two letters "EQ" in it:

  
  ![[Pasted image 20241112212851.png]]

* this setup will use the **Mid Side Splitter** setting in **Stereo Shaper** to split the master audio into a Mid (center) and a Side (stereo width) channel. the side channel contains all of the sounds that are different between the left and right channels.

  
* so by using patcher in this way, we're gaining even more control of the overall final stereo output by finding the differences between the left and right stereo channels and EQ'ing them all at once, before routing them back into the final mix.

  
* you can use the same tricks above to isolate the frequency and slide it around to hear what you're going to be cutting out with this SIDE EQ patch.

  
* you can think of this as an additional **"enhancement EQ"**, the first one is sort of our generic master EQ just sculpting at a very broad range, with the second EQ and this final additional sidechannel patcher EQ we're really narrowing in on specific sounds we want to sculpt, thereby *enhancing* our overall track.
  ![[Pasted image 20241112213532.png]]  

* you can right-click the little arrow coming out of the MID one to mute it while you tweak the side one, i circled it in red above. this will let you hear exactly the differences between the left and right audio channels, before routing them back to the final mix. just be sure to unmute the MID routing when you're done, to restore the full stereo balance.



---
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

---

# Compression

you won't need to use compression on every single song, but it is really nice when you need it. you generally want to use compression on your master track in the following examples:


|   |   |   |
|---|---|---|
|**Too Punchy**|Tame transients, glue the mix together|Moderate ratio, medium attack, short release.|


|   |   |   |
|---|---|---|
|**Too Smooth**|Add energy and excitement|Higher ratio, fast attack, slower release, or parallel compression to preserve dynamics.|

---
**tools:**
1) **Fruity Limiter**
* in cases where your track is too punchy, you can do a simple compression by adding **Fruity Limiter** to the master track, clicking on "comp" for compression mode, and adjust the threshold down while moving the ratio setting up to about **2.0:1 ratio** (in the hint panel).

* *i'll discuss **compression ratios** later in this section as well, this is a good concept to be aware of*

* this is really quick and easy to do but might not give the best results, because fruity limiter is going to behave like a single band compressor and will raise/lower the volume of everything across the whole track. this would probably be most useful in cases where your song is "too smooth" and you just want a general volume boost, or if you're just feeling lazy or want a quick compression for some reason.

* ![[FL64_FgOwzsmrs2.gif]]
	 *example showing fruity limiter in compression mode, tweaking the threshold and ratio*

2) **Maximus**

* **Maximus** is a multiband compressor and will give much better results than just using a simple limiter, but will also be more complex and take a little more time to tweak it just right for your mix.
  
* right away, because it is a multiband compressor, you can click the "solo" button and then click through each of the different bands *(Low / Mid / High)* in the tool to help narrow down specific compression settings you want to apply to different frequency bands in your track -- very good.

* ![[FL64_pOEO0hTBGF.gif]]
		*example showing off the "solo" feature and listening to the different frequency bands*

* as per usual, **just be sure to turn off "solo" mode and/or go back to the MASTER band when finished**, or your track will be stuck in only one of the bands and not sound right.  

* *using maximus for mastering:*

* **compression envelopes**

* by default the **compression envelope** will typically be above anything in your mix (though not always) so by just leaving this envelope on default you might not actually be doing any compression at all. we want to tweak this compression envelope to change the threshold our compression will begin at, by dragging the middle dot in the envelope around
	
	* ![[FL64_q36JPfB2vc.gif]]
	* you can also adjust the final output dB using the right-most dot on the compression envelope
	  
	* ![[FL64_EOLeJdqyMY.gif]]

* again, because this is a multiband compressor, you can make different envelopes on each of the different frequency bands *(Low / Mid / High)* for different effects and results.
  
* after adjusting the compression envelopes as above, you can bump the **post** volume up to compensate for the volume change as well. in this example, i noticed the waveform was mostly around *-3 dB* so i adjust the post volume knob up to about *+3 dB* to compensate. you want to target the post volume because it is the volume that is coming out *after* compression.

* ![[FL64_kONDoTDOKM.gif]]

* **high dynamic range adjustments**

* this is where you'll adjust the *attack / release / sustain* knobs in the middle of maximus across all 3 bands, this will help you to control the HDR (high dynamic range) of your track

* ![[FL64_SQUqt3E7py.gif]]

* generally, release and sustain levels will be pretty good by default, and you'll likely need to lower the attack knob a bit especially in the **LOW** band for targeting your bass.

  
---
## Compression Ratios and Uses Summary

|                |                                                                                |                                                                          |                                                                     |
| -------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------- |
| **Ratio**      | **Purpose**                                                                    | **Applications**                                                         | **Characteristics**                                                 |
| 1.5:1 to 2:1   | Subtle, transparent compression to smooth out minor dynamics.                  | Master bus glue, acoustic music, light control on vocals or instruments. | Gentle and unobtrusive; retains natural dynamics.                   |
| 3:1 to 4:1     | More noticeable compression for tighter control while retaining natural sound. | General mixing tasks: vocals, bass guitars, and drums for consistency.   | Versatile for most mixing tasks; balances control and transparency. |
| 5:1 to 8:1     | Aggressive compression for tighter control or creative effects.                | Punchy vocals, drums, or parallel compression for energy.                | Noticeable compression; tightens dynamics but may sound unnatural.  |
| 10:1 and above | Hard limiting to clamp down signal exceeding the threshold.                    | Preventing clipping, live sound safety, or explosive drum effects.       | Extremely noticeable; clamps down on peaks significantly.           |
| Infinity:1     | Brick wall limiting to completely prevent signal above the threshold.          | Digital clipping prevention in mastering, creative destruction effects.  | Stops all signal above the threshold; can sound harsh or robotic.   |
