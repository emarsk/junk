---


---

<p>A list of gratis and/or libre Ambisonics and binaural plugins (tested - or not - in REAPER on Windows 10).</p>
<ul>
<li><em>2018-10-30: + Anaglyph</em></li>
<li><em>2018-whatever : first draft</em></li>
</ul>
<h1 id="the-ambisonic-toolkit"><a href="http://www.ambisonictoolkit.net/">The Ambisonic Toolkit</a></h1>
<p>Free and open-source.</p>
<p>Video tutorials and example REAPER sessions are available.</p>
<ul>
<li>OS : Windows/MacOS/Linux</li>
<li>Plugin format : JS</li>
<li>Ambisonics order : 1</li>
<li>Ambisonics format : FuMa</li>
<li>GUI style : from above plane (+ height slider)</li>
<li>Plugins:
<ul>
<li>Encoders:
<ul>
<li>mono:
<ul>
<li>onmi</li>
<li>planewave (with 2D panning)</li>
<li>diffuser</li>
<li>spreader</li>
</ul>
</li>
<li>stereo:
<ul>
<li>stereo (with width control)</li>
<li>SuperStereo</li>
<li>UHJ</li>
</ul>
</li>
<li>quadraphonic</li>
<li>5.0</li>
<li>7.0</li>
<li>pantophonic 2D (2 ÷ 16 speakers)</li>
<li>periphonic 3D (2 ÷ 16 pairs of speakers)</li>
</ul>
</li>
<li>Decoders:
<ul>
<li>mono</li>
<li>stereo
<ul>
<li>stereo (with width control)</li>
<li>binaural</li>
<li>UHJ</li>
</ul>
</li>
<li>quadraphonic</li>
<li>5.0</li>
<li>pantophonic 2D (2 ÷ 16 speakers)</li>
<li>periphonic 3D (2 ÷ 16 pairs of speakers)</li>
<li>“PsychoShelf” (“psychoacoustic shelf filtering to a first order B-format signal”) (?)</li>
</ul>
</li>
<li>Converters (to/from FuMa B-format):
<ul>
<li>A-format</li>
<li>ACN SN3D/N3D</li>
</ul>
</li>
<li>Transformations:
<ul>
<li>direct (point)</li>
<li>direct (plane)</li>
<li>push / press / zoom / focus</li>
<li>dominate</li>
<li>mirror (point)</li>
<li>mirror (plane)</li>
<li>rotate / tilt / tumble</li>
<li>near-field correction / proximity effect</li>
</ul>
</li>
<li>Tools:
<ul>
<li>extract 4 channels (from up to 10 channels)</li>
<li>mute/solo channels (4 ch)</li>
</ul>
</li>
</ul>
</li>
</ul>
<h1 id="iem-plug-in-suite"><a href="https://plugins.iem.at/">IEM Plug-in Suite</a></h1>
<p>Free and open-source.</p>
<ul>
<li>OS : Windows/MacOS/Linux</li>
<li>Plugin format : VST</li>
<li>Ambisonics order : 0 ÷ 7 (selectable in each plugin)</li>
<li>Ambisonics format : ambiX (ACN, SN3D/N3D)</li>
<li>GUI style : from above hemisphere (mostly, except the visualiser and the AllRADecoder)</li>
<li>Plugins:
<ul>
<li>Encoders / panners:
<ul>
<li>stereo / mono</li>
<li>multi (1 ÷ 64 channels)</li>
</ul>
</li>
<li>Decoders:
<ul>
<li>probe (mono, directional virtual mic)</li>
<li>binaural</li>
<li>simple : configuration-based (JSON files), with subwoofer</li>
<li>AllRAD : configurable, 4 ÷ 64 speakers, can export the configuration for the SimpleDecoder</li>
</ul>
</li>
<li>Effects:
<ul>
<li>omni compressor / limiter / brick-wall limiter (with 5 ms lookahead)</li>
<li>directional compressor</li>
<li>directivity shaper</li>
<li>dual delay : <em>echo (not “delay”)</em>; each line has rate (0 ÷ 500 ms), LFO, rotation (yaw), low/high cut filter, self- and cross-feedback, mix level</li>
<li>fdn reverb : feedback-delay-network reverb, with eq</li>
<li>room encoder : complex room reverb</li>
</ul>
</li>
<li>Tools:
<ul>
<li>coordinate converter</li>
<li>distance compensator : for up to 64 speakers</li>
<li>matrix multiplier</li>
<li>tool box : flip axes, order conversion, Lower Order Ambisonics weighting (none, maxrE, inPhase)</li>
</ul>
</li>
<li>Visualiser</li>
</ul>
</li>
</ul>
<h1 id="ambix"><a href="http://www.matthiaskronlachner.com/?p=2015">ambiX</a></h1>
<p>Free and open-source.</p>
<ul>
<li>OS : Windows/MacOS/Linux</li>
<li>Plugin format : VST</li>
<li>Ambisonics order : 1, 3, 5, 7 (4 version for each plugin)</li>
<li>Ambisonics format : ambiX (ACN, SN3D)</li>
<li>GUI style : mixed</li>
<li>Plugins:
<ul>
<li>Encoders / panners : (GUI : from above hemisphere)
<ul>
<li>mono</li>
<li>stereo</li>
<li>4 channels</li>
<li>6 channels</li>
<li>8 channels</li>
</ul>
</li>
<li>Decoders:
<ul>
<li>binaural (IR-based)</li>
<li>generic (IR-based) : up to 48 channels <em>(?)</em></li>
<li>virtual mics (8 channels) (GUI : frontal projection)</li>
</ul>
</li>
<li>Converters:
<ul>
<li>any-to-any FuMa/ACN ordering, FuMa/SN3D/N3D normalisation; Condon-Shortley inversion; channel flipping</li>
<li>maxre : apply or reciprocal apply spherical maxre weighting to suppress sidelobes <em>??, this one crashed my Reaper session</em></li>
</ul>
</li>
<li>Transformations / effects:
<ul>
<li>directional loudness (GUI : frontal projection)</li>
<li>mirror</li>
<li>rotator (GUI-less)</li>
<li>rotator z</li>
<li>warp</li>
<li>widening : frequency dependant rotation around the z-axis</li>
</ul>
</li>
</ul>
</li>
</ul>
<h1 id="mcfx"><a href="http://www.matthiaskronlachner.com/?p=1910">mcfx</a></h1>
<p>Free and open-source. Not strictly Ambisonics, but multi-channel (up to 64 channels) effects and utilities.</p>
<ul>
<li>OS : Windows/MacOS/Linux</li>
<li>Plugin format : VST</li>
<li>Ambisonics order (max) : 7 (64 channels)</li>
<li>Plugins:
<ul>
<li>Convolver : comes with a few IRs</li>
<li>Delay : proper delay <em>(not echo)</em>, in samples and ms, 0 ÷ 500 ms (same setting for all channels)</li>
<li>Filter : parametric EQ with spectrograph, low/high cut, low/high shelf, 2 peaks</li>
<li>Gain delay : one setting per channel; gain (-18 ÷ +18 dB), delay (0 ÷ 500 ms), polarity, mute, solo, signal generator</li>
<li>Meter : peak + ?? (VU?, rms?, compared to TBProAudio’s mvMeter2, none of them)</li>
</ul>
</li>
</ul>
<h1 id="wigware"><a href="https://www.brucewiggins.co.uk/?page_id=78">WigWare</a></h1>
<p>Gratis.</p>
<p>I didn’t test the DirectX decoders.</p>
<ul>
<li>OS : Windows/MacOS</li>
<li>Plugin format : VST, JS, DirectX</li>
<li>Ambisonics order : <em>variable</em> (max : 4)</li>
<li>Ambisonics format : FuMa</li>
<li>GUI style : GUI-less</li>
<li>Plugins:
<ul>
<li>Encoders / panners:
<ul>
<li>mono 3D 1st, 2nd and 3rd order</li>
<li><em>4 more mono encoders/panner that I can’t get to work as expected</em></li>
</ul>
</li>
<li>Decoders:
<ul>
<li>5.0 : 1st and 4th order</li>
<li>regular shape 4/6/8 speakers (2D) : 1st order</li>
</ul>
</li>
<li>Converters:
<ul>
<li>any-to-any FuMa/ACN ordering, FuMa/SN3D/N3D normalisation : 3rd order (JS plugin)</li>
<li>ambiX to TBE</li>
<li>TBE to 2nd order FuMa 2D</li>
<li>inverse filter for YouTube Spatial Audio : two versions (JS plugins)</li>
</ul>
</li>
<li>Reverbs : two plugins, 1st order</li>
<li>Meter : multi-channel peak/VU (up to 64 channels) <em>(JS, included in REAPER)</em></li>
</ul>
</li>
</ul>
<h1 id="blue-ripple-sound"><a href="http://www.blueripplesound.com/pro-audio-home">Blue Ripple Sound</a></h1>
<p>Proprietary: some paid suites, and a gratis one (“O3A Core”).</p>
<ul>
<li>OS : Windows/MacOS</li>
<li>Plugin format : VST/AAX</li>
<li>Ambisonics order : 3</li>
<li>Ambisonics format : ambiX (ACN, SN3D)</li>
<li>GUI style : frontal projection (except for the mono panners and a visualiser)</li>
<li>Plugins (gratis suite):
<ul>
<li>Encoders / panners:
<ul>
<li>mono : different GUIs (frontal projection big/small, from above, GUI-less)</li>
<li>stereo</li>
<li>8-channel</li>
</ul>
</li>
<li>Decoders:
<ul>
<li>mono:
<ul>
<li>omni</li>
<li>beamer (mono directional virtual mic)</li>
</ul>
</li>
<li>stereo:
<ul>
<li>basic/binaural <em>(?)</em></li>
<li>virtual microphones (2 channels, frontal, width control, shape control)</li>
</ul>
</li>
<li>5.1</li>
</ul>
</li>
<li>Converters:
<ul>
<li>to/from ACN SN3D 1st and 2nd order</li>
<li>to/from FuMa 3rd order</li>
</ul>
</li>
<li>Transformations:
<ul>
<li>look</li>
<li>rotation</li>
<li>spatial delay : <em>echo (not “delay”)</em></li>
</ul>
</li>
<li>Tools:
<ul>
<li>gain : 16 channels, -inf ÷ +30 dB</li>
</ul>
</li>
<li>Meters : per-order, not per-channel</li>
<li>Visualisers : 4 types (“Flare” is very nice, imo)</li>
</ul>
</li>
</ul>
<h1 id="ssa-plugins"><a href="https://www.ssa-plugins.com/">SSA Plugins</a></h1>
<p>Proprietary: some paid ones and two gratis ones.</p>
<ul>
<li>OS : Windows/MacOS</li>
<li>Plugin format : VST/AAX/AU</li>
<li>Ambisonics order (max): 7</li>
<li>Channel ordering : ACN</li>
<li>Normalisation : <em>SN3D ?</em></li>
<li>Plugins (gratis):
<ul>
<li>stereo encoder / panner : 1st order</li>
<li>meter : peak + rms (but TBProAudio’s mvMeter2 rms mode gives me different (higher) readings), up to 64 channels (7th order), clearer graphics than the mcfx meter</li>
</ul>
</li>
</ul>
<h1 id="spatial-workstation-–-facebook-360-video"><a href="https://facebook360.fb.com/spatial-workstation/">Spatial Workstation – Facebook 360 Video</a></h1>
<p>For mixing for 3D videos.</p>
<p>Gratis plugins, plus a standalone audio/video encoder and a standalone video player.</p>
<p>Video tutorials and example REAPER sessions are available.</p>
<ul>
<li>OS : Windows/MacOS</li>
<li>Plugin format : VST3/AAX</li>
<li>Ambisonics order : 3</li>
<li>Ambisonics format : ambiX (ACN, SN3D),</li>
<li>Plugins:
<ul>
<li>Spatialiser (encoder / panner)
<ul>
<li>input:
<ul>
<li>mono</li>
<li>stereo</li>
<li>4.0</li>
<li>5.0</li>
<li>6.0</li>
<li>7.0</li>
<li>B-format FuMa 1st order</li>
<li>B-format ambiX 1st/2nd/3rd order</li>
</ul>
</li>
<li>controls:
<ul>
<li>position (with distance and spread)</li>
<li>attenuation</li>
<li>Doppler</li>
<li>room</li>
<li>video view</li>
<li>GUI : from above plane</li>
</ul>
</li>
</ul>
</li>
<li>Converter:
<ul>
<li>input:
<ul>
<li>B-format ambiX 2nd/3rd order</li>
<li>Spatial Workstation 8 channels</li>
</ul>
</li>
<li>rotation</li>
<li>output:
<ul>
<li>binaural</li>
<li>B-format ambiX 1st/2nd/3rd order</li>
<li>Spatial Workstation 8 channel</li>
</ul>
</li>
</ul>
</li>
<li>Control (with binaural decoder)</li>
<li>Loudness meter</li>
</ul>
</li>
</ul>
<h1 id="anaglyph"><a href="http://anaglyph.dalembert.upmc.fr/">Anaglyph</a></h1>
<p>High-definition Binaural spatialization engine.</p>
<p><strong>Not ambisonics</strong> (I suppose).</p>
<ul>
<li>OS : Windows/MacOS</li>
<li>Plugin format : VST</li>
<li>Ambisonics : <em>no</em></li>
</ul>
<h1 id="hoalibrary---high-order-ambisonics-library"><a href="http://hoalibrary.mshparisnord.fr/en">HoaLibrary - High Order Ambisonics Library</a></h1>
<p><em>Unmaintained, not working</em></p>
<h1 id="vvaudio"><a href="http://www.vvaudio.com/">VVAudio</a></h1>
<p><em>32 bit, I didn’t check this</em></p>
<h1 id="ironbridge-electronics---ambisonic-auralizer-tools"><a href="http://www.ironbridge-elt.com/products/aat.html">Ironbridge Electronics - Ambisonic Auralizer Tools</a></h1>
<p><em>32 bit, I didn’t check this</em></p>

