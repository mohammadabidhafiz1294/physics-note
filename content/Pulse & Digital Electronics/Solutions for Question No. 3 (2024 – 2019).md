## B.Sc. (Hons) Part-IV Examination - 2024

### 3. (a) What do you mean by operational amplifier? Mention its application.

#### English Answer:

**Operational Amplifier (Op-Amp):** An operational amplifier is a direct-coupled, high-gain, multi-stage voltage amplifier with a differential input and typically a single-ended output. Originally designed to perform mathematical operations (like addition, subtraction, integration, differentiation) in analog computers, modern IC op-amps are versatile building blocks for both linear and non-linear analog circuits.

**Applications:**

1. Mathematical operations (Adder, Subtractor, Integrator, Differentiator).
    
2. Amplification (Inverting, Non-inverting, Instrumentation amplifiers).
    
3. Signal conditioning (Active filters, Oscillators, Waveform generators).
    
4. Voltage comparators and Schmitt triggers.
    
5. Analog-to-Digital and Digital-to-Analog converters.
    

#### বাংলা উত্তর:

**অপারেশনাল এমপ্লিফায়ার (Op-Amp):** অপারেশনাল এমপ্লিফায়ার হলো একটি ডিরেক্ট-কাপলড, উচ্চ-গেইন বিশিষ্ট, মাল্টি-স্টেজ ভোল্টেজ এমপ্লিফায়ার, যার দুটি ইনপুট (ডিফারেনশিয়াল) এবং একটি আউটপুট থাকে। এনালগ কম্পিউটারে গাণিতিক কাজ (যেমন যোগ, বিয়োগ, সমাকলন, ব্যবকলন) করার জন্য প্রাথমিকভাবে এটি ডিজাইন করা হলেও, বর্তমানে এটি লিনিয়ার ও নন-লিনিয়ার সিগন্যাল প্রসেসিংয়ে ব্যাপকভাবে ব্যবহৃত হয়।

**ব্যবহারসমূহ:**

১. গাণিতিক কাজে (অ্যাডার, সাবট্রাক্টর, ইন্টিগ্রেটর, ডিফারেনশিয়েটর সার্কিট)।

২. এমপ্লিফিকেশনে (ইনভার্টিং এবং নন-ইনভার্টিং এমপ্লিফায়ার)।

৩. সিগন্যাল কন্ডিশনিংয়ে (অ্যাকটিভ ফিল্টার, অসিলেটর, ওয়েভফর্ম জেনারেটর)।

৪. ভোল্টেজ কম্পারেটর এবং শ্মিট ট্রিগার হিসেবে।

৫. A/D এবং D/A কনভার্টারে।

### 3. (b) Derive an expression for closed-loop voltage gain of a non-inverting op-amplifier.

#### Circuit Diagram:

Plaintext

```
           +Vcc
             |
             +----+
 Vin o-------| +  |
             |    |----o Vout
         +---| -  |
         |   +----+
         |     |
         +-[Rf]+
         |     -Vcc
       [R1]
         |
        GND
```

#### English Answer:

In a non-inverting amplifier, the input signal $V_{in}$ is applied to the non-inverting terminal (+), while the feedback is given to the inverting terminal (-) through a voltage divider network made of $R_1$ and $R_f$.

**Derivation:**

1. According to the **virtual short** concept of an ideal op-amp, the voltage at the inverting terminal ($V_-$) is almost equal to the voltage at the non-inverting terminal ($V_+$).
    
    $$V_- = V_+ = V_{in}$$
    
2. Since the input impedance of an ideal op-amp is infinite, no current flows into the inverting terminal. Therefore, the current flowing through $R_f$ is the same as the current flowing through $R_1$. Let this current be $I$.
    
3. Using Ohm's law:
    
    Current through $R_1$: $I = \frac{V_- - 0}{R_1} = \frac{V_{in}}{R_1}$
    
    Current through $R_f$: $I = \frac{V_{out} - V_-}{R_f} = \frac{V_{out} - V_{in}}{R_f}$
    
4. Equating the two currents:
    
    $$\frac{V_{in}}{R_1} = \frac{V_{out} - V_{in}}{R_f}$$
    
    $$\frac{R_f}{R_1} V_{in} = V_{out} - V_{in}$$
    
    $$V_{out} = V_{in} \left( 1 + \frac{R_f}{R_1} \right)$$
    
5. The closed-loop voltage gain ($A_v$) is:
    
    $$A_v = \frac{V_{out}}{V_{in}} = 1 + \frac{R_f}{R_1}$$
    

#### বাংলা উত্তর:

নন-ইনভার্টিং এমপ্লিফায়ারে ইনপুট সিগন্যাল $V_{in}$ নন-ইনভার্টিং টার্মিনালে (+) যুক্ত থাকে এবং ফিডব্যাক $R_1$ ও $R_f$ এর মাধ্যমে ইনভার্টিং টার্মিনালে (-) দেওয়া হয়।

**প্রমাণ:**

১. একটি আদর্শ অপ-এম্পের **ভার্চুয়াল শর্ট** নীতির কারণে, ইনভার্টিং টার্মিনালের ভোল্টেজ ($V_-$) এবং নন-ইনভার্টিং টার্মিনালের ভোল্টেজ ($V_+$) সমান হয়।

$$V_- = V_+ = V_{in}$$

২. আদর্শ অপ-এম্পের অভ্যন্তরীণ রোধ অসীম হওয়ায় এর ইনপুট টার্মিনাল দিয়ে কোনো কারেন্ট প্রবেশ করে না। তাই $R_f$ এবং $R_1$ এর মধ্য দিয়ে একই কারেন্ট ($I$) প্রবাহিত হয়।

৩. ওহমের সূত্রানুসারে:

$R_1$ এর মধ্য দিয়ে কারেন্ট: $I = \frac{V_- - 0}{R_1} = \frac{V_{in}}{R_1}$

$R_f$ এর মধ্য দিয়ে কারেন্ট: $I = \frac{V_{out} - V_-}{R_f} = \frac{V_{out} - V_{in}}{R_f}$

৪. কারেন্ট দুটি সমান ধরে পাই:

$$\frac{V_{in}}{R_1} = \frac{V_{out} - V_{in}}{R_f}$$

$$\frac{R_f}{R_1} V_{in} = V_{out} - V_{in}$$

$$V_{out} = V_{in} \left( 1 + \frac{R_f}{R_1} \right)$$

৫. অতএব, ক্লোজড-লুপ ভোল্টেজ গেইন ($A_v$) হলো:

$$A_v = \frac{V_{out}}{V_{in}} = 1 + \frac{R_f}{R_1}$$

### 3. (c) Describe in brief, the different steps in fabricating monolithic IC.

#### English Answer:

The fabrication of a monolithic Integrated Circuit (IC) involves a series of complex photo-chemical processes on a single silicon chip. The primary steps are:

1. **Wafer Preparation:** A pure silicon cylindrical crystal is grown, doped (usually p-type), and then sliced into thin wafers. The wafers are polished to a mirror finish.
    
2. **Epitaxial Growth:** A thin n-type silicon layer is grown on the p-type substrate. This layer will house the active and passive components.
    
3. **Oxidation:** A layer of Silicon Dioxide ($SiO_2$) is grown over the entire wafer surface to act as a protective and insulating mask.
    
4. **Photolithography:** A photoresist material is applied, exposed to ultraviolet light through a patterned mask, and chemically etched. This creates specific "windows" in the $SiO_2$ layer where impurities will be added.
    
5. **Diffusion or Ion Implantation:** Dopant impurities (p-type or n-type) are introduced into the exposed silicon windows at high temperatures to form the required components (transistors, diodes, resistors). Steps 3, 4, and 5 are repeated several times.
    
6. **Metallization:** A thin layer of aluminum is deposited over the wafer and etched to form the necessary electrical interconnections between the components.
    
7. **Testing and Packaging:** The wafer is scored and broken into individual chips (dies). Good chips are attached to a header, wire-bonded to pins, and sealed in plastic or ceramic packages.
    

#### বাংলা উত্তর:

একটি মনোলিথিক আইসি (IC) তৈরির প্রধান ধাপগুলো নিচে সংক্ষেপে আলোচনা করা হলো:

১. **ওয়েফার প্রস্তুতি (Wafer Preparation):** বিশুদ্ধ সিলিকন ক্রিস্টাল তৈরি করে এবং তাতে p-টাইপ ডোপিং করে সরু ও পাতলা চাকতি বা ওয়েফারে কাটা হয়। এরপর একে মসৃণ করা হয়।

২. **এপিট্যাক্সিয়াল বৃদ্ধি (Epitaxial Growth):** সাবস্ট্রেটের ওপর একটি পাতলা n-টাইপ সিলিকন স্তর তৈরি করা হয়। এই স্তরেই সার্কিটের সকল উপাদান তৈরি হবে।

৩. **অক্সিডেশন (Oxidation):** পুরো ওয়েফারের ওপর সিলিকন ডাই-অক্সাইডের ($SiO_2$) একটি আস্তরণ তৈরি করা হয়, যা অন্তরক ও সুরক্ষাকবচ হিসেবে কাজ করে।

৪. **ফটোলিথোগ্রাফি (Photolithography):** এর সাহায্যে $SiO_2$ স্তরের নির্দিষ্ট স্থানে রাসায়নিক প্রক্রিয়ায় ক্ষুদ্র জানালা বা উইন্ডো তৈরি করা হয়, যার ভেতর দিয়ে ডোপিং করা হবে।

৫. **ডিফিউশন (Diffusion):** উইন্ডোগুলোর ভেতর দিয়ে উচ্চ তাপমাত্রায় নির্দিষ্ট ভেজাল (p-টাইপ বা n-টাইপ) প্রবেশ করিয়ে ট্রানজিস্টর, ডায়োড, রোধ ইত্যাদি তৈরি করা হয়।

৬. **মেটালাইজেশন (Metallization):** উপাদানগুলোর মধ্যে বৈদ্যুতিক সংযোগ স্থাপনের জন্য পুরো চিপের ওপর অ্যালুমিনিয়ামের প্রলেপ দেওয়া হয় এবং অপ্রয়োজনীয় অংশ মুছে ফেলা হয়।

৭. **প্যাকেজিং (Testing and Packaging):** ওয়েফার কেটে আলাদা চিপ তৈরি করে পরীক্ষা করা হয় এবং পিনের সাথে যুক্ত করে প্লাস্টিক বা সিরামিকের প্যাকেজে আবদ্ধ করা হয়।

## B.Sc. (Hons) Part-IV Examination - 2023

### 3. (a) What are the different functional stages of an Op-Amp? Explain their functions.

#### Block Diagram:

Plaintext

```
  Inputs
  v1 o-->[ Input Stage  ]-->[ Intermediate ]-->[ Level Shifting ]-->[ Output Stage ]--> o v_out
  v2 o-->[  (Diff Amp)  ]-->[    Stage     ]-->[     Stage      ]-->[              ]
```

#### English Answer:

A typical operational amplifier consists of four main functional stages:

1. **Input Stage (Dual-Input, Balanced-Output Differential Amplifier):** This stage provides the inverting and non-inverting inputs. It amplifies the difference between the two input signals. It determines most of the op-amp's essential characteristics, such as high input impedance, high Common-Mode Rejection Ratio (CMRR), and initial voltage gain.
    
2. **Intermediate Stage (Dual-Input, Unbalanced-Output Differential Amplifier):** It takes the balanced output from the first stage and converts it to a single-ended (unbalanced) output. Its primary function is to provide additional voltage gain.
    
3. **Level Shifting Stage (Emitter Follower):** Due to direct coupling, the DC voltage level at the output of the intermediate stage is usually well above zero volts. The level shifter (typically an emitter follower with a constant current source) shifts this DC level down to zero volts with respect to ground, so that a zero input produces a zero output.
    
4. **Output Stage (Push-Pull Amplifier):** This is a complementary symmetry push-pull amplifier. It increases the current supplying capability (current gain) of the op-amp, provides a low output impedance, and allows the op-amp to deliver maximum output voltage swings.
    

#### বাংলা উত্তর:

একটি সাধারণ অপারেশনাল এমপ্লিফায়ার প্রধানত চারটি কার্যকর ধাপে (stages) বিভক্ত:

১. **ইনপুট স্টেজ (Input Stage):** এটি একটি ডুয়াল-ইনপুট, ব্যালেন্সড-আউটপুট ডিফারেনশিয়াল এমপ্লিফায়ার। এটি দুটি ইনপুট সিগন্যালের পার্থক্যকে বিবর্ধিত করে। অপ-এম্পের উচ্চ ইনপুট ইম্পিডেন্স, উচ্চ CMRR এবং প্রাথমিক ভোল্টেজ গেইন এই স্টেজের মাধ্যমেই নির্ধারিত হয়।

২. **ইন্টারমিডিয়েট স্টেজ (Intermediate Stage):** এটি প্রথম স্টেজের ব্যালেন্সড আউটপুট গ্রহণ করে এবং তাকে সিঙ্গেল-এন্ডেড (unbalanced) আউটপুটে রূপান্তর করে। এর মূল কাজ হলো সিগন্যালের ভোল্টেজ গেইন আরও বৃদ্ধি করা।

৩. **লেভেল শিফটিং স্টেজ (Level Shifting Stage):** ডিরেক্ট-কাপলিং এর কারণে ইন্টারমিডিয়েট স্টেজের আউটপুটে কিছু অনাকাঙ্ক্ষিত ডিসি (DC) ভোল্টেজ থেকে যায়। লেভেল শিফটার এই ডিসি লেভেলকে কমিয়ে শূন্য ভোল্টে নামিয়ে আনে, যাতে ইনপুট শূন্য হলে আউটপুটও শূন্য হয়।

৪. **আউটপুট স্টেজ (Output Stage):** এটি মূলত একটি পুশ-পুল এমপ্লিফায়ার। এটি অপ-এম্পের কারেন্ট গেইন বৃদ্ধি করে, আউটপুট ইম্পিডেন্স কমায় এবং লোডে প্রয়োজনীয় আউটপুট ভোল্টেজ সুইং সরবরাহ করে।

### 3. (b) Derive the closed-loop voltage gain of an inverting Op-Amp configuration.

#### Circuit Diagram:

Plaintext

```
           +Vcc
             |
             +----+
 GND o-------| +  |
             |    |----+----o Vout
 Vin o--[R1]-| -  |    |
         |   +----+    |
         |     |       |
         +---[Rf]------+
               -Vcc
```

#### English Answer:

In an inverting amplifier, the non-inverting terminal (+) is grounded, and the input signal $V_{in}$ is applied to the inverting terminal (-) through a resistor $R_1$. Feedback is provided through $R_f$.

**Derivation:**

1. Because the non-inverting terminal is grounded ($V_+ = 0\text{ V}$), the **virtual ground** concept forces the inverting terminal to also be at zero potential:
    
    $$V_- = V_+ = 0\text{ V}$$
    
2. The current flowing through the input resistor $R_1$ is:
    
    $$I_{in} = \frac{V_{in} - V_-}{R_1} = \frac{V_{in} - 0}{R_1} = \frac{V_{in}}{R_1}$$
    
3. Because the ideal op-amp has infinite input impedance, no current enters the inverting terminal. Therefore, all the input current $I_{in}$ must flow through the feedback resistor $R_f$.
    
    Current through $R_f$: $I_f = I_{in}$
    
4. The current $I_f$ can be written using Ohm's law across $R_f$:
    
    $$I_f = \frac{V_- - V_{out}}{R_f} = \frac{0 - V_{out}}{R_f} = -\frac{V_{out}}{R_f}$$
    
5. Equating $I_{in}$ and $I_f$:
    
    $$\frac{V_{in}}{R_1} = -\frac{V_{out}}{R_f}$$
    
    $$V_{out} = -\frac{R_f}{R_1} V_{in}$$
    
6. The closed-loop voltage gain ($A_v$) is:
    
    $$A_v = \frac{V_{out}}{V_{in}} = -\frac{R_f}{R_1}$$
    
    _(The negative sign indicates a 180° phase shift between input and output)._
    

#### বাংলা উত্তর:

ইনভার্টিং এমপ্লিফায়ারে নন-ইনভার্টিং টার্মিনাল (+) গ্রাউন্ডেড থাকে এবং ইনপুট সিগন্যাল $V_{in}$ রোধ $R_1$ এর মাধ্যমে ইনভার্টিং টার্মিনালে (-) প্রয়োগ করা হয়।

**প্রমাণ:**

১. যেহেতু নন-ইনভার্টিং টার্মিনাল গ্রাউন্ডেড ($V_+ = 0\text{ V}$), তাই **ভার্চুয়াল গ্রাউন্ড** নীতির কারণে ইনভার্টিং টার্মিনালের ভোল্টেজও শূন্য হয়:

$$V_- = V_+ = 0\text{ V}$$

২. ইনপুট রোধ $R_1$ এর মধ্য দিয়ে প্রবাহিত কারেন্ট:

$$I_{in} = \frac{V_{in} - V_-}{R_1} = \frac{V_{in} - 0}{R_1} = \frac{V_{in}}{R_1}$$

৩. আদর্শ অপ-এম্পের ইনপুট রোধ অসীম হওয়ায় এর ভেতরে কোনো কারেন্ট প্রবেশ করে না। তাই সম্পূর্ণ ইনপুট কারেন্ট ফিডব্যাক রোধ $R_f$ এর মধ্য দিয়ে প্রবাহিত হয় ($I_f = I_{in}$)।

৪. $R_f$ এর আড়াআড়ি ভোল্টেজ ড্রপ থেকে পাই:

$$I_f = \frac{V_- - V_{out}}{R_f} = \frac{0 - V_{out}}{R_f} = -\frac{V_{out}}{R_f}$$

৫. $I_{in}$ এবং $I_f$ সমান করে পাই:

$$\frac{V_{in}}{R_1} = -\frac{V_{out}}{R_f}$$

$$V_{out} = -\frac{R_f}{R_1} V_{in}$$

৬. অতএব, ক্লোজড-লুপ গেইন ($A_v$) হলো:

$$A_v = \frac{V_{out}}{V_{in}} = -\frac{R_f}{R_1}$$

_(ঋণাত্মক চিহ্ন নির্দেশ করে আউটপুট সিগন্যাল ইনপুটের সাপেক্ষে ১৮০° ফেজ শিফটে আছে)।_

### 3. (c) How does an Op-Amp function as a differentiator circuit?

#### Circuit Diagram:

Plaintext

```
           +Vcc
             |
             +----+
 GND o-------| +  |
             |    |----+----o Vout
 Vin o--||---| -  |    |
        C    +----+    |
         |     |       |
         +---[Rf]------+
               -Vcc
```

#### English Answer:

A differentiator circuit produces an output voltage that is directly proportional to the rate of change (derivative) of the input voltage with respect to time. It is constructed by placing a capacitor ($C$) at the input and a resistor ($R_f$) in the feedback loop.

**Working Principle:**

1. The non-inverting terminal is grounded. Due to virtual ground, the inverting terminal is also at $0\text{ V}$.
    
2. The current through the input capacitor is given by:
    
    $$i_c = C \frac{d(V_{in} - 0)}{dt} = C \frac{dV_{in}}{dt}$$
    
3. Since no current enters the op-amp, $i_c$ flows entirely through $R_f$.
    
    Current through $R_f$: $i_f = \frac{0 - V_{out}}{R_f} = -\frac{V_{out}}{R_f}$
    
4. Equating $i_c$ and $i_f$:
    
    $$C \frac{dV_{in}}{dt} = -\frac{V_{out}}{R_f}$$
    
    $$V_{out} = -R_f C \frac{dV_{in}}{dt}$$
    
    Thus, the output voltage is proportional to the time derivative of the input signal.
    

#### বাংলা উত্তর:

ডিফারেনশিয়েটর এমন একটি সার্কিট যার আউটপুট ভোল্টেজ ইনপুট ভোল্টেজের সময়ের সাপেক্ষে পরিবর্তনের হারের (ব্যবকলনের) সমানুপাতিক। ইনপুটে একটি ক্যাপাসিটর ($C$) এবং ফিডব্যাকে একটি রেজিস্টর ($R_f$) যুক্ত করে এটি তৈরি করা হয়।

**কার্যনীতি:**

১. নন-ইনভার্টিং টার্মিনাল গ্রাউন্ড থাকায়, ভার্চুয়াল গ্রাউন্ড নীতির কারণে ইনভার্টিং টার্মিনালও $0\text{ V}$ এ থাকে।

২. ইনপুট ক্যাপাসিটরের মধ্য দিয়ে প্রবাহিত কারেন্ট:

$$i_c = C \frac{d(V_{in} - 0)}{dt} = C \frac{dV_{in}}{dt}$$

৩. অপ-এম্পের ভেতরে কোনো কারেন্ট না যাওয়ায়, সম্পূর্ণ $i_c$ কারেন্ট $R_f$ এর মধ্য দিয়ে যায়।

$R_f$ এর কারেন্ট: $i_f = \frac{0 - V_{out}}{R_f} = -\frac{V_{out}}{R_f}$

৪. $i_c$ এবং $i_f$ সমান করে পাই:

$$C \frac{dV_{in}}{dt} = -\frac{V_{out}}{R_f}$$

$$V_{out} = -R_f C \frac{dV_{in}}{dt}$$

অর্থাৎ, আউটপুট ভোল্টেজ ইনপুটের ডিফারেনশিয়েশন বা ব্যবকলনের সমানুপাতিক।

### 3. (d) If $R = 10\ \text{k}\Omega$, $C = 0.1\ \mu\text{F}$, and the input signal is $V_{in} = 10\ \sin(1000t)$, find the output voltage expression.

#### English Answer:

**Given Data:**

- Resistance: $R = 10\text{ k}\Omega = 10 \times 10^3\ \Omega$
    
- Capacitance: $C = 0.1\ \mu\text{F} = 0.1 \times 10^{-6}\text{ F}$
    
- Input Voltage: $V_{in} = 10\sin(1000t)$
    

**Calculation:**

From the differentiator equation, $V_{out} = -RC \frac{dV_{in}}{dt}$.

First, calculate the time constant $RC$:

$$RC = (10 \times 10^3) \times (0.1 \times 10^{-6}) = 10^4 \times 10^{-7} = 10^{-3}\text{ seconds}$$

Now, differentiate the input signal with respect to time:

$$\frac{dV_{in}}{dt} = \frac{d}{dt}(10\sin(1000t)) = 10 \times 1000 \cos(1000t) = 10000 \cos(1000t)$$

Substitute the values into the output equation:

$$V_{out} = -(10^{-3}) \times 10000 \cos(1000t)$$

$$V_{out} = -10 \cos(1000t)\text{ V}$$

#### বাংলা উত্তর:

**দেওয়া আছে:**

- রোধ: $R = 10\text{ k}\Omega = 10 \times 10^3\ \Omega$
    
- ধারকত্ব: $C = 0.1\ \mu\text{F} = 0.1 \times 10^{-6}\text{ F}$
    
- ইনপুট ভোল্টেজ: $V_{in} = 10\sin(1000t)$
    

**গণনা:**

আমরা জানি, ডিফারেনশিয়েটরের আউটপুট $V_{out} = -RC \frac{dV_{in}}{dt}$।

প্রথমে সময় ধ্রুবক $RC$ বের করি:

$$RC = 10 \times 10^3 \times 0.1 \times 10^{-6} = 10^{-3}\text{ s}$$

এবার ইনপুটের ব্যবকলন বা ডিফারেনশিয়েশন করি:

$$\frac{dV_{in}}{dt} = \frac{d}{dt}(10\sin(1000t)) = 10 \times 1000 \cos(1000t) = 10000 \cos(1000t)$$

মানগুলো আউটপুটের সমীকরণে বসিয়ে পাই:

$$V_{out} = -(10^{-3}) \times 10000 \cos(1000t)$$

$$V_{out} = -10 \cos(1000t)\text{ V}$$

## B.Sc. (Hons) Part-IV Examination - 2022

### 3. (a) Describe in brief the different steps in fabricating monolithic IC.

_(This question is identical to **2024 Question 3(c)**. Please refer to that section for the detailed English and Bengali answer)._

### 3. (b) Derive an expression for the closed loop voltage gain of an inverting op-amp.

_(This question is identical to **2023 Question 3(b)**. Please refer to that section for the detailed English and Bengali answer, including the circuit diagram)._

### 3. (c) The input voltage of an op-amp is 0.5 V, input resistance is 47 k$\Omega$, and feedback resistance is 182 k$\Omega$. Calculate the output voltage in the inverting and non-inverting modes.

#### English Answer:

**Given Data:**

- Input Voltage ($V_{in}$) = $0.5\text{ V}$
    
- Input Resistance ($R_1$) = $47\text{ k}\Omega$
    
- Feedback Resistance ($R_f$) = $182\text{ k}\Omega$
    

**1. Inverting Mode:**

The output voltage formula is: $V_{out} = -\left( \frac{R_f}{R_1} \right) V_{in}$

$$V_{out} = -\left( \frac{182\text{ k}\Omega}{47\text{ k}\Omega} \right) \times 0.5\text{ V}$$

$$V_{out} \approx -3.872 \times 0.5\text{ V} \approx -1.936\text{ V}$$

**2. Non-Inverting Mode:**

The output voltage formula is: $V_{out} = \left( 1 + \frac{R_f}{R_1} \right) V_{in}$

$$V_{out} = \left( 1 + \frac{182\text{ k}\Omega}{47\text{ k}\Omega} \right) \times 0.5\text{ V}$$

$$V_{out} = \left( \frac{47 + 182}{47} \right) \times 0.5\text{ V} = \left( \frac{229}{47} \right) \times 0.5\text{ V}$$

$$V_{out} \approx 4.872 \times 0.5\text{ V} \approx 2.436\text{ V}$$

#### বাংলা উত্তর:

**দেওয়া আছে:** $V_{in} = 0.5\text{ V}$, $R_1 = 47\text{ k}\Omega$, $R_f = 182\text{ k}\Omega$।

**১. ইনভার্টিং মোডে আউটপুট:**

$$V_{out} = -\frac{R_f}{R_1} V_{in} = -\frac{182}{47} \times 0.5 \approx -1.936\text{ V}$$

**২. নন-ইনভার্টিং মোডে আউটপুট:**

$$V_{out} = \left( 1 + \frac{R_f}{R_1} \right) V_{in} = \left( 1 + \frac{182}{47} \right) \times 0.5 = \left( \frac{229}{47} \right) \times 0.5 \approx 2.436\text{ V}$$

## B.Sc. (Hons) Part-IV Examination - 2021

### 3. (a) What is an IC? Classify the ICs according to the number of components on the chip.

#### English Answer:

**Integrated Circuit (IC):** An Integrated Circuit is a complete, miniaturized electronic circuit (containing active devices like transistors/diodes and passive devices like resistors/capacitors) completely fabricated on a single piece of semiconductor material (usually silicon), known as a chip.

**Classification according to Integration Scale:**

1. **Small Scale Integration (SSI):** Contains fewer than 10 to 12 logic gates (or up to 100 electronic components) per chip.
    
2. **Medium Scale Integration (MSI):** Contains between 10 and 100 logic gates (or 100 to 1,000 components) per chip. Examples: Multiplexers, decoders.
    
3. **Large Scale Integration (LSI):** Contains between 100 and 10,000 logic gates (or 1,000 to 100,000 components) per chip. Examples: Early microprocessors, memory chips.
    
4. **Very Large Scale Integration (VLSI):** Contains between 10,000 and 1,000,000 logic gates (or 100,000 to 1 million components) per chip. Examples: Modern microprocessors, large memory arrays.
    
5. **Ultra Large Scale Integration (ULSI):** Contains more than 1 million logic gates (or >1 million components) per chip. Examples: Advanced computer CPUs, GPUs.
    

#### বাংলা উত্তর:

**ইন্টিগ্রেটেড সার্কিট (IC):** ইন্টিগ্রেটেড সার্কিট বা আইসি হলো একটি সম্পূর্ণ ও ক্ষুদ্র ইলেকট্রনিক বর্তনী, যেখানে সকল সক্রিয় (ট্রানজিস্টর, ডায়োড) এবং নিষ্ক্রিয় (রোধ, ধারক) উপাদানগুলোকে একটিমাত্র সিলিকন চিপের ওপর তৈরি করা হয়।

**উপাদানের সংখ্যার ভিত্তিতে আইসির শ্রেণীবিভাগ:**

১. **Small Scale Integration (SSI):** এতে ১০-১২ টির কম লজিক গেট (বা ১০০ টির কম উপাদান) থাকে।

২. **Medium Scale Integration (MSI):** এতে ১০ থেকে ১০০ টি লজিক গেট (বা ১০০ থেকে ১,০০০ টি উপাদান) থাকে।

৩. **Large Scale Integration (LSI):** এতে ১০০ থেকে ১০,০০০ টি লজিক গেট (বা ১,০০০ থেকে ১ লক্ষ উপাদান) থাকে।

৪. **Very Large Scale Integration (VLSI):** এতে ১০,০০০ থেকে ১০ লক্ষ লজিক গেট (বা ১ লক্ষ থেকে ১০ লক্ষ উপাদান) থাকে।

৫. **Ultra Large Scale Integration (ULSI):** এতে ১০ লক্ষের বেশি লজিক গেট বা উপাদান থাকে। (যেমন: আধুনিক প্রসেসর)।

### 3. (b) Discuss in brief, the functional stages of an op-amp with a block diagram.

_(This question is identical to **2023 Question 3(a)**. Please refer to that section for the detailed English and Bengali answer and the block diagram)._

### 3. (c) Define the terms: i) Open-loop gain; (ii) Common mode gain and (iii) Slew rate.

#### English Answer:

1. **Open-loop gain ($A_{ol}$):** It is the voltage gain of the operational amplifier when there is no feedback loop connected between the output and the input terminals. For an ideal op-amp, it is infinite, but practically it is very high (around $10^5$ to $10^6$).
    
2. **Common mode gain ($A_c$):** It is the voltage gain of the op-amp when exactly identical signals ($v_1 = v_2$) are applied simultaneously to both the inverting and non-inverting input terminals. An ideal op-amp rejects common-mode signals completely, so $A_c$ should be zero.
    
3. **Slew rate (SR):** It is defined as the maximum rate at which the output voltage of an op-amp can change in response to a sudden step change in the input. It is expressed in Volts per microsecond ($V/\mu\text{s}$). A higher slew rate means the op-amp can handle higher frequency signals without distortion.
    

#### বাংলা উত্তর:

১. **ওপেন-লুপ গেইন ($A_{ol}$):** অপ-এম্পের আউটপুট থেকে ইনপুটে যখন কোনো ফিডব্যাক সংযুক্ত থাকে না, তখন এর ভোল্টেজ গেইনকে ওপেন-লুপ গেইন বলে। আদর্শ অপ-এম্পের ক্ষেত্রে এটি অসীম হয়।

২. **কমন মোড গেইন ($A_c$):** অপ-এম্পের ইনভার্টিং এবং নন-ইনভার্টিং উভয় ইনপুটে যখন একই সিগন্যাল প্রয়োগ করা হয়, তখন আউটপুট এবং ইনপুট সিগন্যালের অনুপাতকে কমন মোড গেইন বলে। আদর্শ অপ-এম্পের ক্ষেত্রে এর মান শূন্য হওয়া উচিত।

৩. **স্লিউ রেট (Slew Rate):** ইনপুট ভোল্টেজের হঠাৎ পরিবর্তনের ফলে অপ-এম্পের আউটপুট ভোল্টেজ প্রতি একক সময়ে সর্বোচ্চ যে হারে পরিবর্তিত হতে পারে, তাকে স্লিউ রেট বলে। এর একক হলো $V/\mu\text{s}$। স্লিউ রেট বেশি হলে অপ-এম্প উচ্চ কম্পাঙ্কের সিগন্যাল বিকৃত না করেই বিবর্ধিত করতে পারে।

## B.Sc. (Hons) Part-IV Examination - 2020

### 3. (a) Describe the steps followed in fabricating monolithic integrated circuits.

_(This question is identical to **2024 Question 3(c)**. Please refer to that section for the detailed English and Bengali answer)._

### 3. (b) Deduce an expression for the closed-loop voltage gain of an inverting operational amplifier.

_(This question is identical to **2023 Question 3(b)**. Please refer to that section for the detailed English and Bengali answer, including the circuit diagram)._

### 3. (c) i) What is an active filter? ii) Compare active filter with passive filter.

#### English Answer:

**i) Active Filter:** An active filter is an electronic filter circuit that uses active components (such as operational amplifiers or transistors) along with passive components (resistors and capacitors) to filter out unwanted frequency components from a signal.

**ii) Comparison between Active and Passive Filters:**

|**Feature**|**Active Filter**|**Passive Filter**|
|---|---|---|
|**Components Used**|Op-amps/Transistors, Resistors ($R$), Capacitors ($C$).|Resistors ($R$), Capacitors ($C$), Inductors ($L$).|
|**Power Supply**|Requires an external DC power supply.|Does not require an external power supply.|
|**Voltage Gain**|Can provide voltage gain (amplify the signal) along with filtering.|Cannot provide gain; the output signal is always attenuated (lossy).|
|**Inductors**|No inductors are used, making it small, light, and cheap.|Requires inductors, which make it bulky, heavy, and expensive at low frequencies.|
|**Frequency Range**|Best suited for low and audio frequencies. Bandwidth is limited by the Op-amp.|Can operate at very high (radio) frequencies.|

#### বাংলা উত্তর:

**i) অ্যাকটিভ ফিল্টার:** যে ইলেকট্রনিক ফিল্টার সার্কিটে নির্দিষ্ট কম্পাঙ্ককে বাধা দেওয়া বা পার হতে দেওয়ার জন্য নিষ্ক্রিয় উপাদানের (R, C) পাশাপাশি সক্রিয় উপাদান (যেমন- অপ-এম্প, ট্রানজিস্টর) ব্যবহার করা হয়, তাকে অ্যাকটিভ ফিল্টার বলে।

**ii) অ্যাকটিভ ও প্যাসিভ ফিল্টারের তুলনা:**

|**বৈশিষ্ট্য**|**অ্যাকটিভ ফিল্টার (Active Filter)**|**প্যাসিভ ফিল্টার (Passive Filter)**|
|---|---|---|
|**উপাদান**|অপ-এম্প, রেজিস্টর ($R$) এবং ক্যাপাসিটর ($C$) থাকে।|রেজিস্টর ($R$), ক্যাপাসিটর ($C$) এবং ইনডাক্টর ($L$) থাকে।|
|**পাওয়ার সাপ্লাই**|কাজ করার জন্য বাহ্যিক ডিসি পাওয়ার সাপ্লাই প্রয়োজন।|কোনো বাহ্যিক পাওয়ার সাপ্লাই প্রয়োজন হয় না।|
|**ভোল্টেজ গেইন**|এটি সিগন্যাল ফিল্টার করার পাশাপাশি গেইন বা বিবর্ধন করতে পারে।|এটি গেইন দিতে পারে না, বরং সিগন্যালের শক্তি কিছুটা হ্রাস পায়।|
|**ইনডাক্টরের ব্যবহার**|এতে ইনডাক্টর থাকে না, তাই এটি আকারে ছোট, হালকা এবং সস্তা হয়।|এতে ইনডাক্টর থাকে বলে এটি আকারে বড়, ভারী এবং তুলনামূলক ব্যয়বহুল।|
|**কম্পাঙ্ক সীমা**|নিম্ন এবং অডিও কম্পাঙ্কের জন্য বেশি উপযোগী।|অত্যন্ত উচ্চ কম্পাঙ্কের (রেডিও ফ্রিকোয়েন্সি) জন্য উপযোগী।|

## B.Sc. (Hons) Part-IV Examination - 2019

### 3. (a) What is an IC? Write down the advantages and disadvantages of ICs.

#### English Answer:

**Integrated Circuit (IC):** An IC is a single microchip (usually made of silicon) containing numerous interconnected electronic components such as transistors, resistors, capacitors, and diodes, designed to function as a complete electronic circuit.

**Advantages of ICs:**

1. Extremely small size and lightweight.
    
2. Very low cost due to mass production techniques.
    
3. Low power consumption.
    
4. Highly reliable with fewer interconnections, reducing chances of failure.
    
5. High operating speed because of the close proximity of internal components.
    

**Disadvantages of ICs:**

1. Inability to handle high power or high voltage operations.
    
2. Inductors and transformers cannot be easily integrated onto a semiconductor chip.
    
3. High sensitivity to temperature changes.
    
4. If a single internal component fails, the entire IC must be replaced; it cannot be repaired.
    

#### বাংলা উত্তর:

**ইন্টিগ্রেটেড সার্কিট (IC):** আইসি হলো একটি ক্ষুদ্র মাইক্রোচিপ (সিলিকনের তৈরি) যার ওপর ট্রানজিস্টর, ডায়োড, রোধ ও ধারকের মতো অসংখ্য উপাদান একত্রে সংযুক্ত করে একটি সম্পূর্ণ ইলেকট্রনিক বর্তনী তৈরি করা হয়।

**আইসির সুবিধাসমূহ:**

১. আকার অত্যন্ত ছোট এবং ওজন খুব কম।

২. ব্যাপক হারে উৎপাদনের কারণে এর দাম অনেক কম।

৩. এটি খুব কম বিদ্যুৎ খরচ করে।

৪. বাহ্যিক তারের সংযোগ না থাকায় এটি অত্যন্ত নির্ভরযোগ্য।

৫. ভেতরের উপাদানগুলো খুব কাছাকাছি থাকায় এর কাজ করার গতি (Speed) অনেক বেশি।

**আইসির অসুবিধাসমূহ:**

১. এটি বেশি পাওয়ার বা উচ্চ ভোল্টেজ নিয়ে কাজ করতে পারে না।

২. ইনডাক্টর এবং ট্রান্সফরমার আইসির ভেতরে তৈরি করা যায় না।

৩. এটি তাপমাত্রার পরিবর্তনের প্রতি অত্যন্ত সংবেদনশীল।

৪. এর ভেতরের একটি অংশ নষ্ট হলে পুরো আইসি বাতিল করতে হয়, এটি মেরামত করা যায় না।

### 3. (b) Discuss, in brief, the functional stages of an op-amp with a block diagram.

_(This question is identical to **2023 Question 3(a)**. Please refer to that section for the detailed English and Bengali answer and the block diagram)._

### 3. (c) Define the terms: i) Open-loop gain, ii) Common mode gain, iii) Slew rate.

_(This question is identical to **2021 Question 3(c)**. Please refer to that section for the detailed English and Bengali answer)._