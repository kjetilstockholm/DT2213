---
theme: default
background: 638358609_1493615702772846_7723936173858625006_n.jpg?auto=format&fit=crop&q=80
#class: text-white
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## From Shape to Sound
  Teaching Nonlinear Music through Spatial Form
title: Shape2Sound
---

<div class="absolute top-[7%] left-1/2 -translate-x-1/2">
  <img src="/KTH_logo_RGB_vit.svg" class="w-35 " />
</div>

<div class="pt-[180px]">

# From Shape to Sound
## Teaching Nonlinear Music through Spatial Form

K. Falkenberg, H. Lindetorp, C. Akner-Koler

**INTED 2026**

<div class="pt-12 font-medium">
  Kjetil Falkenberg <br>
  <span class="opacity-70">KTH Royal Institute of Technology</span>
</div>

</div>


<div class="absolute bottom-2 right-8 flex items-center gap-6">
  <img src="/KTH_logo_RGB_vit.svg" class="w-16" />
  <img src="/KMH_logo.png" class="w-16" translate-y-2/>
  <img src="/Konstfack-liten.png" class="w-16" translate-y-1/>
</div>


<style>
h1, h3, p, div {
  color: white; 
  text-shadow: 0px 4px 10px rgba(0,0,0,0.6);
}
</style>


---
layout: split
---

# A Pedagogical Challenge
Nonlinear music is highly prominent in modern media (e.g., game audio), but teaching it presents significant obstacles.

* **The Representation Gap** 

<div v-click="1" class="expandable">Traditional tools rely on abstract notation, code-heavy environments, or fixed timelines.</div>

* **Degrees of Freedom**

<div v-click="2" class="expandable">Students are forced to engage with dynamic, relational phenomena through symbolic and static interfaces.</div>

* **Our Approach** 

<div v-click="3" class="expandable">We bridge this gap by translating abstract concepts into tangible, cross-modal experiences with low-threshold technologies.</div>

::right::

<div class="flex flex-col items-center gap-6 p-4">
  <img src="/vlcsnap-2026-02-22-14h04m31s844.jpg" class="w-[170px] rounded-lg shadow-lg" />

  <blockquote class="text-lg italic border-l-4 border-blue-500 bg-blue-50/10 p-3 rounded-r-lg w-full">
    "Simplicity becomes an enabler, not a limitation."
  </blockquote>

  <video src="/20260219_193827.mp4" autoplay loop muted class="w-[200px] rounded-lg shadow-lg"></video>
</div>

<style>
.expandable {
  @apply text-sm opacity-100 pl-6 mt-1 text-#1954a6;
  
  max-height: 60px; 
  overflow: hidden;
  transition: all 0.4s ease-in-out;
}

.expandable.slidev-vclick-hidden {
  max-height: 0;
  opacity: 0;
  margin-top: 0; 
}

</style>

---
layout: split
---

# Theoretical Framework

* #### 4E Cognition & Embodiment

<div v-click="1" class="expandableref">Abrahamson; Godøy; Leman; Dourish</div>
<div v-click="2" class="expandable">Thinking as <span v-mark.circle.orange="5">enacted process</span>, embodied and extended into the physical.</div>
<div v-click="2" class="expandable">Abstract concepts become accessible through bodily action.</div>

* #### Form Pedagogy

<div v-click="1" class="expandableref">Kostellow; Stone; Akner-Koler</div>

<div v-click="3" class="expandable">Insight is derived through handling, rotating, and folding physical forms. </div>
<div v-click="3" class="expandable">The manipulations act as <span v-mark.circle.orange="5">epistemic actions</span>.</div>

* #### Interactive music

<div v-click="1" class="expandableref">Jensenius; Lindetorp; Magnusson</div>
<div v-click="4" class="expandable">Music is not a static series of notes.</div>
<div v-click="4" class="expandable"><span v-mark.circle.orange="5">Action-sound couplings</span> between form and rotation. </div>


::right::

<div class="flex flex-col items-center justify-center h-full gap-8 p-4">
  <blockquote class="text-lg italic border-l-4 border-emerald-500 bg-emerald-50/10 p-4 rounded-r-lg">
    "Nonlinear music functions much like a kinetic sculpture, where finding its 'meaning' arises through movement and shifting perspective." 
  </blockquote>

  <img src="/Screenshot 2026-02-21 at 19.50.08.jpg" class="w-[250px] rounded-xl shadow-xl border border-gray-200/20" />
</div>


<style>
.expandable {
  @apply text-sm opacity-100 pl-6 mt-1 text-#1954a6;
  
  max-height: 60px; 
  overflow: hidden;
  transition: all 0.4s ease-in-out;
}

.expandable.slidev-vclick-hidden {
  max-height: 0;
  opacity: 0;
  margin-top: 0; 
}

.expandableref {
  @apply text-sm opacity-100 pl-6 mt-1 italic;
  
  max-height: 60px; 
  overflow: hidden;
  transition: all 0.4s ease-in-out;
}

.expandableref.slidev-vclick-hidden {
  max-height: 0;
  opacity: 0;
  margin-top: 0; 
}

</style>



---
layout: split-70
---

# The Technical Setup

| *Component* | *Function* |
| --- | --- | 
| **Materials** | Cardboard, mat knife, straight edge ruler |
| **Technical** | Webcam, computer, loudspeaker, lighting, green screen  |
| **Vision** | MediaPipe for real-time tracking of colors via a webcam |
| **Audio** | WebAudio/WAXML for mapping visuals to sound |
| **Interface** | Browser-native to reduce cognitive overhead of DAWs |

::right::


<p class="text-sm italic text-center text-gray-500">We prioritize transparent and accessible technology to keep the focus on embodied experience.</p>

<p class="text-sm italic text-center text-gray-500">The cardboard form itself becomes an embodied interface for navigating nonlinear musical logic.</p>

<p class="text-sm text-center"><span v-click="1" v-mark.red="1">Low threshold</span><span v-click="2">, </span><span v-click="2" v-mark.blue="2">High ceiling</span><span v-click="3">, </span><span v-click="3" v-mark.green="3">Wide walls</span></p>


---
layout: split
---

# Workshop Phase 1

Constructing physical interfaces to control musical structures.

* **Materials**: Cardboard, mat knife, straight edge ruler.
* **The Task**: Cut straight scores and fold to create interconnected rectangular planes.
* **Spatial Focus**: Exploring interior/exterior spaces, openings, enclosures, and how shadows and light modulate the composition.
* **Color Coding**: Each side is painted a unique color, establishing a perceptual vocabulary where planes become relational units.


::right::


<div class="flex flex-col items-center justify-center h-full gap-6">
  <div>
    <video src="/karen_stone_scoring_and_folding_img_6212 (1080p).mp4" autoplay loop muted class="w-[150px] rounded-lg shadow-lg"></video>
    <div class="text-xs text-center mt-2 opacity-70 italic">Demonstration by Karen Stone</div>
  </div>

  <img src="/vlcsnap-2026-02-22-11h43m36s369.jpg" class="w-[150px] rounded-lg shadow-lg" />
</div>

---
layout: split
---

# Workshop Phase 2

Mapping Shape to Sound: Translating spatial segmentation.

* **Isomorphism**: Structural correspondence between the physical shape and the musical structure. 
* **Musification**: Mapping data into musical structures so students perceive the underlying logic.
* **Relational Blocks**: Music is treated not as a continuous timeline, but as distinct blocks that can be activated, layered, or bypassed based on spatial navigation.

::right::

<div class="flex flex-col items-center justify-center h-full gap-6">
  <video src="/20260128_113942.mp4" autoplay loop muted class="w-[250px] rounded-lg shadow-lg"></video>
    <div class="text-xs text-center mt-2 opacity-70 italic">From sessions 1 (above) and 2 (below)</div>
  <img src="/20260219_150605.jpg" class="w-[250px] rounded-lg shadow-lg" />
</div>

---
layout: split-70
---

# Results: 3 workshops

<div class="flex flex-col justify-center gap-2 mt-8">
  <img src="/result1.jpg" class="w-full rounded-lg shadow-md" />
  <img src="/result3.jpg" class="w-full rounded-lg shadow-md" />
  <img src="/result4.jpg" class="w-full rounded-lg shadow-md" />
</div>

::right::


<ol class="list-none mt-8 space-y-4">
  <li v-click="1">
    <strong class="text-xl">Shape2Sound</strong>
    <div v-click="2" class="expandable">Synth tone</div>
    <div v-click="3" class="expandable">Mixing different parameters to show that rotation changes sound</div>
  </li>
  <li v-click="1">
    <strong class="text-xl">Shape2Sound</strong>
    <div v-click="2" class="expandable">Non-linear music</div>
    <div v-click="4" class="expandable">Playing different activity levels of six instruments to show non-linear logic</div>
  </li>
  <li v-click="1">
    <strong class="text-xl">Repair Vinyl</strong>
    <div v-click="1" text-sm italic>with Ernesto Garcia</div>
    <div v-click="2" class="expandable">Non-linear music</div>
    <div v-click="5" class="expandable">Crossfading between several sound sources to demonstrate other type of non-linearity</div>
  </li>
</ol>

<style>
.expandable {
  @apply text-sm opacity-100 pl-6 mt-1 text-#1954a6;
  
  max-height: 60px; 
  overflow: hidden;
  transition: all 0.4s ease-in-out;
}

.expandable.slidev-vclick-hidden {
  max-height: 0;
  opacity: 0;
  margin-top: 0; 
}
</style>


---
layout: center
---

# DEMO 1: Shape2SOUND

---
layout:default
---

<div class="absolute left-8 top-1/2 -translate-y-1/2 z-10 bg-white/80 p-4 rounded-xl shadow-xl backdrop-blur-sm">
  <h3 class="text-sm text-center mt-0 mb-2 font-bold text-gray-800">TEST IT!</h3>
  <img src="/qrcode_shape2sound.png" class="w-32 rounded-lg" />
</div>

<div class="ml-[100px] relative w-[calc(100%-100px)] h-full overflow-hidden rounded-2xl shadow-2xl">
  <iframe 
    src="https://smcresearch.se/apps/shape2sound" 
    class="absolute top-0 left-0 w-[200%] h-[200%] origin-top-left scale-50 border-none"
    allow="camera; microphone"
  ></iframe>
</div>


---
layout: center
---

# DEMO 2: Repair vinyl


---
layout:default
---

<div class="absolute left-8 top-1/2 -translate-y-1/2 z-10 bg-white/80 p-4 rounded-xl shadow-xl backdrop-blur-sm">
  <h3 class="text-sm text-center mt-0 mb-2 font-bold text-gray-800">TEST IT!</h3>
  <img src="/qrcode_repair.png" class="w-32 rounded-lg" />
</div>

<div class="ml-[100px] relative w-[calc(100%-100px)] h-full overflow-hidden rounded-2xl shadow-2xl">
  <iframe 
    src="https://smcresearch.se/apps/vinyltracker" 
    class="absolute top-0 left-0 w-[200%] h-[200%] origin-top-left scale-50 border-none"
    allow="camera; microphone"
  ></iframe>
</div>


---
layout: split
---

# Outcomes and Implications


* **Improvements**

<div v-click="1" class="expandable">Fix better tracking.</div>

* **Cross-Disciplinary Dialogue**

<div v-click="2" class="expandable">Levels differences between art, design, and engineering students.</div>

* **Embodied Understanding**

<div v-click="3" class="expandable">Students don't just understand the system symbolically—they <span v-mark.green="3">feel</span> it behaving through rotation, occlusion, and proximity.</div>

* **Future Work**

<div v-click="4" class="expandable">Implementation in wider teaching contexts and evaluating learning outcomes.</div>


::right::

<div class="flex flex-col items-center justify-center h-full gap-6">
  <img src="/IMG_6420.jpg" class="w-[350px] rounded-lg shadow-lg" />
</div>

<style>
.expandable {
  @apply text-sm opacity-100 pl-6 mt-1 text-#1954a6;
  
  max-height: 60px; 
  overflow: hidden;
  transition: all 0.4s ease-in-out;
}

.expandable.slidev-vclick-hidden {
  max-height: 0;
  opacity: 0;
  margin-top: 0; 
}

</style>


---
layout: default
class: text-center text-white
---

<div class="absolute top-0 left-0 w-full h-full z-[-1]">
  <img src="/form.jpg" class="w-full h-full object-cover" />
  <div class="absolute top-0 left-0 w-full h-full bg-black/50"></div>
</div>

<div class="absolute top-5 left-5 flex flex-col items-center gap-8">
  <img src="/KTH_logo_RGB_vit.svg" class="w-32" />
  <img src="/KMH_logo.png" class="w-28" />
  <img src="/Konstfack-liten.png" class="w-28" />
</div>

<div class="pt-[120px] flex flex-col items-center">

# Thank You!

<br>

<div class="text-sm font-bold opacity-100">
  Full paper:<br>
  <img src="/qrcode_paper.png" class="w-32 rounded-lg block m-auto mt-3 mb-3 shadow-lg" />
  Contact: kjetil@kth.se
</div>

<div class="mt-24 text-xs opacity-80 max-w-lg">
  Funding provided by NAVET (KTH Centre for Research in Art, Technology and Design)
</div>

</div>

<style>
h1, p, span, div {
  text-shadow: 0px 4px 10px rgba(0,0,0,0.8);
}
</style>

