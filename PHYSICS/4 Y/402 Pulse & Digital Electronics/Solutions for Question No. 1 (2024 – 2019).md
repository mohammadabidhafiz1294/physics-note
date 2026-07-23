
## B.Sc. (Hons) Part-IV Examination - 2024

### 1. (a) Define pulse train. What are mark and space in pulse?

#### English Answer:

- **Pulse Train:** A continuous sequence or continuous series of electrical pulses repeated at uniform or non-uniform time intervals is called a **pulse train**.
    
- **Mark and Space:**
    
    - **Mark:** The duration or time interval $T_m$ during which a pulse signal remains at its **HIGH** voltage level (logic '1' or active state) is defined as the _Mark_.
        
    - **Space:** The duration or time interval $T_s$ during which a pulse signal remains at its **LOW** voltage level (logic '0' or inactive baseline) is defined as the _Space_.
        

#### বাংলা উত্তর:

- **পালস ট্রেইন (Pulse Train):** নির্দিষ্ট বা অনির্দিষ্ট সময় পরপর ধারাবাহিকভাবে নির্গত বা সঞ্চালিত বৈদ্যুতিক পালসের সমাহারকে **পালস ট্রেইন** বলে।
    
- **মার্ক এবং স্পেস (Mark and Space):**
    
    - **মার্ক (Mark):** একটি পালস সংকেত যে সময়কাল ($T_m$) ধরে তার **উচ্চ বিভব স্তর** (HIGH voltage level / লজিক '১') বজায় রাখে, তাকে _মার্ক_ বলে।
        
    - **স্পেস (Space):** একটি পালস সংকেত যে সময়কাল ($T_s$) ধরে তার **নিম্ন বিভব স্তর** (LOW voltage level / লজিক '০') বজায় রাখে, তাকে _স্পেস_ বলে।
        

### 1. (b) Discuss the various types of waveforms, illustrating each with the necessary diagrams.

#### English Answer:

In pulse and digital electronics, electrical signals are broadly categorized into continuous (analog) waveforms and discontinuous/pulsed (digital) waveforms:

1. **Sinusoidal Waveform:** A smooth, continuous harmonic periodic wave represented by mathematical sine or cosine functions.
    
2. **Square Waveform:** A symmetrical rectangular waveform where the HIGH duration (mark) equals the LOW duration (space), i.e., $T_m = T_s$ (50% duty cycle).
    
3. **Rectangular Waveform:** An asymmetrical periodic pulse wave where the mark duration does not equal the space duration ($T_m \neq T_s$).
    
4. **Triangular Waveform:** A periodic waveform with linear rise and fall ramps of equal slope and duration.
    
5. **Sawtooth Waveform:** A wave featuring a slow linear ramp up (or down) followed by a sharp, almost instantaneous drop (or rise), widely used in time-base/sweep generators.
    

```
1. Sine Wave:            2. Square Wave:          3. Rectangular Wave:
    +V |   .--.             +V |+---+   +---+        +V |+--+    +--+
       |  /    \               ||   |   |   |           ||  |    |  |
     0 +-+------+--> t       0 +-+---+---+---+--> t   0 +-+--+----+--+--> t
    -V |/      \            -V |                        -V |
       |'------'

2. Triangular Wave:      5. Sawtooth Wave:
    +V |  /\  /\            +V | /|  /|  /|
       | /  \/  \              |/ | / | / |
     0 +-+-------+--> t      0 +--+-+--+-+--> t
    -V |                    -V |
```

#### বাংলা উত্তর:

পালস ও ডিজিটাল ইলেকট্রনিক্সে বিভিন্ন ধরনের তরঙ্গরূপ (Waveforms) ব্যবহার করা হয়:

১. **সাইনুসোইডাল তরঙ্গ (Sinusoidal Waveform):** এটি একটি মসৃণ, ধারাবাহিক পর্যায়বৃত্ত এসি তরঙ্গ যা সাইন বা কোসাইন গাণিতিক অপেক্ষক দ্বারা নির্দেশিত হয়।

২. **বর্গাকার তরঙ্গ (Square Waveform):** এটি একটি সুষম আয়তাকার তরঙ্গ যেখানে মার্ক সময় এবং স্পেস সময় সমান হয় ($T_m = T_s$), অর্থাৎ ডিউটি সাইকেল ৫০%।

৩. **আয়তাকার তরঙ্গ (Rectangular Waveform):** এটি একটি বিষম পর্যায়বৃত্ত পালস তরঙ্গ যেখানে মার্ক সময় এবং স্পেস সময় সমান নয় ($T_m \neq T_s$)।

৪. **ত্রিভুজাকার তরঙ্গ (Triangular Waveform):** এই তরঙ্গের বিভব সমান ঢাল বা হারে রৈখিকভাবে বৃদ্ধি পায় এবং হ্রাস পায়।

৫. **করাত-দাঁতী তরঙ্গ (Sawtooth Waveform):** এতে রৈখিকভাবে ধীরে ধীরে বিভব বৃদ্ধি পায় এবং পরবর্তীতে হঠাৎ করে দ্রুত হ্রাস পায়। এটি প্রধানত সুইপ সার্কিট বা টাইম-বেস জেনারেটরে ব্যবহৃত হয়।

### 1. (c) What is non-linear waveshaping? Explain the working principle of a negative biased positive clamping circuit.

#### English Answer:

- **Non-linear Waveshaping:** The process of altering the shape of a voltage/current waveform using non-linear circuit elements (such as semiconductor diodes, transistors, or Zener diodes) is called **non-linear waveshaping**. Unlike linear waveshaping, non-linear waveshaping generates new frequency harmonics.
    
- **Negative Biased Positive Clamping Circuit:**
    
    - **Function:** A positive clamper shifts the entire input signal vertically upward. When a negative DC bias voltage ($-V_B$) is added, the output waveform is shifted such that its minimum peak level is fixed at $-V_B - V_D$ (where $V_D$ is the diode forward voltage drop).
        
    
    **Circuit Schematic:**
    
    ```
            C
    vi(t) --||--+--------o vo(t)
                |
               --- Diode (D) (Anode down, Cathode up)
              \   /
               \ /
               ---
                |
               ---  Negative DC Bias (-Vb)
               ---
                |
               GND
    ```
    
    - **Working Principle:**
        
        1. **Negative Half-Cycle:** During the negative peak of the input signal ($v_i = -V_m$), the diode $D$ becomes forward-biased because the cathode voltage drops below $-V_B - V_D$. The diode acts as a closed switch, allowing capacitor $C$ to charge rapidly to a voltage:
            
            $$V_C = V_m - V_B - V_D$$
            
        2. **Positive Half-Cycle:** As the input voltage increases towards $+V_m$, the diode becomes reverse-biased (OFF state). The capacitor retains its charge $V_C$ through a large load resistance $R_L$.
            
        3. **Output Voltage Expression:** The output voltage becomes:
            
            $$v_o(t) = v_i(t) + V_C$$
            
            The minimum output voltage level (clamp level) is given by:
            
            $$v_{o,\min} = -V_m + (V_m - V_B - V_D) = -V_B - V_D$$
            

#### বাংলা উত্তর:

- **অরৈখিক তরঙ্গ-আকৃতিদান (Non-linear Waveshaping):** অরৈখিক বর্তনী উপাদান (যেমন: ডায়োড, ট্রানজিস্টর বা জেনার ডায়োড) ব্যবহার করে কোনো ইনপুট তরঙ্গের আকৃতি পরিবর্তন করার প্রক্রিয়াকে **অরৈখিক তরঙ্গ-আকৃতিদান** বলে। এতে নতুন কম্পাঙ্কের হারমোনিক্স উৎপন্ন হয়।
    
- **নেগেটিভ বায়াসযুক্ত পজিটিভ ক্ল্যাম্পিং সার্কিট:**
    
    - **কার্যনীতি:** পজিটিভ ক্ল্যাম্পার সার্কিট সম্পূর্ণ ইনপুট তরঙ্গকে উপরের দিকে (পজিটিভ দিকে) স্থানান্তরিত করে। যখন একটি নেগেটিভ ডি-সি বায়াস ($-V_B$) সংযুক্ত করা হয়, তখন আউটপুট তরঙ্গের সর্বনিম্ন মান $-V_B - V_D$ স্তরে নির্ধারিত হয়।
        
    - **ক্রিয়াকৌশল:**
        
        ১. **ঋণাত্মক অর্ধ-চক্র:** ইনপুট সংকেত যখন ঋণাত্মক পিক $-V_m$-এ পৌঁছায়, তখন ডায়োডটি ফরওয়ার্ড বায়াসড হয়। ডায়োডটি পরিবাহী হওয়ায় ক্যাপাসিটর $C$ দ্রুত চার্জ লাভ করে চার্জের বিভব হয়:
        
        $$V_C = V_m - V_B - V_D$$
        
        ২. **ধনাত্মক অর্ধ-চক্র:** ইনপুট ধনাত্মক দিকে গেলে ডায়োডটি রিভার্স বায়াসড (বন্ধ) হয়ে যায়। ক্যাপাসিটর লোড রেজিস্ট্যান্সের মধ্য দিয়ে ধীরে ডিসচার্জ হয় এবং চার্জ ধরে রাখে।
        
        ৩. **আউটপুট বিভব:** আউটপুট বিভব হয়:
        
        $$v_o(t) = v_i(t) + V_C$$
        
        ফলে আউটপুটের সর্বনিম্ন মান (ক্ল্যাম্প লেভেল) দাঁড়ায়:
        
        $$v_{o,\min} = -V_B - V_D$$
        

### 1. (d) Numerical Problem

**Given:**

- Input voltage: $v_i(t) = 12\sin(\omega t) \implies \text{Peak Voltage } V_m = 12\text{ V}$
    
- Negative bias voltage: $V_B = 4\text{ V}$ (i.e., $-V_B = -4\text{ V}$)
    
- Silicon diode voltage drop: $V_D = 0.7\text{ V}$
    

#### Calculation:

**(i) Capacitor Charging Voltage ($V_C$):**

$$V_C = V_m - V_B - V_D = 12\text{ V} - 4\text{ V} - 0.7\text{ V} = 7.3\text{ V}$$

**(ii) Clamp Level (Minimum Output Voltage, $v_{o,\min}$):**

$$v_{o,\min} = -V_B - V_D = -4\text{ V} - 0.7\text{ V} = -4.7\text{ V}$$

**(iii) Peak Output Voltage ($v_{o,\max}$):**

$$v_{o,\max} = +V_m + V_C = 12\text{ V} + 7.3\text{ V} = 19.3\text{ V}$$

#### বাংলা সমাধান:

- **(i) ক্যাপাসিটরের চার্জিং ভোল্টেজ ($V_C$):** $12 - 4 - 0.7 = 7.3\text{ V}$
    
- **(ii) ক্ল্যাম্প লেভেল / সর্বনিম্ন আউটপুট ($v_{o,\min}$):** $-4 - 0.7 = -4.7\text{ V}$
    
- **(iii) পিক বা সর্বোচ্চ আউটপুট ভোল্টেজ ($v_{o,\max}$):** $12 + 7.3 = 19.3\text{ V}$
    

## B.Sc. (Hons) Part-IV Examination - 2023

### 1. (a) Draw a non-ideal pulse waveform and describe its key pulse parameters.

#### English Answer:

A practical (non-ideal) rectangular pulse exhibits continuous transitions and parasitic transient effects rather than ideal instantaneous steps.

```
       Overshoot
        .--._______ Sag / Tilt
       /           \
      /             \
     /               \___________
    /                             \   Backswing
---'                               '---'
   |<--tr-->|      |<--tf-->|
   |<- Pulse Width (W) ->|
```

**Key Pulse Parameters:**

1. **Rise Time ($t_r$):** The time required for the pulse amplitude to rise from 10% to 90% of its maximum steady-state amplitude.
    
2. **Fall Time ($t_f$):** The time required for the pulse amplitude to fall from 90% to 10% of its steady-state value.
    
3. **Pulse Duration / Width ($W$ or $t_p$):** The time interval measured between the 50% amplitude points on the leading and trailing edges.
    
4. **Sag (Tilt):** The decay or drop in the pulse amplitude across its top flat region during the pulse duration.
    
5. **Overshoot & Backswing:** Transient spikes above the maximum flat level during the turn-on phase (Overshoot) or dropping below the baseline after the trailing edge (Backswing).
    

#### বাংলা উত্তর:

একটি বাস্তব (Non-ideal) পালস তরঙ্গের বিভিন্ন বৈশিষ্ট্যপূর্ণ প্যারামিটার নিচে বর্ণনা করা হলো:

১. **রাইজ টাইম ($t_r$):** পালসের বিস্তার ১০% থেকে ৯০%-এ উন্নীত হতে প্রয়োজনীয় সময়।

২. **ফল টাইম ($t_f$):** পালসের বিস্তার ৯০% থেকে কমে ১০%-এ নামতে প্রয়োজনীয় সময়।

৩. **পালস প্রস্থ ($W$ বা $t_p$):** অগ্রগামী ও পশ্চাৎগামী প্রান্তের ৫০% বিস্তার বিন্দুর মধ্যবর্তী সময় ব্যবধান।

৪. **স্যাগ বা টিল্ট (Sag/Tilt):** পালস স্থায়ী থাকার সময় ফ্ল্যাট শীর্ষভাগের বিভব হ্রাসের পরিমাণ।

৫. **ওভারশুট ও ব্যাকসুইং:** পালস শুরুর মুহূর্তে কাঙ্ক্ষিত সীমার অতিরিক্ত বৃদ্ধিকে ওভারশুট এবং পালস শেষে বেসলাইনের নিচে সাময়িক পতনকে ব্যাকসুইং বলে।

### 1. (b) Explain the working principle of RC low-pass circuit for a square wave input. How can the low-pass RC circuit be used as an integrator?

#### English Answer:

- **RC Low-Pass Circuit Operation:**
    
    An RC low-pass circuit consists of a series resistor $R$ and a shunt capacitor $C$ connected across the output. When a square wave is applied, the capacitor exponentially charges through $R$ during the HIGH period ($V$) and exponentially discharges during the LOW period ($0\text{ V}$).
    

```
   Vi o---[ R ]---+---o Vo
                  |
                 --- C
                 ---
                  |
                 GND
```

- **Condition for Integrator:**
    
    The loop voltage equation is:
    
    $$v_{in}(t) = v_R(t) + v_o(t) = R i(t) + v_o(t)$$
    
    If the time constant is chosen to be much larger than the pulse period ($RC \gg T$), the output voltage across the capacitor remains very small compared to the drop across the resistor ($v_o(t) \ll v_R(t)$). Thus:
    
    $$v_{in}(t) \approx R i(t) \implies i(t) \approx \frac{v_{in}(t)}{R}$$
    
    The output voltage across capacitor $C$ is:
    
    $$v_o(t) = \frac{1}{C} \int i(t) \, dt \approx \frac{1}{RC} \int v_{in}(t) \, dt$$
    
    Since $RC$ is constant, $v_o(t) \propto \int v_{in}(t) \, dt$. Hence, the low-pass RC circuit acts as a **mathematical integrator**.
    

#### বাংলা উত্তর:

- **RC লো-পাস সার্কিটের কার্যনীতি:**
    
    একটি শ্রেণি-সংযুক্ত রোধ $R$ এবং সমান্তরাল ক্যাপাসিটর $C$ সমন্বয়ে লো-পাস সার্কিট গঠিত হয়। স্কয়ার ওয়েভ ইনপুট দেওয়া হলে ইনপুটের HIGH স্তরে ক্যাপাসিটর $C$ রোধের মাধ্যমে এক্সপোনেনশিয়ালি চার্জ হয় এবং LOW স্তরে ডিসচার্জ হয়।
    
- **ইন্টিগ্রেটর হিসেবে ব্যবহার:**
    
    কার্শফের ভোল্টেজ সূত্রানুসারে: $v_{in}(t) = R i(t) + v_o(t)$
    
    যদি সার্কিটের টাইম কনস্ট্যান্ট, তরঙ্গকালের চেয়ে অনেক বড় হয় ($RC \gg T$), তবে ক্যাপাসিটরের ভোল্টেজ ড্রপ রোধের তুলনায় নগণ্য হয় ($v_o(t) \ll v_R(t)$)।
    
    অতএব: $v_{in}(t) \approx R i(t) \implies i(t) \approx \frac{v_{in}(t)}{R}$
    
    ক্যাপাসিটরের প্রান্তীয় আউটপুট বিভব:
    
    $$v_o(t) = \frac{1}{C} \int i(t) \, dt = \frac{1}{RC} \int v_{in}(t) \, dt$$
    
    যেহেতু $RC$ একটি ধ্রুবক, তাই $v_o(t) \propto \int v_{in}(t) \, dt$। অর্থাৎ আউটপুট বিভব ইনপুট বিভবের সমাকলনের (integration) সমানুপাতিক।
    

### 1. (c) Numerical Problem

**Given:**

- Pulse width $t_p = 8\ \mu\text{s}$
    
- Duty cycle $D = 40\% = 0.40$
    

#### Calculation:

1. **Period ($T$):**
    
    $$D = \frac{t_p}{T} \implies T = \frac{t_p}{D} = \frac{8\ \mu\text{s}}{0.40} = 20\ \mu\text{s}$$
    
2. **Frequency ($f$):**
    
    $$f = \frac{1}{T} = \frac{1}{20 \times 10^{-6}\text{ s}} = 50,000\text{ Hz} = 50\text{ kHz}$$
    

#### বাংলা সমাধান:

- **পর্যায়কাল ($T$):** $T = \frac{8\ \mu\text{s}}{0.40} = 20\ \mu\text{s}$
    
- **কম্পাঙ্ক ($f$):** $f = \frac{1}{20 \times 10^{-6}\text{ s}} = 50\text{ kHz}$
    

## B.Sc. (Hons) Part-IV Examination - 2022

### 1. (a) What is clamper circuit? Describe the working principle of a positive clamper circuit for $V_L$ with necessary diagrams.

#### English Answer:

- **Clamper Circuit:** A clamper is a non-linear wave-shaping circuit that adds a DC level to an AC signal, shifting the waveform above or below a reference potential without altering the original shape or peak-to-peak amplitude of the signal.
    
- **Positive Clamper Working Principle:**
    
    A positive clamper pushes the signal upward such that the lower peak of the waveform is clamped to $0\text{ V}$ (or DC reference).
    

```
          C
  vi(t) --||--+--------o vo(t)
              |      |
             --- D   [ RL ]
            / \      |
            ---      |
              |      |
             GND    GND
```

1. **Negative Half Cycle:** Diode $D$ conducts (forward biased). Capacitor $C$ rapidly charges to $V_m$ with polarity (+ right, - left). Output voltage $v_o \approx 0\text{ V}$.
    
2. **Positive Half Cycle:** Diode $D$ is reverse biased (OFF). The input voltage $v_i = +V_m$ acts in series with the capacitor voltage $V_C = V_m$.
    
3. **Total Output:**
    
    $$v_o = v_i + V_C = V_m + V_m = 2V_m$$
    
    The input range $[-V_m, +V_m]$ is shifted to $[0, 2V_m]$.
    

#### বাংলা উত্তর:

- **ক্ল্যাম্পার সার্কিট:** যে সার্কিটের মাধ্যমে এসি সংকেতের সাথে একটি ডিসি ভোল্টেজ যোগ করে তরঙ্গের মূল আকৃতি ও পিক-টু-পিক বিস্তার অপরিবর্তিত রেখে সংকেতকে সম্পূর্ণ উপরে বা নিচে স্থানান্তরিত করা হয়, তাকে **ক্ল্যাম্পার সার্কিট** বলে।
    
- **পজিটিভ ক্ল্যাম্পারের কার্যনীতি:**
    
    ১. **ঋণাত্মক অর্ধ-চক্র:** ইনপুটের ঋণাত্মক অর্ধে ডায়োড $D$ ফরওয়ার্ড বায়াসড হয়ে পরিবাহী হয়। ক্যাপাসিটর $C$ দ্রুত চার্জ লাভ করে $V_m$ ভোল্টেজে চার্জিত হয়। এই সময় আউটপুট ভোল্টেজ শূন্য থাকে।
    
    ২. **ধনাত্মক অর্ধ-চক্র:** ইনপুটের ধনাত্মক অর্ধে ডায়োড $D$ রিভার্স বায়াসড (বন্ধ) হয়। তখন ক্যাপাসিটর ভোল্টেজ $V_C$ এবং ইনপুট ভোল্টেজ $v_i$ সিরিজে যুক্ত হয়ে আউটপুটে পাওয়া যায়।
    
    ৩. **মোট আউটপুট:** $v_o = v_i + V_C = V_m + V_m = 2V_m$। অর্থাৎ তরঙ্গটি পজিটিভ অক্ষের দিকে শিফট হয়।
    

### 1. (b) Explain the working principle of an RC high-pass circuit for a square wave input. How can the high-pass RC circuit be used as a differentiator?

#### English Answer:

- **RC High-Pass Circuit:**
    
    It consists of a series capacitor $C$ and a shunt resistor $R$ across which output $v_o$ is taken.
    

```
   Vi o---||---+---o Vo
          C    |
              [ R ]
               |
              GND
```

- **Differentiator Operation:**
    
    The voltage relation is:
    
    $$v_{in}(t) = v_C(t) + v_o(t) = v_C(t) + R i(t)$$
    
    If $RC \ll T$ (time constant is extremely small relative to input period $T$), the capacitor charges instantly, so $v_C(t) \approx v_{in}(t)$.
    
    The current passing through $R$ is:
    
    $$i(t) = C \frac{d v_C(t)}{dt} \approx C \frac{d v_{in}(t)}{dt}$$
    
    Therefore, the output voltage is:
    
    $$v_o(t) = R i(t) = RC \frac{d v_{in}(t)}{dt}$$
    
    Since $RC$ is constant, $v_o(t) \propto \frac{d v_{in}(t)}{dt}$. Thus, the circuit acts as a **differentiator**.
    

#### বাংলা উত্তর:

- **RC হাই-পাস সার্কিট:** সিরিজে ক্যাপাসিটর $C$ এবং সমান্তরালে রোধ $R$ যুক্ত করে এই সার্কিট গঠন করা হয়, যেখানে রোধের দুই প্রান্ত থেকে আউটপুট নেওয়া হয়।
    
- **ডিফারেনশিয়েটর হিসেবে কাজ:**
    
    বর্তনীর সমীকরণ: $v_{in}(t) = v_C(t) + v_o(t)$
    
    যদি সময় ধ্রুবক $RC \ll T$ হয়, তবে ক্যাপাসিটরটি অত্যন্ত দ্রুত চার্জ হয় এবং $v_C(t) \approx v_{in}(t)$ লেখা যায়।
    
    ক্যাপাসিটরের মধ্য দিয়ে প্রবাহিত কারেন্ট:
    
    $$i(t) = C \frac{d v_C(t)}{dt} \approx C \frac{d v_{in}(t)}{dt}$$
    
    অতএব রোধের দুই প্রান্তের আউটপুট ভোল্টেজ:
    
    $$v_o(t) = R i(t) = RC \frac{d v_{in}(t)}{dt}$$
    
    আউটপুট ভোল্টেজ ইনপুট সংকেতের সময়-ব্যবকলনের (differentiation) সমানুপাতিক।
    

### 1. (c) Numerical / Design Problem

**Given:**

- Pulse width of square wave: $t_p = 50\text{ ms}$
    

#### Solution & Design:

For an RC high-pass circuit to function effectively as a differentiator, the circuit time constant $\tau = RC$ must be significantly smaller than the pulse width $t_p$:

$$RC \le 0.1 \times t_p$$

$$RC \le 0.1 \times 50\text{ ms} = 5\text{ ms} = 0.005\text{ s}$$

**Component Selection:**

- Let us select a standard capacitor value: $C = 1\ \mu\text{F} = 10^{-6}\text{ F}$
    
- Then the required resistor value is:
    
    $$R = \frac{\tau}{C} = \frac{5 \times 10^{-3}\text{ s}}{10^{-6}\text{ F}} = 5000\ \Omega = 5\text{ k}\Omega$$
    

#### Circuit Diagram:

```
                C = 1 uF
   In o-----------||-----------+-----------o Out
                              |
                             [ ] R = 5 kOhm
                             [ ]
                              |
                             GND
```

#### বাংলা সমাধান:

ডিফারেনশিয়েটরের জন্য সময় ধ্রুবক $RC \le 0.1 \times t_p = 5\text{ ms}$ হতে হবে।

ক্যাপাসিটর $C = 1\ \mu\text{F}$ ধরা হলে,

$R = \frac{5\text{ ms}}{1\ \mu\text{F}} = 5\text{ k}\Omega$।

## B.Sc. (Hons) Part-IV Examination - 2021

### 1. (a) Define pulse parameters with diagram.

#### English Answer:

_(Refer to diagram in 2023 1(a))_

1. **Rise time ($t_r$):** Time taken by the pulse to transition from 10% to 90% of its maximum amplitude.
    
2. **Sag (Tilt):** The fractional decrease in pulse amplitude across its top flat duration:
    
    $$\text{Sag} = \frac{V_1 - V_2}{V_1} \times 100\%$$
    
3. **Backswing:** Transient voltage drop below the initial baseline level immediately following the trailing edge.
    
4. **Settling time:** The time taken for the pulse to enter and remain within a specified amplitude error band (e.g., $\pm 2\%$).
    
5. **Duty cycle ($D$):** The ratio of pulse width $t_p$ to the total signal period $T$:
    
    $$D = \frac{t_p}{T} \times 100\%$$
    

#### বাংলা উত্তর:

১. **রাইজ টাইম ($t_r$):** পিকের ১০% থেকে ৯০% বৃদ্ধিতে অতিক্রান্ত সময়।

২. **স্যাগ (Sag/Tilt):** পালসের সর্বোচ্চ বিভব ধরে রাখার সময়কালের মধ্যে বিভব হ্রাসের শতকরা হার: $\text{Sag} = \frac{V_1 - V_2}{V_1} \times 100\%$।

৩. **ব্যাকসুইং (Backswing):** পালসের শেষ প্রান্তে বেসলাইনের নিচে অস্থায়ী পতন।

৪. **সেটলিং টাইম (Settling time):** পালস আউটপুট চূড়ান্ত স্থির মানের নির্দিষ্ট সীমার (যেমন $\pm 2\%$) মধ্যে স্থির হতে প্রয়োজনীয় সময়।

৫. **ডিউটি সাইকেল ($D$):** পর্যায়কালের তুলনায় পালস স্থায়িত্বের অনুপাত: $D = \frac{t_p}{T} \times 100\%$।

### 1. (b) Mathematical proof that $v_o(t) \propto \int v_{in}(t) \, dt$ when $RC \gg T$

#### English Answer:

Consider an RC low-pass filter with input $v_{in}(t)$ and output $v_o(t)$ across capacitor $C$.

Applying KVL:

$$v_{in}(t) = R i(t) + v_o(t)$$

Since $v_o(t) = \frac{1}{C} \int i(t) \, dt$, substituting $i(t) = C \frac{d v_o}{dt}$:

$$v_{in}(t) = RC \frac{d v_o(t)}{dt} + v_o(t)$$

When $RC \gg T$, the rate of change term $RC \frac{d v_o(t)}{dt}$ completely dominates $v_o(t)$ because the charging current is limited by the large $R$. Therefore:

$$v_{in}(t) \approx RC \frac{d v_o(t)}{dt}$$

Integrating both sides with respect to time $t$:

$$\int v_{in}(t) \, dt \approx RC \cdot v_o(t)$$

$$v_o(t) \approx \frac{1}{RC} \int v_{in}(t) \, dt$$

Hence, $v_o(t)$ is directly proportional to the time integral of the input signal.

#### বাংলা প্রমাণ:

কেভিএল (KVL) অনুযায়ী: $v_{in}(t) = R i(t) + v_o(t) = RC \frac{d v_o(t)}{dt} + v_o(t)$

যখন $RC \gg T$, তখন $RC \frac{d v_o(t)}{dt} \gg v_o(t)$ হয়।

অতএব: $v_{in}(t) \approx RC \frac{d v_o(t)}{dt}$

উভয়পক্ষকে সময়ের সাপেক্ষে সমাকলন (integration) করে পাই:

$$v_o(t) = \frac{1}{RC} \int v_{in}(t) \, dt$$

অর্থাৎ, আউটপুট ভোল্টেজ ইনপুট সংকেতের ইন্টিগ্রালের সমানুপাতিক।

### 1. (c) Numerical Problem

**Given:**

- Frequency $f = 2.3\text{ MHz} = 2.3 \times 10^6\text{ Hz}$
    
- Pulse width $t_p = 9\ \mu\text{s}$
    

#### Calculation:

1. **Period ($T$):**
    
    $$T = \frac{1}{f} = \frac{1}{2.3 \times 10^6\text{ Hz}} \approx 0.4348\ \mu\text{s} = 434.8\text{ ns}$$
    
2. **Duty Cycle ($D$):**
    
    $$D = \frac{t_p}{T} \times 100\% = \frac{9\ \mu\text{s}}{0.4348\ \mu\text{s}} \times 100\% \approx 2070\%$$
    

> **Technical Note:** Physically, pulse width $t_p$ cannot exceed period $T$ ($D \le 100\%$). The mathematical value resulting from the given parameter values is $2070\%$.

#### বাংলা সমাধান:

- **পর্যায়কাল ($T$):** $T = \frac{1}{2.3 \times 10^6} = 0.4348\ \mu\text{s}$
    
- **ডিউটি সাইকেল ($D$):** $D = \frac{9\ \mu\text{s}}{0.4348\ \mu\text{s}} \times 100\% = 2070\%$ (গাণিতিক ফলাফল)।
    

## B.Sc. (Hons) Part-IV Examination - 2020

### 1. (a) Compare linear and non-linear waveshapings.

#### English Answer:

|**Feature**|**Linear Waveshaping**|**Non-linear Waveshaping**|
|---|---|---|
|**Circuit Components**|Consists of linear elements ($R, L, C$).|Uses non-linear elements (Diodes, Transistors, Zeners).|
|**New Frequencies**|No new frequency components are generated.|Generates new harmonic frequency components.|
|**Superposition**|Obey Superposition Principle.|Violates Superposition Principle.|
|**Examples**|RC High-pass (Differentiator), Low-pass (Integrator).|Clippers, Clampers, Diode Limiters.|

#### বাংলা উত্তর:

|**বৈশিষ্ট্য**|**রৈখিক তরঙ্গ-আকৃতিদান (Linear)**|**অরৈখিক তরঙ্গ-আকৃতিদান (Non-linear)**|
|---|---|---|
|**উপাদান**|নিষ্ক্রিয় রৈখিক উপাদান ($R, L, C$) ব্যবহার হয়।|সক্রিয়/অরৈখিক উপাদান (ডায়োড, ট্রানজিস্টর) ব্যবহার হয়।|
|**নতুন কম্পাঙ্ক**|নতুন কোনো কম্পাঙ্ক উৎপন্ন হয় না।|নতুন হারমোনিক্স বা কম্পাঙ্ক তৈরি হয়।|
|**সুপারপজিশন**|সুপারপজিশন নীতি মেনে চলে।|সুপারপজিশন নীতি মেনে চলে না।|
|**উদাহরণ**|ইন্টিগ্রেটর, ডিফারেনশিয়েটর সার্কিট।|ক্লিপার, ক্ল্যাম্পার সার্কিট।|

### 1. (b) (i) Explain RC high-pass for rectangular input, (ii) How it acts as a differentiator?

#### English Answer:

_(Refer to solution 2022 1(b) for part (ii))_

For a rectangular input wave, when the pulse steps from $0$ to $V$, the capacitor acts as a short circuit initially, causing output $v_o$ to jump instantly to $V$. As the capacitor charges through $R$, $v_o$ decays exponentially toward $0$. When input steps back to $0$, $v_o$ drops sharply to $-V$ and then decays exponentially back to $0$.

#### বাংলা উত্তর:

ইনপুট বিভব হঠাৎ বৃদ্ধি পেলে ক্যাপাসিটর শুরুতে শর্ট সার্কিট হিসেবে কাজ করায় আউটপুট একলাফে পিকের সমপরিমাণে উন্নীত হয় এবং ক্যাপাসিটর চার্জ হওয়ার সাথে সাথে এক্সপোনেনশিয়ালি কমে শূন্যের দিকে যায়।

### 1. (c) Discuss zero-level positive peak clamping.

#### English Answer:

A **Zero-Level Positive Peak Clamper** fixes the maximum positive peak of the output waveform at $0\text{ V}$ baseline (shifting the entire wave downward into the negative voltage region).

```
          C
  vi(t) --||--+--------o vo(t)
              |
             --- Diode (Anode up, Cathode down)
            / \
            ---
              |
             GND
```

When input $v_i$ goes positive, the diode conducts, charging capacitor $C$ to peak $V_m$ with positive on the left. The output is held at $0\text{ V}$ during positive peaks and swings down to $-2V_m$ during negative peaks.

#### বাংলা উত্তর:

এই সার্কিটটি ইনপুট সংকেতকে এমনভাবে নেগেটিভ অক্ষের দিকে ঠেলে দেয় যাতে সংকেতের ধনাত্মক পিক $0\text{ V}$ লেভেলে ক্ল্যাম্পড (আবদ্ধ) থাকে। ডায়োডের অ্যানোডকে আউটপুট ও ক্যাথোডকে গ্রাউন্ডে সংযুক্ত করে এটি তৈরি করা হয়।

## B.Sc. (Hons) Part-IV Examination - 2019

### 1. (a) Define pulse parameters: (i) Rise time, (ii) Sag, (iii) Backswing, (iv) Duration.

_(Refer to detailed answers in 2023 1(a) and 2021 1(a))_

### 1. (b) RC low-pass integrating circuit and mathematical proof.

_(Refer to detailed derivation in 2021 1(b))_

### 1. (c) Show how positive peaks can be clipped using a shunt-diode clipper circuit.

#### English Answer:

A **Shunt-Diode Positive Peak Clipper** removes or clips off the portion of the input signal that lies above a specified positive threshold (or above zero).

```
           R
  vi(t) --[ ]--+--------o vo(t)
               |
              --- Diode (D)
             / \  (Anode up, Cathode down)
             ---
              |
             ---  Reference Voltage (+Vref)
             ---
              |
             GND
```

- **Working Principle:**
    
    1. **When $v_i < V_{ref} + V_D$:** The diode remains reverse biased (OFF). No current flows through resistor $R$, so output follows input: $v_o(t) = v_i(t)$.
        
    2. **When $v_i \ge V_{ref} + V_D$:** The diode turns ON (forward biased), acting as a low-resistance path. The output voltage is clipped at:
        
        $$v_o = V_{ref} + V_D$$
        
        All positive peaks above this potential are flattened/clipped off.
        

#### বাংলা উত্তর:

একটি **শান্ট-ডায়োড পজিটিভ পিক ক্লিপার** সার্কিট নির্দিষ্ট ধনাত্মক বিভবের উপরের অংশ কেটে বাদ দেয়।

- **কার্যনীতি:**
    
    ১. যখন ইনপুট বিভব $v_i < V_{ref} + V_D$ থাকে, তখন ডায়োডটি বন্ধ (Reverse biased) থাকে। ফলে আউটপুটে সম্পূর্ণ ইনপুট সংকেত পাওয়া যায় ($v_o = v_i$)।
    
    ২. যখন ইনপুট বিভব $v_i \ge V_{ref} + V_D$ হয়, তখন ডায়োডটি চালু (Forward biased) হয়ে পরিবাহী হয়। ফলে আউটপুট বিভব $V_{ref} + V_D$ মানে স্থির হয়ে যায় এবং এর উপরের অংশ ক্লিপড (কাটা) হয়ে যায়।