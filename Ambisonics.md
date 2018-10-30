A list of Ambisonics and binaural plugins (tested - or not - in REAPER on Windows 10).
- *2018-10-30: + Anaglyph*
- *2018-whatever : first draft*

# [The Ambisonic Toolkit](http://www.ambisonictoolkit.net/)

Free and open-source.

Video tutorials and example REAPER sessions are available.

-   OS : Windows/MacOS/Linux
-   Plugin format : JS
-   Ambisonics order : 1
-   Ambisonics format : FuMa
-   GUI style : from above plane (+ height slider)
-   Plugins:
    -   Encoders:
        -   mono:
            -   onmi
            -   planewave (with 2D panning)
            -   diffuser
            -   spreader
        -   stereo:
            -   stereo (with width control)
            -   SuperStereo
            -   UHJ
        -   quadraphonic
        -   5.0
        -   7.0
        -   pantophonic 2D (2 ÷ 16 speakers)
        -   periphonic 3D (2 ÷ 16 pairs of speakers)
    -   Decoders:
        -   mono
        -   stereo
            -   stereo (with width control)
            -   binaural
            -   UHJ
        -   quadraphonic
        -   5.0
        -   pantophonic 2D (2 ÷ 16 speakers)
        -   periphonic 3D (2 ÷ 16 pairs of speakers)
        -   "PsychoShelf" ("psychoacoustic shelf filtering to a first order B-format signal") (?)
    -   Converters (to/from FuMa B-format):
        -   A-format
        -   ACN SN3D/N3D
    -   Transformations: 
        -   direct (point)
        -   direct (plane)
        -   push / press / zoom / focus
        -   dominate
        -   mirror (point)
        -   mirror (plane)
        -   rotate / tilt / tumble
        -   near-field correction / proximity effect
    -   Tools:
        -   extract 4 channels (from up to 10 channels)
        -   mute/solo channels (4 ch)

# [IEM Plug-in Suite](https://plugins.iem.at/)

Free and open-source.

-   OS : Windows/MacOS/Linux
-   Plugin format : VST
-   Ambisonics order : 0 ÷ 7 (selectable in each plugin)
-   Ambisonics format : ambiX (ACN, SN3D/N3D)
-   GUI style : from above hemisphere (mostly, except the visualiser and the AllRADecoder)
-   Plugins:
    -   Encoders / panners:
        -   stereo / mono
        -   multi (1 ÷ 64 channels)
    -   Decoders:
        -   probe (mono, directional virtual mic)
        -   binaural
        -   simple : configuration-based (JSON files), with subwoofer
        -   AllRAD : configurable, 4 ÷ 64 speakers, can export the configuration for the SimpleDecoder
    -   Effects:
        -   omni compressor / limiter / brick-wall limiter (with 5 ms lookahead)
        -   directional compressor
        -   directivity shaper
        -   dual delay : *echo (not "delay")*; each line has rate (0 ÷ 500 ms), LFO, rotation (yaw), low/high cut filter, self- and cross-feedback, mix level
        -   fdn reverb : feedback-delay-network reverb, with eq
        -   room encoder : complex room reverb
    -   Tools:
        -   coordinate converter
        -   distance compensator : for up to 64 speakers
        -   matrix multiplier
        -   tool box : flip axes, order conversion, Lower Order Ambisonics weighting (none, maxrE, inPhase)
    -   Visualiser

# [ambiX](http://www.matthiaskronlachner.com/?p=2015)

Free and open-source.

-   OS : Windows/MacOS/Linux
-   Plugin format : VST
-   Ambisonics order : 1, 3, 5, 7 (4 version for each plugin)
-   Ambisonics format : ambiX (ACN, SN3D)
-   GUI style : mixed
-   Plugins:
    -   Encoders / panners : (GUI : from above hemisphere)
        -   mono
        -   stereo
        -   4 channels
        -   6 channels
        -   8 channels
    -   Decoders:
        -   binaural (IR-based)
        -   generic (IR-based) : up to 48 channels *(?)*
        -   virtual mics (8 channels) (GUI : frontal projection)
    -   Converters:
        -   any-to-any FuMa/ACN ordering, FuMa/SN3D/N3D normalisation; Condon-Shortley inversion; channel flipping
        -   maxre : apply or reciprocal apply spherical maxre weighting to suppress sidelobes *??, this one crashed my Reaper session*
    -   Transformations / effects:
        -   directional loudness (GUI : frontal projection)
        -   mirror
        -   rotator (GUI-less)
        -   rotator z
        -   warp
        -   widening : frequency dependant rotation around the z-axis

# [mcfx](http://www.matthiaskronlachner.com/?p=1910)

Free and open-source. Not strictly Ambisonics, but multi-channel (up to 64 channels) effects and utilities.

-   OS : Windows/MacOS/Linux
-   Plugin format : VST
-   Ambisonics order (max) : 7 (64 channels)
-   Plugins:
    -   Convolver : comes with a few IRs
    -   Delay : proper delay *(not echo)*, in samples and ms, 0 ÷ 500 ms (same setting for all channels)
    -   Filter : parametric EQ with spectrograph, low/high cut, low/high shelf, 2 peaks
    -   Gain delay : one setting per channel; gain (-18 ÷ +18 dB), delay (0 ÷ 500 ms), polarity, mute, solo, signal generator
    -   Meter : peak + ?? (VU?, rms?, compared to TBProAudio's mvMeter2, none of them)

# [WigWare](https://www.brucewiggins.co.uk/?page_id=78)

Gratis.

I didn't test the DirectX decoders.

-   OS : Windows/MacOS
-   Plugin format : VST, JS, DirectX
-   Ambisonics order : *variable* (max : 4)
-   Ambisonics format : FuMa
-   GUI style : GUI-less
-   Plugins:
    -   Encoders / panners:
        -   mono 3D 1st, 2nd and 3rd order
        -   *4 more mono encoders/panner that I can't get to work as expected*
    -   Decoders:
        -   5.0 : 1st and 4th order
        -   regular shape 4/6/8 speakers (2D) : 1st order
    -   Converters:
        -   any-to-any FuMa/ACN ordering, FuMa/SN3D/N3D normalisation : 3rd order (JS plugin)
        -   ambiX to TBE
        -   TBE to 2nd order FuMa 2D
        -   inverse filter for YouTube Spatial Audio : two versions (JS plugins)
    -   Reverbs : two plugins, 1st order
    -   Meter : multi-channel peak/VU (up to 64 channels) *(JS, included in REAPER)*

# [Blue Ripple Sound](http://www.blueripplesound.com/pro-audio-home)

Proprietary: some paid suites, and a gratis one ("O3A Core").

-   OS : Windows/MacOS
-   Plugin format : VST/AAX
-   Ambisonics order : 3
-   Ambisonics format : ambiX (ACN, SN3D)
-   GUI style : frontal projection (except for the mono panners and a visualiser)
-   Plugins (gratis suite):
    -   Encoders / panners:
        -   mono : different GUIs (frontal projection big/small, from above, GUI-less)
        -   stereo
        -   8-channel
    -   Decoders:
        -   mono:
            -   omni
            -   beamer (mono directional virtual mic)
        -   stereo: 
            -   basic/binaural *(?)*
            -   virtual microphones (2 channels, frontal, width control, shape control)
        -   5.1
    -   Converters:
        -   to/from ACN SN3D 1st and 2nd order
        -   to/from FuMa 3rd order
    -   Transformations:
        -   look
        -   rotation
        -   spatial delay : *echo (not "delay")*
    -   Tools:
        -   gain : 16 channels, -inf ÷ +30 dB
    -   Meters : per-order, not per-channel
    -   Visualisers : 4 types ("Flare" is very nice, imo)

# [SSA Plugins](https://www.ssa-plugins.com/)

Proprietary: some paid ones and two gratis ones.

-   OS : Windows/MacOS
-   Plugin format : VST/AAX/AU
-   Ambisonics order (max): 7
-   Channel ordering : ACN
-   Normalisation : *SN3D ?*
-   Plugins (gratis):
    -   stereo encoder / panner : 1st order
    -   meter : peak + rms (but TBProAudio's mvMeter2 rms mode gives me different (higher) readings), up to 64 channels (7th order), clearer graphics than the mcfx meter

# [Spatial Workstation – Facebook 360 Video](https://facebook360.fb.com/spatial-workstation/)

For mixing for 3D videos.

Gratis plugins, plus a standalone audio/video encoder and a standalone video player.

Video tutorials and example REAPER sessions are available.

-   OS : Windows/MacOS
-   Plugin format : VST3/AAX
-   Ambisonics order : 3
-   Ambisonics format : ambiX (ACN, SN3D), 
-   Plugins:
    -   Spatialiser (encoder / panner)
        -   input:
            -   mono
            -   stereo
            -   4.0
            -   5.0
            -   6.0
            -   7.0
            -   B-format FuMa 1st order
            -   B-format ambiX 1st/2nd/3rd order
        -   controls:
            -   position (with distance and spread)
            -   attenuation
            -   Doppler
            -   room
            -   video view
            -   GUI : from above plane
    -   Converter:
        -   input:
            -   B-format ambiX 2nd/3rd order
            -   Spatial Workstation 8 channels
        -   rotation
        -   output:
            -   binaural
            -   B-format ambiX 1st/2nd/3rd order
            -   Spatial Workstation 8 channel
    -   Control (with binaural decoder)
    -   Loudness meter

# [Anaglyph](http://anaglyph.dalembert.upmc.fr/)

High-definition Binaural spatialization engine.

**Not ambisonics** (I suppose).

-   OS : Windows/MacOS
-   Plugin format : VST
-   Ambisonics : *no*
    
# [HoaLibrary - High Order Ambisonics Library](http://hoalibrary.mshparisnord.fr/en)

*Unmaintained, not working*

# [VVAudio](http://www.vvaudio.com/)

*32 bit, I didn't check this*

# [Ironbridge Electronics - Ambisonic Auralizer Tools](http://www.ironbridge-elt.com/products/aat.html)

*32 bit, I didn't check this*

> Written with [StackEdit](https://stackedit.io/).
