# p5.sing (not a thing yet)

An open source (maybe ML-based) vocal synthesizer that runs on the browser.

While I was at sfpc in 2015 I wanted to make a sort of singing text-to-speech, or maybe a vocaloid. I experimented with [Festival](http://www.cstr.ed.ac.uk/projects/festival/) and other stuff I don't really remember. I did find [a perl script](https://code.google.com/archive/p/sing/) that takes text and ABC notation as input, then tweaks the utterance rate of Mac's say command to make it sing. Of course I made it sing the first phrase from _A Bicycle Built For Two_ then [put in on some synth](./daisy.mp3). But other than that I never got anywhere far.

Now it's almost 2018, as [samim comments on Google's Tacotron 2](https://twitter.com/samim/status/943092532396863488) machine learning seems to be at a state where it can do speech, and potentially singing, really well. There's even a [start-up pitching that](https://www.voiceful.io/). Combine this with all the [generative music composition stuff coming up](https://medium.com/artists-and-machine-intelligence/neural-nets-for-generating-music-f46dffac21c0) from start-ups like Jukedeck or Amper, as well as from big companies' in-house labs, it seems that we can expect to see consumer-level pop song generation or something similar pretty soon. The fact that deep learning libraries can now run in the browser will also help, although the aforementioned start-ups seem to keep their sauce a secret (i.e. keep the actual generation mechanism in the cloud beyond the browser). 

This seems to indicate to me that an open source JavaScript (because the web) speech synthesizer that maybe stitches together available ML TTS models and melody generators should be feasible. If possible, [p5.js](https://github.com/processing/p5.js) seems to be a good place to implement such a ~~sing~~thing, considering its focus on making technology accessible to diverse people and because it's a quite an all-round creative toolset. It also already has p5.speech and p5.sound, though I'm not sure they apply here because they are wrappers around the Web Speech API and Web Audio API respectively. Although I don't think I am familiar enough with TTS to do this right now (nor do I have the time, really), but I will definitely be keeping my ears open if anyone engages in something similar.

---

just saw this meet-up notice: https://www.facebook.com/events/1983316915270556/

---

- on how to take speech output and use it for audio input: https://stackoverflow.com/a/45003549/8157867
- web audio vocoder: https://github.com/cwilso/Vocoder
