---
# You can also start simply with 'default'
theme: neversink
neversink_slug: 2026-03-24 DElab meeting
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Matching Pennies in Mice and Monkeys
info: |
  Timothy Sit
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
colorSchema: light
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: fade
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# open graph
seoMeta:
  # By default, Slidev will use ./og-image.png if it exists,
  # or generate one from the first slide if not found.
  ogImage: auto
  # ogImage: https://cover.sli.dev
---



# Studying strategic stochasticity in Mice and Monkeys

Tim Sit | 2026-03-24

<img src="/im_so_random.png" class="mt-10 mx-auto w-[60%]" />


<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade
layout: default
---

# When you have to be strategically random to survive

<div class="flex flex-col items-center justify-center text-center gap-0">

  <!-- Image appears second -->
  <img 
    v-click="1"
    src="/driver-and-humphries-1970.png" 
    class="w-[35%] object-contain  ml-70"
  />

  <!-- Quote appears first -->
  <div v-click="2" class="max-w-3xl text-lg italic leading-relaxed">
    “Protean behaviour is defined as that behaviour which is sufficiently unsystematic 
    to prevent a reactor predicting in detail the position or actions of the actor.”
    <br/>
    <span class="text-sm not-italic opacity-70">
      — Humphries & Driver (1970)
    </span>
  </div>



</div>


---
transition: fade
layout: default
---

# Multiple species exhibit strategic stochasticity

<div class="grid grid-cols-3 gap-6 w-full items-start">

<!-- Column 1 -->
<div v-click="1" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-sm font-semibold leading-snug max-w-xs">
    Fish increase path complexity after being poked
  </div>

  <img
    src="/pacific-blue-eye.jpg"
    class="h-40 object-contain rounded-lg"
  />
  <img
    src="/blue-eye-fish-entropy.png"
    class="h-40 object-contain rounded-lg"
  />
  <div class="text-xs leading-snug italic max-w-xs">
    Herbert-Read et al. 2015<br>
    <span class="not-italic">
      Escape path complexity and its context dependency in Pacific blue-eyes
    </span>
  </div>
</div>

<!-- Column 2 -->
<div v-click="2" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-sm font-semibold leading-snug max-w-xs">
    Male bird absence duration becomes more unpredictable as their mate approach fertile periods
  </div>

  <img
    src="/kittiwake_adult.jpg"
    class="h-40 object-cover object-top rounded-lg mt--5"
  />
  <img
    src="/richard-wagner-2004.png"
    class="h-40 object-contain rounded-lg"
  />
  <div class="text-xs leading-snug italic max-w-xs">
    Richard Wagner et al. 2004<br>
    <span class="not-italic">
      Is Male Unpredictability a Paternity Assurance Strategy?
    </span>
  </div>
</div>

<!-- Column 3 -->
<div v-click="3" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-sm font-semibold leading-snug max-w-xs">
    Humans can learn to draw random rectangles based on feedback alone
  </div>

  <img
    src="/mondrian.jpg"
    class="h-40 object-contain rounded-lg"
  />
  <img
    src="/ross-and-neuringer-2001.png"
    class="h-40 object-contain rounded-lg"
  />
  <div class="text-xs leading-snug italic max-w-xs">
    Ross and Neuringer 2002<br>
    <span class="not-italic">
      Reinforcement of variations and repetitions along three independent response dimensions
    </span>
  </div>
</div>

</div>


---
transition: fade
layout: default
---


# Studying strategic stochasticity using matching pennies


<div class="relative w-full">

  <img v-click="1" src="/MP_task.png" class="w-full transition-opacity duration-500"
  :class="$clicks >= 2 ? 'opacity-30' : 'opacity-100'" />

  <div v-click="1" class="absolute bottom-4 left-6 text-sm opacity-70">
    Project led by Joanna Aloor
  </div>

  <!-- Monkeys -->
  <div
    v-click="2"
    class="absolute border border-black rounded-sm"
    style="left: 8%; top: 10%; width: 60%;"
  >
    <div class="absolute -top-6 left-0 bg-black/100 text-white text-s px-2 py-0 rounded-sm">
      Monkeys
    </div>
    <img
      src="/lee-2004-cognitive-brain-research.png"
      class="w-full object-contain"
    />
  </div>

  <!-- Rats -->
  <div
    v-click="3"
    class="absolute border border-black rounded-sm"
    style="left: 20%; top: 40%; width: 50%;"
  >
    <div class="absolute -top-6 left-0 bg-black/100 text-white text-s px-2 py-0 rounded-sm">
      Rats
    </div>
    <img
      src="/tervo-cell-2014.png"
      class="w-full object-contain"
    />
  </div>

  <!-- Mice -->
  <div
    v-click="4"
    class="absolute border border-black rounded-sm"
    style="left: 40%; top: 70%; width: 60%;"
  >
    <div class="absolute -top-6 left-0 bg-black/100 text-white text-s px-2 py-0 rounded-sm">
      Mice
    </div>
    <img
      src="/wang-2022-eNeuro.png"
      class="w-full object-contain"
    />
  </div>

</div>


---
transition: fade
layout: default 
---

# Mice learn to make more stochastic choices 


<div class="ml-20 mt-5">
<img src="/mouse_example_choices_2.png" class="opacity-100 w-[80%] mb-8" v-click="1"/>

<img src="/learning_summary_horizontal.png" class="opacity-100 w-[90%]" v-click="2"/>
</div>


---
transition: fade
layout: default 
---


# Mice behaviour can be broadly divided into three states



<img src="/GLM-HMM-cartoon_v1.svg" class="opacity-100 w-[50%]" v-click="1"/>

<img src="/clustered_glm_weights_cosyneabstract2025.svg" class="opacity-100 w-[60%]" v-click="2"/>


<div v-click="3" class="absolute top-[55%] left-150 w-[70%] -translate-y-1/2">
  <img src="/average_pstate_smooth_cosyneabstract2025.svg" class="opacity-100 w-[50%]"/>
</div>


<div class="absolute bottom-4 left-6 text-sm opacity-70">
GLM-HMM from Ashwoord 2022
</div>

---
transition: fade
class: flex flex-col justify-center
---

# Overview

<v-click>

**Past** (last lab meeting on October 2025)

</v-click>

<v-clicks>

1. Analysis of photometry data during MP -> Cosyne poster
2. A pair of multiplayer MP mice

</v-clicks>

<v-click>

**Present**

</v-click>

<v-clicks>

1. <span v-mark.highlight.teal="{ at: 11}">MP widefield + monkey comparison paper</span>
2. Some variations of multiplayer MP in mice
3. Human MP pilots

</v-clicks>

<v-click>

**Future**

</v-click>

<v-clicks>

1. More human and mice multiplayer MP
2. MP + Neuropixels

</v-clicks>




---
layout: section
color: teal 
transition: fade
---

# Part I: Mouse and monkey matching pennies behaviour comparison


--- 
layout: top-title-two-cols
columns: is-6
transition: fade 
clicks: 6
color: teal
---

:: title ::

# Monkey matching pennies dataset

:: left :: 

<img src="/monkey-algorithms-cartoon-truncated.svg" class="opacity-100 w-[100%]" v-click="1"/>

<v-clicks>

- 3 monkeys: C, E, F
- Algorithm 0: coin flip (50/50) for L and R choices
- Algorithm 1: chooses based on stored choice history (sequences of length 4)
- Algorithm 2: chooses based on stored choice and reward history (sequences of length 4) (same as mouse computer opponent)

</v-clicks>

:: right :: 

<div>
  <img v-show="$clicks === 5" src="/D_lee_block_transition_p_right_plots.png" class="w-[90%]" />
  
  <img v-show="$clicks >= 6" src="/monkey_dataset_1_choose_right.svg" class="w-[100%]" />
</div>

<div v-show="$clicks >= 5">

Data from Lee 2004 - Reinforcement learning and decision making in monkeys during a competitive game.

</div>

---
layout: side-title
color: teal 
transition: fade
---

:: title :: 

# Monkey vs mouse scientific questions 

:: content ::

<div style="transform: translateY(12vh)">

<v-clicks>

1. Can monkey behaviour also be described as different GLM-HMM states? 
2. Can we relate these states back to behavioural metrics such as P(right) and entropy?
3. Are there differences in how well mice and monkeys were doing the task?

</v-clicks>

</div>


---
transition: fade-out 
layout: top-title-two-cols
color: teal 
columns: is-6
---

:: title :: 

# Mouse and monkey behaviour can both be broadly classified into three states


:: left :: 

## Monkey

<img src="/delta_logloss_per_state_balanced_trials_per_algorithm.svg" class="opacity-100 w-[55%]" v-click="3"/>

<img src="/monkey_three_states_weight_v2.svg" class="opacity-100 w-[100%]" v-click="3"/>


:: right :: 

## Mouse

<img src="/glmhmm_CV_delta_test_ll.svg" class="opacity-100 w-[50%]" v-click="1"/>


<img src="/glmhmm_glm_weights (1).png" class="opacity-100 w-[100%]" v-click="2"/>


<div v-click="4"
     class="absolute bottom-50 left-80 w-[35%] 
            bg-teal-200/90 text-black text-lg font-semibold 
            p-4 rounded-xl shadow-xl leading-snug">
  Both mouse and monkey's behaviour can be characterised into 3 states,  
  with a common stochastic state
</div>

---
layout: top-title-two-cols
columns: is-6
color: teal 
---

:: title :: 

# GLM-HMM provides an equally good quantification of behaviour as that used in the original paper

:: left :: 

## Logistic regression 

<v-click>

$$
\log \frac{P(R)_t}{P(L)_t} = a_0 + \sum^5_{i=1} a_i M_{t-i} + \sum^5_{i=1} b_i C_{t-i}
$$

</v-click>

<v-clicks>

where:

- $a_0$ is the monkey's bias
- $M_t$ is the monkey's choice on trial $t$
- $C_t$ is the computer's choice on trial $t$ 

</v-clicks>

:: right :: 

## Q-learning model 

<v-click>

$$
\log \frac{P(R)_t}{P(L)_t} = V_t(R) - V_t(L)
$$

</v-click>

<v-click>

$$
V_{t+1} (x) = \alpha V_t(x) + \Delta_t (x)
$$

</v-click>

<v-clicks>

where: 

- $V(R)$ is the rightward choice value on trial $t$
- $\alpha$ is the learning rate

</v-clicks>

<v-click>

$$
\Delta_t(x) \begin{cases}
 \Delta_1 & \text{if chosen rewarded} \\ 
 \Delta_2 & \text{if chosen unrewarded} \\ 
 0        & \text{if not chosen}
\end{cases}
$$

</v-click>


---
transition: fade-out 
layout: top-title-two-cols
columns: is-6
color: teal 
---

:: title :: 

# GLM-HMM provides an equally good quantification of behaviour as that used in the original paper

:: content :: 

:: left :: 

<img src="/monkey_glmhmm_vs_qlearning_vs_lr.svg" class="opacity-100 w-[100%]"/>


:: right :: 

<div style="transform: translateY(5vh)">

<v-clicks>

- GLM-HMM fit to entire dataset. For LR and Q-learning, one model per algorithm.
- This comparison requires a trial-based cross-validation procedure used in Ashwood et al for comparing GLM-HMM with psytrack. 

</v-clicks>

</div>



---
transition: fade-out 
layout: top-title-two-cols
columns: is-6
color: teal
---

:: title :: 

# GLM-HMM states over sessions

:: left :: 


## Monkey


<div class="relative w-full h-[500px] mt-0" v-click="3">
  <!-- Image 1: visible on click 3 only -->
  <img
    src="/C_state_probabilities_per_session.png"
    class="opacity-100 w-[100%] absolute inset-0"
    v-click="3"
    v-click-hide="6"
  />

  <!-- Image 2: visible on click 4 only -->
  <img
    src="/E_state_probabilities_per_session.png"
    class="opacity-100 w-[100%] absolute inset-0 mt-30"
    v-click="4"
    v-click-hide="6"
  />

  <!-- Image 3: visible on click 5 only -->
  <img
    src="/F_state_probabilities_per_session.png"
    class="opacity-100 w-[100%] absolute inset-0 mt-60"
    v-click="5"
    v-click-hide="6"
  />

  <!-- Image 4: visible from click 6 onwards -->
  <img
    src="/monkey_ave_p_state_over_algorithms.png"
    class="opacity-100 w-[100%] absolute inset-0 mt-20"
    v-click="6"
  />
</div>

:: right ::


<div v-click="2">
  <img src="/monkey_three_states_weight_v2.png" class="opacity-100 w-[100%]"/>
</div>



## Mouse


<div v-click="1" class="absolute top-[70%] left-120 w-[70%] -translate-y-1/2">
  <img src="/average_pstate_smooth_cosyneabstract2025.svg" class="opacity-100 w-[50%]"/>
</div>


<div v-click="7"
     class="absolute bottom-50 left-80 w-[35%] 
            bg-teal-200/90 text-black text-lg font-semibold 
            p-4 rounded-xl shadow-xl leading-snug">
  In monkeys, the transition between states corresponds well with the 3 computer algorithms.
  In mice, there is a general increase in stochastic states over training.
</div>



---
transition: fade-out 
layout: top-title-two-cols
color: teal
columns: is-6
---

:: title :: 

# We can relate states to other behavioural measures 


:: left :: 

## Monkey 

<div v-click="1">
  <img src="/monkey_three_states_weight.png" class="opacity-100 w-[100%]"/>
</div>

<div class="relative w-full h-[150px] kde-reveal">
  <!-- Step 1 & 2: left 1/3 visible -->
  <img
    src="/monkey_kde_per_state.png"
    class="absolute inset-0 w-full h-full object-contain kde-left-third"
    v-click="[3,5]"
  />

  <!-- Step 2: right 1/3 visible (so left + right at click 8) -->
  <img
    src="/monkey_kde_per_state.png"
    class="absolute inset-0 w-full h-full object-contain kde-right-third"
    v-click="[4,5]"
  />

  <!-- Step 3: full image -->
  <img
    src="/monkey_kde_per_state.png"
    class="absolute inset-0 w-full h-full object-contain"
    v-click="5"
  />
</div>

<style>
/* Only affects this slide’s container */
.kde-reveal .slidev-vclick-hidden {
  display: none;
}

/* Left 1/3 of the image */
.kde-left-third {
  clip-path: inset(0 61% 0 0);
}

/* Right 1/3 of the image */
.kde-right-third {
  clip-path: inset(0 0 0 68.7%);
}

/* Only affects this slide’s container */
.mouse-kde-reveal .slidev-vclick-hidden {
  display: none;
}

/* Left 1/3 of the image */
.mouse-kde-left-third {
  clip-path: inset(0 69% 0 0);
}

/* Right 1/3 of the image */
.mouse-kde-right-third {
  clip-path: inset(0 0 0 56%);
}
</style>

<div v-click="4" class="absolute bottom-5 left-12 w-[45%] text-sm opacity-75">
  <hr class="border-t border-gray-600 opacity-0 mb-2" />
  
  > P(WSLS) calculated as $P(X_t = Y_{t-1})$ where <br> $X_t$ and $Y_t$ are the animal’s and opponent’s choices on trial $t$.
</div>

:: right :: 

## Mouse 

<div v-click="2">
  <img src="/glmhmm_glm_weights (1).png" class="opacity-100 w-[90%]"/>
</div>

<div class="relative w-full h-[150px] mouse-kde-reveal">
  <!-- Step 1 & 2: left 1/3 visible -->
  <img
    src="/mouse_kde_per_state.png"
    class="absolute inset-0 w-full h-full object-contain mouse-kde-left-third"
    v-click="[3,5]"
  />

  <!-- Step 2: right 1/3 visible (so left + right at click 8) -->
  <img
    src="/mouse_kde_per_state.png"
    class="absolute inset-0 w-full h-full object-contain mouse-kde-right-third"
    v-click="[4,5]"
  />

  <!-- Step 3: full image -->
  <img
    src="/mouse_kde_per_state.png"
    class="absolute inset-0 w-full h-full object-contain"
    v-click="5"
  />
</div>

<div v-click="5" class="absolute bottom-5 right-10 w-[45%] text-sm opacity-75">
  <hr class="border-t border-gray-600 opacity-0 mb-2" />
  
  > Entropy measure follows Lee 2004 by calculating animal's choices on trial $t-3$ to $t$ and opponent's choices on trial $t-3$ to $t-1$. Mutual information was calculated between choice sequence of both players on trial $t-4$ to $t-1$ and the animal's choice on trial $t$. 
</div>




---
transition: fade-out 
layout: top-title-two-cols
color: teal
columns: is-6
---

:: title :: 

# We can relate states to other behavioural measures 


:: left :: 

## Monkey 

<div v-click="2" class="flex gap-4 mt-20">
  <img src="/monkey_block_entropy_vs_p_stochastic_per_session.svg" class="opacity-100 w-[50%]"/> 
  <img src="/monkey_mutual_info_vs_p_stochastic_per_session.svg" class="opacity-100 w-[50%]"/>
</div>


:: right :: 
## Mouse 

<div v-click="1" class="flex gap-4 mt-20">
  <img src="/mouse_block_entropy_vs_p_stochastic_per_session.svg" class="opacity-100 w-[47%]"/> 
  <img src="/mouse_mutual_info_vs_p_stochastic_per_session.svg" class="opacity-100 w-[47%]"/>
</div>




<div v-click="3"
     class="absolute bottom-30 left-80 w-[35%] 
            bg-teal-200/90 text-black text-lg font-semibold 
            p-4 rounded-xl shadow-xl leading-snug">
  Overall, unsupervised clustering of left/right choices via GLM-HMM captures changes in  higher-order statistics of behaviour (entropy, mutual info, WSLS)
</div>


---
transition: fade-out 
color: teal
layout: top-title
columns: is-6
---

:: title :: 

# Are monkeys better at the task than mice?

:: content :: 

<div class="flex w-full mt-10 gap-8">
  <!-- LEFT: 2×2 grid that gets replaced in-place -->
  <div class="w-1/2 relative">
    <!-- 2×2 grid, shown until click 5 -->
    <div class="grid grid-cols-2 gap-4" v-click-hide="5">
      <img v-click="1" src="/monkey_p_stochastic_heatmap.svg" class="w-full" />
      <img v-click="2" src="/mouse_p_stochastic_heatmap.svg" class="w-full" />
      <img v-click="3" src="/mean_p_stochastic_per_trial_and_session_interpolated_monkey_v2.svg" class="w-full" />
      <img v-click="4" src="/mean_p_stochastic_per_trial_and_session_interpolated_mice_v2.svg" class="w-full" />
    </div>

  <!-- Replacement image, same position, appears on click 5 -->
  <div v-click="5" class="absolute inset-0 flex items-center justify-center">
    <img src="/mouse_monkey_inverted_U_shape_p_stochastic_v2.svg"
          class="w-full h-full object-contain" />
  </div>
</div>

  <!-- RIGHT: 2×2 grid -->
  <div class="grid grid-cols-2 gap-4 w-1/2">
    <img v-click="7" src="/mouse_and_monkey_segment_length_and_entropy.svg" class="w-full" />
    <img v-click="8" src="/mouse_and_monkey_entropy_vs_reward_rate_segment_length_300.svg" class="w-full" />
    <img v-click="9" src="/mouse_and_monkey_reward_and_entropy_as_func_of_seg_length.svg" class="w-full" />
    <!-- Optional: use v-click="9" if you want an extra step -->
    <div></div>
  </div>
</div>

<div v-click="6"
     class="absolute bottom-0 left-30 w-[35%] 
            bg-teal-200/90 text-black text-lg font-semibold 
            p-4 rounded-xl shadow-xl leading-snug">
  Overall, monkeys can sustain stochastic states better. But how about if we focus on stochastic sequences? 
</div>

<div v-click="10"
     class="absolute bottom-25 left-180 w-[28%] 
            bg-teal-200/90 text-black text-lg font-semibold 
            p-4 rounded-xl shadow-xl leading-snug">
  Higher entropy in monkeys.
  Similar reward rates
</div>

---
transition: fade-out 
color: teal
layout: top-title
columns: is-6
clicks: 2
---

:: title :: 

# Are humans better at the task than monkeys/mice?

:: content :: 


<div class="w-full flex justify-center items-center h-full">
  <Transition
    enter-active-class="transition-all duration-700 ease-out"
    leave-active-class="transition-all duration-400 ease-in"
    enter-from-class="opacity-0 scale-90"
    enter-to-class="opacity-100 scale-100"
    leave-from-class="opacity-100 scale-100"
    leave-to-class="opacity-0 scale-110"
    mode="out-in"
  >
    <img
      v-if="$clicks < 1"
      key="base"
      src="/segment_length_vs_entropy_zoomed_in.svg"
      class="h-110 object-contain"
    />
    <img
      v-else
      key="human"
      src="/segment_length_vs_entropy_zoomed_in_w_human.svg"
      class="h-110 object-contain"
    />
  </Transition>
</div>


---
layout: side-title
color: teal 
transition: fade
---

:: title :: 

# Behavioural analysis and comparison summary 

:: content ::

<div style="transform: translateY(6vh)">

<v-clicks :every="2">

<p class="text-lg font-semibold italic text-teal-600">Can monkey behaviour also be described as different GLM-HMM states?</p>
<p class="text-base text-gray-700 mb-4 ml-4">Yes: in monkeys, the three states correspond to behaviour during the 3 algorithms, and fits as well as individual logistic regression models.</p>

<p class="text-lg font-semibold italic text-teal-600">Can we relate these states back to behavioural metrics such as P(right) and entropy?</p>
<p class="text-base text-gray-700 mb-4 ml-4">Stochastic states correspond to periods of higher entropy; bias states correspond to periods with more extreme P(right) values.</p>

<p class="text-lg font-semibold italic text-teal-600">Are there differences in how well mice and monkeys were doing the task?</p>
<p class="text-base text-gray-700 ml-4">Monkeys show more sustained high-entropy periods and overall higher entropy, but reward rates during those periods in mice and monkeys are similar.</p>

</v-clicks>

</div>


---
layout: section
color: coral 
transition: fade
---

# Part II: Widefield and movement analysis




--- 
layout: top-title-two-cols
color: coral  
columns: is-6
transition: fade 
---

:: title :: 

# Widefield dataset overview + short intro to locaNMF

:: left :: 

<div class="mt-16" style="width: 70%; position: relative;">

  <div v-click="[1,2]" style="position: absolute; top: 0; left: 0; width: 100%;">
    <img src="/widefield-raw-image-example.svg" class="w-full" />
  </div>

  <div v-click="[2,6]" style="position: absolute; top: 0; left: 0; overflow: hidden; width: 75%;">
    <img src="/widefield_decoding_cartoon_v2-cropped.svg"
         style="width: 225%; max-width: none; display: block;" />
  </div>

  <div v-click="6" style="position: absolute; top: 0; left: 0; width: 75%;">
    <img src="/widefield_decoding_cartoon_v2-cropped.svg"
         style="width: 200%; max-width: none; margin-left: 0%; display: block;" />
  </div>

  <!-- spacer so the parent div has height -->
  <img src="/widefield-raw-image-example.svg" class="w-full invisible" />

</div>

<div v-click="[1,2]" class="mt-3 text-xs opacity-60">n = 7 mice (CamkII-tTA tetO-GCaMP6s)</div>

:: right :: 

<div v-click="3">

Ways to process widefield data

1. Individual pixels: uses all the available information, but computationally expensive

</div>

<v-clicks at="4">

2. Average pixel per region: easy to interpret, but can throw out information / underyling activity can span multiple regions
3. SVD: good balance of 1 and 2, but spatial components can be hard to interpret

</v-clicks>

<div v-click="6" class="mt-3">

4. **locaNMF**: similar principle to SVD, but constrain spatial components to be positive and locally distributed (easier to interpret)

<div class="mt-2 flex items-center gap-2 text-xs">
  <span style="display: inline-block; width: 3px; height: 2.2em; background: currentColor; opacity: 0.35; border-radius: 2px; flex-shrink: 0;"></span>
  <span class="italic opacity-55">Saxena et al. 2020 — Localized semi-nonnegative matrix factorization (LocaNMF) of widefield calcium imaging data</span>
</div>

</div>

--- 
layout: side-title
color: coral 
transition: fade 
---

:: title :: 

# Scientific questions

:: content :: 


<div style="transform: translateY(12vh)">

<v-clicks>


1. What are the decodable signals from widefield data and how do they vary across states?
2. Are there differences in uninstructed movement across states? 
3. What signals are encoded in widefield activity (beyond movement)?


</v-clicks>

</div>




--- 
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# Widefield decoding : a variety of signals

:: content :: 

<div class="grid grid-cols-3 grid-rows-[auto_auto] gap-x-4 gap-y-0 w-full justify-items-center content-start">

  <!-- Row 1 -->
  <img v-click="1" src="/all_state_decoding_choice.svg" class="h-60 object-contain" />
  <img v-click="2" src="/all_state_decoding_reward.svg" class="h-60 object-contain" />
  <img v-click="3" src="/all_state_decoding_prevChoice.svg" class="h-60 object-contain" />

  <!-- Row 2 -->
  <img v-click="4" src="/all_state_decoding_prevReward.svg"
       class="h-60 object-contain justify-self-end -mt-6" />

  <img v-click="5" src="/all_state_decoding_state.svg"
       class="h-60 object-contain justify-self-start -mt-6" />

</div>


<div v-click="6 "
     class="absolute bottom-30 left-150 w-[30%] 
            bg-coral-pop text-black text-lg font-semibold 
            p-4 rounded-xl shadow-xl leading-snug">
  Perhaps reward and previous reward signals will be different across states?
</div>



--- 
layout: top-title
color: coral 
transition: fade 
clicks: 4
---

:: title :: 

# Finding behavioural segments that may use reward information differently

:: content ::


<div class="w-full flex justify-center">
  <img v-if="$clicks === 0" src="/block_switch_cartoon_slide_0.svg" class="h-100" />
  <img v-else-if="$clicks === 1" src="/block_switch_cartoon_slide_1.svg" class="h-100" />
  <img v-else-if="$clicks === 2" src="/block_switch_cartoon_slide_2.svg" class="h-100" />
  <img v-else-if="$clicks === 3" src="/block_switch_cartoon_slide_3.svg" class="h-100" />
  <img v-else src="/block_switch_cartoon_slide_4.svg" class="h-100" />
</div>

--- 
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# Differences in reward decoding across states

:: content :: 


<div class="grid grid-cols-2 grid-rows-[auto_auto] gap-x-4 gap-y-0 w-full justify-items-center content-start">

  <!-- Row 1 -->
  <img v-click="1" src="/20260321-mp-decode-blockswitch_prevReward.svg" class="h-100 object-contain" />
  <img v-click="2" src="/20260321-mp-decode-blockswitch_reward.svg" class="h-100 object-contain" />

</div>



--- 
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# A reward axis predicts P(switch) in a state-dependent manner 

:: content :: 

<div class="grid grid-cols-2 gap-0 w-full h-full items-center">
  <div class="flex justify-end pr-1">
    <img
      src="/reward_axis_projection_and_p_switch_diff_states_unrewarded.svg"
      class="h-100 object-contain"
    />
  </div>

  <div class="flex justify-start pl-1">
    <img
      src="/reward_axis_projection_and_p_switch_diff_states_unrewarded_slope.svg"
      class="h-100 object-contain"
    />
  </div>
</div>


--- 
layout: top-title
color: coral 
transition: fade 
---


:: title :: 

# Movement analysis 

:: content :: 

<div
  v-click
  class="grid grid-cols-5 gap-2 w-full mt-4"
>
  <img src="/JOA-M-0008__JOA-M-0008_MatchingPennies_WF_20230824_115409_Rig370001.hf-rig-001-sidecam.20230824_115430_motion_rois.png" class="sweep-img sweep-1" />
  <img src="/JOA-M-0008__JOA-M-0008_MatchingPennies_WF_20230906_122351_Rig370001.hf-rig-001-sidecam.20230906_122412_motion_rois.png" class="sweep-img sweep-2" />
  <img src="/JOA-M-0008__JOA-M-0008_MatchingPennies_WF_20230912_092538_Rig370001.hf-rig-001-sidecam.20230912_092633_motion_rois.png" class="sweep-img sweep-3" />
  <img src="/JOA-M-0008__JOA-M-0008_MatchingPennies_WF_20230913_114648_Rig370001.hf-rig-001-sidecam.20230913_114709_motion_rois.png" class="sweep-img sweep-4" />
  <img src="/JOA-M-0008__JOA-M-0008_MatchingPennies_WF_20230915_111915_Rig370001.hf-rig-001-sidecam.20230915_111936_motion_rois.png" class="sweep-img sweep-5" />

  <img src="/JOA-M-0009__JOA-M-0009_MatchingPennies_WF_20230830_102743_Rig370001.hf-rig-001-sidecam.20230830_102805_motion_rois.png" class="sweep-img sweep-6" />
  <img src="/JOA-M-0008__JOA-M-0008_MatchingPennies_WF_20230925_131039_Rig370001.hf-rig-001-sidecam.20230925_131058_motion_rois.png" class="sweep-img sweep-7" />
  <img src="/JOA-M-0009__JOA-M-0009_MatchingPennies_WF_20230906_094521_Rig370001.hf-rig-001-sidecam.20230906_094608_motion_rois.png" class="sweep-img sweep-8" />
  <img src="/JOA-M-0009__JOA-M-0009_MatchingPennies_WF_20230913_124932_Rig370001.hf-rig-001-sidecam.20230913_124952_motion_rois.png" class="sweep-img sweep-9" />
  <img src="/JOA-M-0009__JOA-M-0009_MatchingPennies_WF_20230918_093003_Rig370001.hf-rig-001-sidecam.20230918_093043_motion_rois.png" class="sweep-img sweep-10" />
</div>

<style>
.sweep-img {
  width: 100%;
  height: auto;
  object-fit: contain;
  opacity: 0;
  transform: translateX(-18px);
}

/* When the single v-click is activated, Slidev adds .slidev-vclick-target / current / hidden
   and the images animate in with staggered delays. */
.slidev-vclick-current .sweep-img,
.slidev-vclick-prior .sweep-img {
  animation: sweep-in 0.45s ease forwards;
}

.sweep-1  { animation-delay: 0.00s !important; }
.sweep-2  { animation-delay: 0.08s !important; }
.sweep-3  { animation-delay: 0.16s !important; }
.sweep-4  { animation-delay: 0.24s !important; }
.sweep-5  { animation-delay: 0.32s !important; }
.sweep-6  { animation-delay: 0.40s !important; }
.sweep-7  { animation-delay: 0.48s !important; }
.sweep-8  { animation-delay: 0.56s !important; }
.sweep-9  { animation-delay: 0.64s !important; }
.sweep-10 { animation-delay: 0.72s !important; }

@keyframes sweep-in {
  from {
    opacity: 0;
    transform: translateX(-18px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}
</style>

--- 
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# Mice exhibit more uninstructed movements during stochastic states

:: content :: 

<div class="grid grid-cols-2 grid-rows-[auto_auto] gap-x-4 gap-y-0 w-full justify-items-center content-start">

  <!-- Row 1 -->
  <img v-click="1" src="/mp_wf_sound_aligned_motion_energy_per_state.svg" class="h-100 object-contain" />
  <img v-click="2" src="/mp_wf_lick_aligned_motion_energy_per_state.svg" class="h-100 object-contain" />

</div>




--- 
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# Widefield regression 

:: content :: 


<div class="grid grid-cols-1 gap-0 w-full h-full items-center">

  <div class="flex justify-start pl-15">
    <img
      src="/locanmf-regression-cartoon.png"
      class="h-100 object-contain"
    />
  </div>
</div>


---
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# Single variable models

:: content :: 

<div class="grid grid-cols-1 grid-rows-[auto_auto] gap-y-0 w-full content-start">

  <div class="flex justify-start pl-10">
    <img
      src="/single_variable_ev_heatmap.svg"
      class="h-40 object-contain"
    />
  </div>

  <div class="flex justify-start pl-40 -mt-8">
    <img
      src="/single_variable_ev_scatter.svg"
      class="h-85 object-contain"
    />
  </div>

</div>

---
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# Full model permutation test $\Delta$EV and weights

:: content :: 

<div class="grid grid-cols-1 grid-rows-[auto_auto] gap-y-0 w-full content-start">

  <div class="flex justify-start pl-1 mt-8">
    <img
      src="/delta_ev_map_ave_mice.svg"
      class="h-40 object-contain"
    />
  </div>

  <div class="flex justify-start pl-1 -mt-15">
    <img
      src="/mp-widefield-model022_weight_map_ave_mice.svg"
      class="h-85 object-contain"
    />
  </div>

</div>

<div v-click="2"
     class="absolute bottom-50 left-80 w-[35%] 
            text-black text-lg font-semibold 
            p-4 rounded-xl shadow-xl leading-snug"
            style="background-color: rgba(232, 105, 74, 0.9);">
  Still some state and reward X state modulation after taking account of movement, albeit weak... 
</div>


---
layout: top-title
color: coral 
transition: fade 
---

:: title :: 

# State and prev reward interaction in encoding model

:: content :: 


<div class="grid grid-cols-2 grid-rows-[auto_auto] gap-x-4 gap-y-0 w-full justify-items-center content-start">

<!-- First image -->
<img
  v-click="1"
  src="/20260321-mp-decode-blockswitch_prevReward.svg"
  class="h-100 object-contain"
/>

<!-- Second image + caption -->
<div class="relative">
  <img
    v-click="2"
    src="/mp-widefield-model026-blockswitch-include-undefined_blockswitch_stochastic_pm_X_prevReward_pm_vemap_per_subject_and_ave.svg"
    class="h-100 object-contain"
  />

  <div
    v-click="2"
    class="absolute top-20 left-1/2 -translate-x-1/2 -translate-y-full text-sm text-center"
  >
  Testing for interaction:  stochastic/blockswitch X previous reward
  </div>
</div>

</div>



---
layout: side-title
color: coral 
transition: fade
---

:: title :: 

# Widefield and movement analysis summary

:: content :: 


<div style="transform: translateY(6vh)">

<v-clicks :every="2">

<p class="text-lg font-semibold italic text-coral">What are the decodable signals from widefield data and how do they vary across states?</p>
<p class="text-base text-gray-700 mb-4 ml-4">From widefield data, we can decode choice, reward, prevous choice, previous reward, state etc.</p>

<p class="text-lg font-semibold italic text-coral">Are there differences in uninstructed movement across states? </p>
<p class="text-base text-gray-700 mb-4 ml-4">Yes, and only in the period between sound onset and first lick</p>

<p class="text-lg font-semibold italic text-coral">What signals are encoded in widefield activity (beyond movement)?</p>
<p class="text-base text-gray-700 ml-4">There is still some state and reward interaction signal, but they are weak... More work to be done to understand widefield data... </p>

</v-clicks>

</div>




---
layout: credits 
color: light 
speed: 1
loop: true
---

<div class="grid text-size-4 grid-cols-3 w-3/4 gap-y-10 auto-rows-min ml-auto mr-auto">
<div class="grid-item text-center mr-0- col-span-3">
  
</div>
<div class="grid-item text-center mr-0- col-span-3">
  <strong>Cast</strong><br> 
  <span class="font-size-3 mt-0">(In order of appearance)</span>
</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Widefield</strong></div>
<div class="grid-item col-span-2">Joanna did all the recordings&nbsp;&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Monkey MP</strong></div>
<div class="grid-item col-span-2">Dae-yeol Lee <br/> Monkeys C, E, F&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Mouse MP</strong></div>
<div class="grid-item col-span-2">Joanna&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Human MP</strong></div>
<div class="grid-item col-span-2">Julia Nicklaus&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Mice</strong></div>
<div class="grid-item col-span-2">JOA-M-0020<br/>JOA-M-0022<br/>JOA-M-0023<br/>JOA-M-0024<br/>JOA-M-0025<br/>JOA-M-0026<br/>JOA-M-0027<br/>JOA-M-0028<br/>JOA-M-0029<br/>JOA-M-0030<br/>JOA-M-0031<br/>JOA-M-0033<br/>JOA-M-0036</div>


<div class="grid-item text-right mr-4 col-span-1"><strong>Humans</strong></div>
<div class="grid-item col-span-2">Orsi <br/> Margot <br/> Chen Chen <br/> Joschua <br/> ... &nbsp;</div>

<div class="grid-item text-right mr-4 col-span-1"><strong>Supervision</strong></div>
<div class="grid-item col-span-2">Ann</div>
<div class="grid-item col-span-3 text-center mt-80px mb-auto font-size-1.5rem"><strong>The end</strong></div>
</div>

