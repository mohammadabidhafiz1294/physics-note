## B.Sc. (Hons) Part-IV Examination - 2024

### 2. (a) Explain the operation of a blocking oscillator. Include the role of the transformer, feedback, and transistor.

#### English Answer:

A **blocking oscillator** is a type of relaxation oscillator that uses a single transistor and a pulse transformer to generate very narrow, high-power pulses followed by long resting (cut-off) intervals.

- **Role of Transistor:** It acts as the primary active switching element. When it turns ON, it allows current to flow through the transformer's primary winding.
    
- **Role of Transformer:** The pulse transformer couples the collector circuit back to the base circuit. It dictates the pulse width and provides the necessary phase inversion for positive feedback.
    
- **Role of Feedback:** The transformer provides heavy regenerative (positive) feedback. This ensures that the transistor is driven rapidly into deep saturation (creating the sharp leading edge of the pulse) and then rapidly into cut-off (creating the sharp trailing edge).
    

**Working Principle:**

When the circuit is turned on, a small base current starts flowing, causing collector current to rise. This rising current through the transformer's primary induces a voltage in the secondary winding, which is fed back to the base with positive polarity. This regenerative feedback instantly drives the transistor into saturation. The capacitor at the base charges up during this ON time. Once the transformer core saturates or the capacitor charges fully, the feedback is lost, and the transistor rapidly cuts off. The capacitor then slowly discharges through a base resistor, keeping the transistor blocked (OFF) until the voltage rises enough to turn the transistor ON again.

#### বাংলা উত্তর:

একটি **ব্লকিং অসিলেটর** হলো এক ধরনের রিলাক্সেশন অসিলেটর যা একটিমাত্র ট্রানজিস্টর এবং একটি পালস ট্রান্সফর্মার ব্যবহার করে অত্যন্ত সরু এবং উচ্চ-ক্ষমতার পালস তৈরি করে, যার মাঝে দীর্ঘ বিরতি (cut-off) থাকে।

- **ট্রানজিস্টরের ভূমিকা:** এটি প্রধান সুইচিং উপাদান হিসেবে কাজ করে। এটি চালু (ON) হলে ট্রান্সফর্মারের প্রাইমারি কয়েলের মধ্য দিয়ে বিদ্যুৎ প্রবাহিত হয়।
    
- **ট্রান্সফর্মারের ভূমিকা:** পালস ট্রান্সফর্মার কালেক্টর সার্কিটকে পুনরায় বেস সার্কিটের সাথে যুক্ত করে। এটি পালসের প্রস্থ নির্ধারণ করে এবং পজিটিভ ফিডব্যাকের জন্য প্রয়োজনীয় ফেজ ইনভার্সন প্রদান করে।
    
- **ফিডব্যাকের ভূমিকা:** ট্রান্সফর্মার অত্যন্ত শক্তিশালী পজিটিভ (রিজেনারেটিভ) ফিডব্যাক প্রদান করে। এর ফলে ট্রানজিস্টরটি খুব দ্রুত ডিপ স্যাচুরেশনে চলে যায় (যাতে পালসের অগ্রভাগ তৈরি হয়) এবং পরবর্তীতে দ্রুত কাট-অফে চলে যায়।
    

**কার্যনীতি:**

সার্কিটটি চালু হলে সামান্য বেস কারেন্ট প্রবাহিত হয়, ফলে কালেক্টর কারেন্ট বাড়তে থাকে। ট্রান্সফর্মারের প্রাইমারিতে এই কারেন্ট বৃদ্ধির ফলে সেকেন্ডারিতে একটি ভোল্টেজ আবিষ্ট হয়, যা পজিটিভ পোলারিটি সহ বেসে ফিরে আসে। এই পজিটিভ ফিডব্যাক ট্রানজিস্টরটিকে দ্রুত স্যাচুরেশনে নিয়ে যায়। এই ON থাকার সময়ে বেসের ক্যাপাসিটরটি চার্জ হতে থাকে। যখন ট্রান্সফর্মার কোর স্যাচুরেটেড হয়ে যায় বা ক্যাপাসিটরটি সম্পূর্ণ চার্জ হয়ে যায়, তখন ফিডব্যাক বন্ধ হয়ে যায় এবং ট্রানজিস্টরটি দ্রুত কাট-অফ বা বন্ধ হয়ে যায়। এরপর ক্যাপাসিটরটি একটি রোধের মাধ্যমে ধীরে ধীরে ডিসচার্জ হয়, যা ট্রানজিস্টরটিকে দীর্ঘ সময়ের জন্য ব্লক (OFF) করে রাখে, যতক্ষণ না ভোল্টেজ পুনরায় ট্রানজিস্টরটিকে অন করার জন্য পর্যাপ্ত হয়।

### 2. (b) Describe a linear time-base generator and its importance in oscilloscopes and sweep circuits.

#### English Answer:

- **Linear Time-Base Generator:** A linear time-base generator (also known as a sweep generator) is an electronic circuit designed to produce an output voltage or current that increases linearly with time (constant slope) for a specific duration, and then rapidly drops back to its initial value. The resulting waveform resembles a sawtooth wave.
    
- **Importance in Oscilloscopes & Sweep Circuits:** In a Cathode Ray Oscilloscope (CRO), this linearly increasing sweep voltage is applied to the horizontal deflection plates. It sweeps the electron beam horizontally across the screen from left to right at a constant speed, creating a uniform time axis. Without this linear ramp, it would be impossible to accurately display, view, and measure time-domain characteristics (such as frequency, period, and phase) of an unknown input signal.
    

#### বাংলা উত্তর:

- **লিনিয়ার টাইম-বেস জেনারেটর:** লিনিয়ার টাইম-বেস জেনারেটর (বা সুইপ জেনারেটর) হলো এমন একটি ইলেকট্রনিক সার্কিট যা এমন একটি আউটপুট ভোল্টেজ বা কারেন্ট তৈরি করে যা সময়ের সাথে সমানুপাতিক হারে (রৈখিকভাবে) বৃদ্ধি পায় এবং একটি নির্দিষ্ট সময় পর খুব দ্রুত তার প্রাথমিক অবস্থায় নেমে আসে। এর ফলে তৈরি হওয়া তরঙ্গটি করাত-দাঁতী (Sawtooth) তরঙ্গের মতো দেখায়।
    
- **অসিলোস্কোপ এবং সুইপ সার্কিটে এর গুরুত্ব:** ক্যাথোড রে অসিলোস্কোপে (CRO) এই লিনিয়ার সুইপ ভোল্টেজটি অনুভূমিক (horizontal) ডিফ্লেকশন প্লেটে প্রয়োগ করা হয়। এটি ইলেকট্রন বিমকে স্ক্রিনের বাম থেকে ডান দিকে একটি ধ্রুব বেগে সরিয়ে নিয়ে যায়, যা একটি সুষম সময়ের অক্ষ (time axis) তৈরি করে। এই লিনিয়ার র‍্যাম্প ছাড়া কোনো অজানা ইনপুট সিগন্যালের সময়-নির্ভর বৈশিষ্ট্যগুলো (যেমন- কম্পাঙ্ক, পর্যায়কাল এবং ফেজ) নিখুঁতভাবে পর্দায় দেখা বা পরিমাপ করা অসম্ভব।
    

### 2. (c) A blocking oscillator uses a transformer with a turns ratio of 1:10. The supply voltage is 12 V, and the base resistor is 1 kΩ. Assuming transistor parameters such that the oscillator produces pulses every 50 μs, calculate approximate pulse repetition frequency.

#### English Answer:

**Given:**

- Transformer turns ratio = $1:10$
    
- Supply voltage $V_{CC} = 12\text{ V}$
    
- Base resistor $R_B = 1\text{ k}\Omega$
    
- Pulse period (time between pulses) $T = 50\ \mu\text{s} = 50 \times 10^{-6}\text{ s}$
    

**Calculation:**

The question provides various circuit parameters, but explicitly states that the oscillator produces pulses every $50\ \mu\text{s}$. This value ($50\ \mu\text{s}$) is the total time period ($T$) of the oscillator.

The Pulse Repetition Frequency (PRF) is the reciprocal of the total time period.

$$PRF = \frac{1}{T} = \frac{1}{50 \times 10^{-6}\text{ s}} = 20,000\text{ Hz} = 20\text{ kHz}$$

#### বাংলা সমাধান:

**প্রদত্ত:**

- ট্রান্সফর্মারের টার্নস রেশিও = $1:10$
    
- সাপ্লাই ভোল্টেজ $V_{CC} = 12\text{ V}$
    
- বেস রোধ $R_B = 1\text{ k}\Omega$
    
- পালসের পর্যায়কাল (দুটি পালসের মধ্যবর্তী সময়) $T = 50\ \mu\text{s} = 50 \times 10^{-6}\text{ s}$
    

**গণনা:**

প্রশ্নে অন্যান্য মান দেওয়া থাকলেও, সরাসরি উল্লেখ করা আছে যে অসিলেটরটি প্রতি $50\ \mu\text{s}$ পর পর পালস তৈরি করে। অর্থাৎ এটিই হলো মোট পর্যায়কাল ($T$)।

পালস রিপিটিশন ফ্রিকোয়েন্সি (PRF) হলো পর্যায়কালের বিপরীত রাশি।

$$PRF = \frac{1}{T} = \frac{1}{50 \times 10^{-6}\text{ s}} = 20,000\text{ Hz} = 20\text{ kHz}$$

### 2. (d) Compare a blocking oscillator and an astable multivibrator.

#### English Answer:

|**Feature**|**Blocking Oscillator**|**Astable Multivibrator**|
|---|---|---|
|**Active Components**|Uses a single transistor.|Uses two cross-coupled transistors.|
|**Feedback Mechanism**|Uses inductive (transformer) positive feedback.|Uses capacitive cross-coupled positive feedback.|
|**Waveform Generated**|Generates very narrow, high-power sharp pulses with long off-times.|Typically generates symmetrical or asymmetrical square/rectangular waves.|
|**Duty Cycle**|Extremely low duty cycle (pulse width is much smaller than off-time).|Usually 50% (symmetrical) or moderately asymmetrical duty cycle.|
|**Complexity & Cost**|Requires a pulse transformer, making it bulkier and slightly more expensive.|Uses simple RC components, making it cheaper and easy to integrate into ICs.|

#### বাংলা উত্তর:

|**বৈশিষ্ট্য**|**ব্লকিং অসিলেটর (Blocking Oscillator)**|**অ্যাস্টেবল মাল্টিভাইব্রেটর (Astable Multivibrator)**|
|---|---|---|
|**সক্রিয় উপাদান**|একটিমাত্র ট্রানজিস্টর ব্যবহৃত হয়।|দুটি ক্রস-কাপলড ট্রানজিস্টর ব্যবহৃত হয়।|
|**ফিডব্যাক মেকানিজম**|পালস ট্রান্সফর্মারের মাধ্যমে ইনডাকটিভ পজিটিভ ফিডব্যাক ব্যবহার করে।|ক্যাপাসিটরের মাধ্যমে ক্রস-কাপলড পজিটিভ ফিডব্যাক ব্যবহার করে।|
|**তরঙ্গের ধরন**|দীর্ঘ গ্যাপযুক্ত অত্যন্ত সরু ও উচ্চ-ক্ষমতার তীক্ষ্ণ পালস তৈরি করে।|সাধারণত বর্গাকার (Square) বা আয়তাকার (Rectangular) তরঙ্গ তৈরি করে।|
|**ডিউটি সাইকেল**|এর ডিউটি সাইকেল খুবই কম হয়।|সাধারণত ৫০% (সুষম) বা মাঝারি মানের ডিউটি সাইকেল হয়।|
|**গঠনগত জটিলতা**|পালস ট্রান্সফর্মার প্রয়োজন হয়, যা আকারে বড় এবং ব্যয়বহুল।|সাধারণ রোধ ও ধারক (RC) দিয়ে তৈরি হয়, যা সস্তা এবং IC-তে বসানো সহজ।|

## B.Sc. (Hons) Part-IV Examination - 2023

### 2. (a) What is a relaxation oscillator?

#### English Answer:

A **relaxation oscillator** is a non-linear electronic oscillator circuit that produces a non-sinusoidal output waveform, such as a square wave, triangular wave, or sawtooth wave. It works by repeatedly charging a reactive element (like a capacitor or inductor) through a resistor until it reaches a specific threshold voltage, and then rapidly discharging it, "relaxing" back to its initial state to begin the cycle again.

#### বাংলা উত্তর:

**রিলাক্সেশন অসিলেটর** হলো এমন এক ধরনের অরৈখিক (non-linear) ইলেকট্রনিক অসিলেটর সার্কিট, যা নন-সাইনুসয়ডাল তরঙ্গ (যেমন- স্কয়ার ওয়েভ, ট্রায়াঙ্গুলার ওয়েভ বা স-টুথ ওয়েভ) তৈরি করে। এটি মূলত একটি রোধের মধ্য দিয়ে একটি ক্যাপাসিটরকে (বা ইনডাক্টরকে) চার্জ করে এবং একটি নির্দিষ্ট থ্রেশহোল্ড ভোল্টেজে পৌঁছানোর পর খুব দ্রুত ডিসচার্জ করে (রিলাক্স করে) পুনরায় আগের অবস্থায় ফিরে আসে এবং চক্রটির পুনরাবৃত্তি করে।

### 2. (b) Explain the working principle of a symmetrical astable multivibrator and draw its output waveforms. Sketch the charging and discharging paths.

#### Circuit Diagram:

Plaintext

```
           + VCC
             |
   +----+----+----+----+
   |    |         |    |
  [R1] [R2]      [R3] [R4]
   |    |         |    |
   |    +---||----+    |
   |   C1         C2   |
 Vc1+---+         +---+Vc2
   |    |         |    |
   |    +---------+    |
   |         X         |
   |    +----+----+    |
   |    |         |    |
 |/    [Rb1]   [Rb2]    \|
-Q1(NPN)|         |      Q2(NPN)-
 |\     |         |      /|
   |    |         |    |
  GND  GND       GND  GND

* R1=R4 (Collector Resistors Rc)
* R2=R3 (Base Resistors Rb)
* C1=C2 (Coupling Capacitors C)
```

#### English Answer:

**Working Principle:**

A symmetrical astable multivibrator consists of two cross-coupled NPN transistors ($Q_1$ and $Q_2$). Since it is astable, it has no stable states; it continuously switches back and forth between two quasi-stable states.

1. When power is applied, slight circuit imbalances cause one transistor (e.g., $Q_1$) to turn ON faster than the other ($Q_2$).
    
2. **State 1 ($Q_1$ ON, $Q_2$ OFF):** The collector voltage of $Q_1$ drops to near $0\text{ V}$. This negative voltage transition is transmitted through capacitor $C_1$ to the base of $Q_2$, driving $Q_2$ deep into cutoff (OFF). Since $Q_2$ is OFF, its collector sits at $+V_{CC}$.
    
3. **Transition:** While $Q_2$ is OFF, capacitor $C_1$ starts charging through base resistor $R_3$ (towards $+V_{CC}$). Once the voltage at the base of $Q_2$ reaches approximately $+0.7\text{ V}$, $Q_2$ turns ON.
    
4. **State 2 ($Q_2$ ON, $Q_1$ OFF):** $Q_2$ turning ON drops its collector voltage to $0\text{ V}$. This drop is transmitted via $C_2$ to the base of $Q_1$, immediately turning $Q_1$ OFF. Capacitor $C_2$ now charges through $R_2$ until $Q_1$ turns ON again. This cycle repeats indefinitely.
    

- **Charging Path for $C_1$ (when $Q_1$ is ON):** $+V_{CC} \rightarrow R_3 \rightarrow C_1 \rightarrow Q_1 (\text{Collector-Emitter}) \rightarrow \text{Ground}$.
    
- **Discharging/Recharging Path for $C_1$ (when $Q_1$ turns OFF):** Ground $\rightarrow \text{Base-Emitter of } Q_2 \rightarrow C_1 \rightarrow R_1 \rightarrow +V_{CC}$.
    

#### Waveforms:

Plaintext

```
Vc1 (Q1 Collector)
 Vcc |   +----+      +----+
     |   |    |      |    |
   0 +---+    +------+    +---> t

Vb2 (Q2 Base)
0.7V |   .    +--    .    +--
   0 + - | - / - - - | - / - -> t
 -Vcc|   +--+        +--+

Vc2 (Q2 Collector)
 Vcc |---+    +------+    +--
     |   |    |      |    |
   0 +   +----+      +----+---> t
```

#### বাংলা উত্তর:

**কার্যনীতি:**

একটি সুষম (symmetrical) অ্যাস্টেবল মাল্টিভাইব্রেটরে দুটি ক্রস-কাপলড ট্রানজিস্টর ($Q_1$ এবং $Q_2$) থাকে। এর কোনো স্থায়ী অবস্থা নেই; এটি পর্যায়ক্রমে দুটি অস্থায়ী অবস্থার মধ্যে পরিবর্তন হয়।

১. সার্কিটে বিদ্যুৎ সরবরাহ করা হলে, ট্রানজিস্টরগুলোর অভ্যন্তরীণ সামান্য অসামঞ্জস্যতার কারণে একটি (ধরি $Q_1$) অন্যটির ($Q_2$) চেয়ে আগে চালু (ON) হয়।

২. **অবস্থা ১ ($Q_1$ ON, $Q_2$ OFF):** $Q_1$ চালু হলে এর কালেক্টর ভোল্টেজ প্রায় $0\text{ V}$-এ নেমে যায়। এই ভোল্টেজ ড্রপ $C_1$-এর মাধ্যমে $Q_2$-এর বেসে পৌঁছায় এবং $Q_2$-কে কাট-অফ (OFF) করে দেয়। এসময় $Q_2$-এর কালেক্টর ভোল্টেজ $+V_{CC}$ থাকে।

৩. **অবস্থা পরিবর্তন:** $Q_2$ যখন বন্ধ থাকে, তখন ক্যাপাসিটর $C_1$, বেস রোধ $R_3$-এর মধ্য দিয়ে $+V_{CC}$-এর দিকে ধীরে ধীরে চার্জ হতে থাকে। $Q_2$-এর বেস ভোল্টেজ বৃদ্ধি পেয়ে $+0.7\text{ V}$-এ পৌঁছালে, $Q_2$ চালু (ON) হয়ে যায়।

৪. **অবস্থা ২ ($Q_2$ ON, $Q_1$ OFF):** $Q_2$ চালু হলে এর কালেক্টর ভোল্টেজ শূন্য হয়ে যায়, যা $C_2$-এর মাধ্যমে $Q_1$-এর বেসে নেগেটিভ পালস পাঠায় এবং $Q_1$-কে বন্ধ করে দেয়। এরপর $C_2$ চার্জ হতে থাকে এবং প্রক্রিয়াটি ক্রমাগত চলতে থাকে।

- **চার্জিং পথ ($C_1$ এর জন্য):** $+V_{CC} \rightarrow R_3 \rightarrow C_1 \rightarrow Q_1 (\text{Collector-Emitter}) \rightarrow \text{Ground}$
    
- **ডিসচার্জিং পথ ($C_1$ এর জন্য):** $\text{Ground} \rightarrow Q_2 (\text{Base-Emitter}) \rightarrow C_1 \rightarrow R_1 \rightarrow +V_{CC}$
    

### 2. (c) Why is the hysteresis desirable in Schmitt trigger circuit?

#### English Answer:

Hysteresis in a Schmitt trigger means that the circuit has two distinct threshold voltage levels for switching: an Upper Trigger Point (UTP) and a Lower Trigger Point (LTP).

Hysteresis is highly desirable because it provides **noise immunity**. If an input signal contains electrical noise or small fluctuations, a standard comparator without hysteresis might rapidly switch its output back and forth (known as "chattering" or false triggering) as the noise fluctuates around a single threshold point. The hysteresis band (the voltage gap between UTP and LTP) ensures that once the output changes state, the noise must exceed this entire voltage gap to falsely trigger it back. This results in clean, reliable, and sharp output transitions.

#### বাংলা উত্তর:

শ্মিট ট্রিগার সার্কিটে হিস্টেরেসিস থাকার অর্থ হলো, এর ইনপুট সংকেত পরিবর্তনের জন্য দুটি ভিন্ন থ্রেশহোল্ড ভোল্টেজ লেভেল থাকে: আপার ট্রিগার পয়েন্ট (UTP) এবং লোয়ার ট্রিগার পয়েন্ট (LTP)।

হিস্টেরেসিস অত্যন্ত কাঙ্ক্ষিত কারণ এটি সার্কিটকে **নয়েজ ইমিউনিটি (Noise Immunity)** প্রদান করে। যদি কোনো ইনপুট সিগন্যালে ইলেকট্রিক্যাল নয়েজ বা ছোট পরিবর্তন থাকে, তবে একটি সাধারণ কম্পারেটর (যাতে হিস্টেরেসিস নেই) সিগন্যালটিকে বারবার অন-অফ করতে পারে (যাকে চ্যাটারিং বলে)। হিস্টেরেসিস ব্যান্ড (UTP এবং LTP এর মধ্যকার পার্থক্য) নিশ্চিত করে যে একবার আউটপুট অবস্থা পরিবর্তন করলে, নয়েজকে অবশ্যই এই পুরো ভোল্টেজ গ্যাপ অতিক্রম করতে হবে আউটপুটকে পুনরায় মিথ্যা ট্রিগার করতে। এর ফলে একটি পরিষ্কার ও নির্ভরযোগ্য আউটপুট পাওয়া যায়।

### 2. (d) In a symmetrical astable multivibrator $R_B = 15\text{ k}\Omega$, $R_L = 1\text{ k}\Omega$ and coupling capacitor $100\text{ pF}$ with $V_{CC} = 10\text{ V}$. Determine (i) $(I_C)_{sat}$, (ii) $(V_B \text{ off})_{t=0}$, (iii) $(V_B)_{on}$ and (iv) frequency of oscillation.

#### English Answer:

**Given Data:**

- $V_{CC} = 10\text{ V}$
    
- Base Resistor $R_B = 15\text{ k}\Omega$
    
- Load (Collector) Resistor $R_L = 1\text{ k}\Omega$
    
- Coupling Capacitor $C = 100\text{ pF} = 100 \times 10^{-12}\text{ F}$
    

**Calculations:**

**(i) Collector saturation current $(I_C)_{sat}$:**

Assuming ideal saturation where $V_{CE(sat)} \approx 0\text{ V}$:

$$(I_C)_{sat} = \frac{V_{CC}}{R_L} = \frac{10\text{ V}}{1\text{ k}\Omega} = 10\text{ mA}$$

**(ii) Initial base voltage of the OFF transistor $(V_B \text{ off})_{t=0}$:**

When a transistor just switches OFF, the capacitor cross-coupling pushes the base voltage down by an amount equal to $V_{CC}$ (from approx $0\text{ V}$ to $-V_{CC}$).

$$(V_B \text{ off})_{t=0} \approx -V_{CC} = -10\text{ V}$$

**(iii) Base voltage of the ON transistor $(V_B)_{on}$:**

For a standard silicon transistor in saturation, the base-emitter voltage is approximately $0.7\text{ V}$.

$$(V_B)_{on} \approx V_{BE(sat)} = +0.7\text{ V}$$

**(iv) Frequency of oscillation ($f$):**

For a symmetrical astable multivibrator, the total time period is $T = 1.38 R_B C$.

$$T = 1.38 \times (15 \times 10^3\ \Omega) \times (100 \times 10^{-12}\text{ F}) = 2.07 \times 10^{-6}\text{ s}$$

$$f = \frac{1}{T} = \frac{1}{2.07 \times 10^{-6}\text{ s}} \approx 483,091\text{ Hz} \approx 483\text{ kHz}$$

#### বাংলা সমাধান:

**(i) কালেক্টর স্যাচুরেশন কারেন্ট $(I_C)_{sat}$:** $(I_C)_{sat} = \frac{10\text{ V}}{1\text{ k}\Omega} = 10\text{ mA}$

**(ii) অফ অবস্থায় প্রাথমিক বেস ভোল্টেজ $(V_B \text{ off})_{t=0}$:** ক্যাপাসিটিভ কাপলিংয়ের কারণে এটি তাৎক্ষণিকভাবে $-V_{CC}$ তে নেমে যায়।

$(V_B \text{ off})_{t=0} = -10\text{ V}$

**(iii) অন অবস্থায় বেস ভোল্টেজ $(V_B)_{on}$:** সিলিকন ট্রানজিস্টরের ক্ষেত্রে এটি সাধারণত $+0.7\text{ V}$ হয়।

$(V_B)_{on} = +0.7\text{ V}$

**(iv) দোলনের কম্পাঙ্ক ($f$):** $f = \frac{1}{1.38 R_B C} = \frac{1}{1.38 \times 15 \times 10^3 \times 100 \times 10^{-12}} = \frac{1}{2.07 \times 10^{-6}} \approx 483\text{ kHz}$

## B.Sc. (Hons) Part-IV Examination - 2022

### 2. (a) Mention the basic differences among relaxation oscillators.

#### English Answer:

Relaxation oscillators (specifically multivibrators) are broadly classified into three categories based on their stable states:

1. **Astable Multivibrator:** It has **zero (no) stable states**. It automatically switches back and forth between two quasi-stable states, generating a continuous periodic output without requiring any external trigger.
    
2. **Monostable Multivibrator:** It has **one stable state** and one quasi-stable state. It remains in its stable state until an external trigger pulse forces it into the quasi-stable state. After a predetermined time (set by an RC circuit), it automatically returns to its stable state.
    
3. **Bistable Multivibrator:** It has **two stable states**. It remains in a given state indefinitely until an external trigger pulse forces it to switch to the other state. It requires a distinct trigger for every state transition.
    

#### বাংলা উত্তর:

রিলাক্সেশন অসিলেটরগুলো (বিশেষ করে মাল্টিভাইব্রেটর) তাদের স্থিতিশীল অবস্থার (stable states) উপর ভিত্তি করে প্রধানত তিনটি ভাগে বিভক্ত:

১. **অ্যাস্টেবল মাল্টিভাইব্রেটর:** এর **কোনো স্থায়ী অবস্থা নেই**। এটি বাহ্যিক কোনো ট্রিগার ছাড়াই স্বয়ংক্রিয়ভাবে দুটি অস্থায়ী অবস্থার মধ্যে পরিবর্তিত হয় এবং ক্রমাগত পর্যায়বৃত্ত তরঙ্গ তৈরি করে।

২. **মনোস্টেবল মাল্টিভাইব্রেটর:** এর **একটি স্থায়ী অবস্থা** এবং একটি অস্থায়ী অবস্থা থাকে। এটি একটি বাহ্যিক ট্রিগার প্রয়োগ না করা পর্যন্ত স্থায়ী অবস্থায় থাকে। ট্রিগার প্রয়োগ করলে এটি অস্থায়ী অবস্থায় যায় এবং একটি নির্দিষ্ট সময় (RC টাইম কনস্ট্যান্ট দ্বারা নির্ধারিত) পর স্বয়ংক্রিয়ভাবে স্থায়ী অবস্থায় ফিরে আসে।

৩. **বাইস্টেবল মাল্টিভাইব্রেটর:** এর **দুটি স্থায়ী অবস্থা** থাকে। এটি যেকোনো একটি অবস্থায় অনির্দিষ্টকালের জন্য স্থির থাকতে পারে। বাহ্যিক ট্রিগার প্রয়োগ করা হলে এটি এক অবস্থা থেকে অন্য অবস্থায় পরিবর্তিত হয়। এর প্রতিটি পরিবর্তনের জন্য আলাদা ট্রিগার প্রয়োজন।

### 2. (b) Describe the construction and working principle of a fixed bias transistor binary using necessary diagrams and mention its applications.

#### Circuit Diagram:

Plaintext

```
           + VCC
             |
       +-----+-----+
       |           |
     [Rc1]       [Rc2]
       |           |
 Vc1+--+--[R1]-+---+--+Vc2
    |  |       |   |  |
    |  +-[R1']-+   |  |
    |              |  |
  |/               \| |
 -Q1(NPN)       (NPN)Q2-
  |\               /|
    |  +--[R2]--+  |
    |  |        |  |
    |  +--[R2']-+  |
    |  |        |  |
   GND -VBB    -VBB GND
```

#### English Answer:

**Construction:**

A fixed-bias transistor binary (Bistable Multivibrator) consists of two identical NPN transistors ($Q_1$ and $Q_2$). The collector of $Q_1$ is resistively coupled to the base of $Q_2$ via $R_1$, and the collector of $Q_2$ is coupled to the base of $Q_1$ via $R_1'$. The bases of both transistors are also connected to a negative biasing voltage source ($-V_{BB}$) through resistors $R_2$ and $R_2'$. This negative bias ensures that the OFF transistor is driven deeply into cutoff.

**Working Principle:**

Because of heavy regenerative cross-coupling, one transistor is always driven to saturation (ON) while the other is driven to cutoff (OFF).

- Suppose $Q_1$ is ON and $Q_2$ is OFF. The collector voltage of $Q_1$ is near $0\text{ V}$.
    
- This very low voltage, combined with the negative $-V_{BB}$, ensures the base of $Q_2$ is held at a negative potential, keeping $Q_2$ firmly OFF.
    
- Since $Q_2$ is OFF, no current flows through its collector resistor $R_{c2}$, making its collector voltage high (near $+V_{CC}$).
    
- This high voltage drives current through $R_1'$ into the base of $Q_1$, keeping $Q_1$ firmly ON.
    
- The circuit holds this stable state indefinitely until an external trigger pulse is applied to flip the states.
    

**Applications:**

Used in digital electronics as basic memory cells (Flip-Flops), in frequency dividers, and in binary counting circuits.

#### বাংলা উত্তর:

**গঠন:**

একটি ফিক্সড বায়াস বাইনারি (বাইস্টেবল মাল্টিভাইব্রেটর) সার্কিটে দুটি সমরূপ NPN ট্রানজিস্টর ($Q_1$ এবং $Q_2$) থাকে। $Q_1$-এর কালেক্টর একটি রোধ $R_1$-এর মাধ্যমে $Q_2$-এর বেসের সাথে এবং $Q_2$-এর কালেক্টর $R_1'$-এর মাধ্যমে $Q_1$-এর বেসের সাথে যুক্ত থাকে। অফ (OFF) ট্রানজিস্টরটিকে সম্পূর্ণ কাট-অফে (Cutoff) রাখার জন্য বেস দুটিকে রোধ $R_2$ ও $R_2'$-এর মাধ্যমে একটি নেগেটিভ বায়াস ভোল্টেজ ($-V_{BB}$)-এর সাথে যুক্ত করা হয়।

**কার্যনীতি:**

শক্তিশালী ক্রস-কাপলড ফিডব্যাকের কারণে এর একটি ট্রানজিস্টর সবসময় স্যাচুরেশনে (ON) এবং অন্যটি কাট-অফে (OFF) থাকে।

- ধরি $Q_1$ অন এবং $Q_2$ অফ আছে। $Q_1$ অন থাকায় এর কালেক্টর ভোল্টেজ প্রায় $0\text{ V}$ হয়।
    
- এই নিম্ন ভোল্টেজ এবং $-V_{BB}$-এর কারণে $Q_2$-এর বেস ভোল্টেজ নেগেটিভ হয়, ফলে $Q_2$ দৃঢ়ভাবে অফ থাকে।
    
- যেহেতু $Q_2$ অফ, তাই এর কালেক্টর ভোল্টেজ উচ্চ (প্রায় $+V_{CC}$) হয়।
    
- এই উচ্চ ভোল্টেজ $Q_1$-এর বেসে পর্যাপ্ত কারেন্ট পাঠায়, যা $Q_1$-কে অন ধরে রাখে।
    
- বাহ্যিক ট্রিগার প্রয়োগ না করা পর্যন্ত সার্কিটটি এই অবস্থায় স্থিতিশীল থাকে।
    

**ব্যবহার:**

ডিজিটাল লজিকে বেসিক মেমরি সেল (ফ্লিপ-ফ্লপ) হিসেবে, ফ্রিকোয়েন্সি ডিভাইডার এবং বাইনারি কাউন্টিং সার্কিটে ব্যবহৃত হয়।

### 2. (c) Calculate the stable state current and voltages of a flip-flop circuit using $V_{CC} = 12\text{ V}$, $R_{c1} = R_{c2} = 2.2\text{ k}\Omega$, $R_1 = R_1' = 15\text{ k}\Omega$, $R_2 = R_2' = 100\text{ k}\Omega$ and $V_{BB} = -12\text{ V}$ (here $h_{fe} = 20$).

#### English Answer:

Let $Q_1$ be OFF and $Q_2$ be ON (Stable State). Assume standard silicon parameters: $V_{CE(sat)} \approx 0.2\text{ V}$ and $V_{BE(sat)} \approx 0.7\text{ V}$.

**1. Stable State Collector Current of ON Transistor ($Q_2$):**

$$I_{C2(sat)} = \frac{V_{CC} - V_{CE(sat)}}{R_{c2}} = \frac{12\text{ V} - 0.2\text{ V}}{2.2\text{ k}\Omega} = \frac{11.8\text{ V}}{2.2\text{ k}\Omega} = 5.36\text{ mA}$$

**2. Voltage at Collector of OFF Transistor ($V_{C1}$):**

Current $I_1$ flows from $V_{CC}$ through $R_{c1}$ and $R_1$ into the base of $Q_2$ (which is at $0.7\text{ V}$).

$$I_1 = \frac{V_{CC} - V_{BE(sat)}}{R_{c1} + R_1} = \frac{12\text{ V} - 0.7\text{ V}}{2.2\text{ k}\Omega + 15\text{ k}\Omega} = \frac{11.3\text{ V}}{17.2\text{ k}\Omega} = 0.657\text{ mA}$$

$$V_{C1(off)} = V_{CC} - I_1 R_{c1} = 12\text{ V} - (0.657\text{ mA} \times 2.2\text{ k}\Omega) = 12 - 1.445 = 10.55\text{ V}$$

**3. Voltage at Base of OFF Transistor ($V_{B1}$):**

This voltage is determined by the voltage divider formed by $R_1'$ and $R_2'$ between $Q_2$'s collector ($V_{CE(sat)} = 0.2\text{ V}$) and $V_{BB}$ ($-12\text{ V}$).

$$V_{B1(off)} = V_{BB} + \left(\frac{V_{CE(sat)} - V_{BB}}{R_1' + R_2'}\right) R_2'$$

$$V_{B1(off)} = -12 + \left(\frac{0.2 - (-12)}{15\text{ k} + 100\text{ k}}\right) \times 100\text{ k} = -12 + \left(\frac{12.2}{115}\right) \times 100 = -12 + 10.61 = -1.39\text{ V}$$

_(The negative voltage confirms $Q_1$ is firmly OFF)._

#### বাংলা সমাধান:

ধরি $Q_1$ অফ (OFF) এবং $Q_2$ অন (ON) অবস্থায় আছে।

**১. ON ট্রানজিস্টরের কালেক্টর কারেন্ট ($I_{C2}$):**

$$I_{C2(sat)} = \frac{12 - 0.2}{2.2\text{ k}\Omega} = 5.36\text{ mA}$$

**২. OFF ট্রানজিস্টরের কালেক্টর ভোল্টেজ ($V_{C1}$):** $V_{CC}$ থেকে $R_{c1}$ ও $R_1$ হয়ে $Q_2$-এর বেস পর্যন্ত প্রবাহিত কারেন্ট $I_1$:

$$I_1 = \frac{12 - 0.7}{2.2\text{ k} + 15\text{ k}} = 0.657\text{ mA}$$

অতএব,

$$V_{C1(off)} = 12 - (0.657 \times 2.2) = 10.55\text{ V}$$

**৩. OFF ট্রানজিস্টরের বেস ভোল্টেজ ($V_{B1}$):** এটি $V_{CE(sat)}$ ($0.2\text{ V}$) এবং $V_{BB}$ ($-12\text{ V}$) এর মধ্যে ভোল্টেজ ডিভাইডারের কারণে তৈরি হয়:

$$V_{B1(off)} = -12 + \frac{0.2 - (-12)}{15\text{ k} + 100\text{ k}} \times 100\text{ k} = -12 + 10.61 = -1.39\text{ V}$$

### 2. (d) What is the effect of omitting $R_E$ in a Schmitt trigger circuit?

#### English Answer:

In a standard Schmitt trigger circuit, the common emitter resistor $R_E$ provides the regenerative (positive) feedback necessary for the circuit to snap rapidly between its states and create the hysteresis band (the difference between Upper and Lower Trigger Points).

If $R_E$ is omitted (bypassed or grounded directly), the coupling between the emitters is lost. The circuit completely loses its positive feedback loop and hysteresis property. It ceases to act as a Schmitt trigger and instead behaves simply as a standard, high-gain non-linear amplifier or a basic comparator without any noise immunity.

#### বাংলা উত্তর:

একটি সাধারণ শ্মিট ট্রিগার সার্কিটে, কমন এমিটার রোধ $R_E$ প্রয়োজনীয় পজিটিভ ফিডব্যাক প্রদান করে যা সার্কিটটিকে খুব দ্রুত অবস্থা পরিবর্তন করতে এবং হিস্টেরেসিস (UTP এবং LTP এর পার্থক্য) তৈরি করতে সাহায্য করে।

যদি $R_E$ বাদ দেওয়া হয় (বা সরাসরি গ্রাউন্ড করা হয়), তবে এমিটারগুলোর মধ্যে সংযোগ বিচ্ছিন্ন হয়ে যায়। এর ফলে সার্কিটটি তার পজিটিভ ফিডব্যাক লুপ এবং হিস্টেরেসিস বৈশিষ্ট্য পুরোপুরি হারিয়ে ফেলে। এটি তখন আর শ্মিট ট্রিগার হিসেবে কাজ করে না, বরং নয়েজ ইমিউনিটি বিহীন একটি সাধারণ হাই-গেইন এমপ্লিফায়ার বা বেসিক কম্পারেটরের মতো আচরণ করে।

## B.Sc. (Hons) Part-IV Examination - 2021

### 2. (a) What is multivibrator? Describe the construction and working principle of a monostable multivibrator and mention its uses.

#### Circuit Diagram (Monostable Multivibrator):

Plaintext

```
           + VCC
             |
       +-----+-----+-----+
       |           |     |
     [Rc1]       [Rc2]  [R]
       |           |     |
       +---||------+-----+
       |   C       |     |
       |           |     |
       +-[R1]-+    |     |
       |      |    |     |
     |/       |  |/      |
(Trig)Q1      +--|Q2     |
     |\          |\      |
       |           |     |
      GND         GND   GND
```

#### English Answer:

**Multivibrator:** A multivibrator is an electronic circuit consisting of two amplifying devices (like transistors) cross-coupled by resistors and capacitors. It is used to implement two-state systems such as oscillators, timers, and flip-flops.

**Construction of Monostable Multivibrator:**

It consists of two NPN transistors, $Q_1$ and $Q_2$. The collector of $Q_1$ is capacitively coupled (via capacitor $C$) to the base of $Q_2$. The collector of $Q_2$ is resistively coupled (via resistor $R_1$) to the base of $Q_1$. The base of $Q_2$ is connected to $V_{CC}$ through a timing resistor $R$. This establishes the stable state where $Q_2$ is normally ON (biased by $R$) and $Q_1$ is normally OFF.

**Working Principle:**

1. **Stable State:** $Q_2$ receives base bias through $R$ and is fully ON. Its collector voltage is low ($0\text{ V}$), keeping $Q_1$ OFF. Capacitor $C$ charges to approximately $V_{CC}$.
    
2. **Quasi-Stable State:** When an external positive trigger pulse is applied to the base of $Q_1$, $Q_1$ turns ON. Its collector voltage drops to $0\text{ V}$. This negative voltage transition is transferred through capacitor $C$ to the base of $Q_2$, driving $Q_2$ OFF. The collector voltage of $Q_2$ rises to $V_{CC}$, which reinforces $Q_1$ to stay ON.
    
3. **Recovery:** Capacitor $C$ now begins to discharge and recharge in the reverse direction through resistor $R$ toward $V_{CC}$. Once the base voltage of $Q_2$ reaches approximately $+0.7\text{ V}$, $Q_2$ turns back ON. This drops its collector voltage, turning $Q_1$ OFF and returning the circuit to its original stable state. The duration of the quasi-stable state (pulse width) is given by $T = 0.69 RC$.
    

**Uses:**

Used as delay circuits, pulse stretchers, timer circuits, and to generate uniform output pulses from irregular input pulses (pulse shaping).

#### বাংলা উত্তর:

**মাল্টিভাইব্রেটর:** মাল্টিভাইব্রেটর হলো দুটি এমপ্লিফায়িং ডিভাইস (যেমন ট্রানজিস্টর) দ্বারা গঠিত এমন একটি সার্কিট, যা রোধ ও ধারকের মাধ্যমে ক্রস-কাপলড থাকে এবং এটি অসিলেটর, টাইমার বা ফ্লিপ-ফ্লপ হিসেবে দুই-অবস্থা বিশিষ্ট সিস্টেমে ব্যবহৃত হয়।

**মনোস্টেবল মাল্টিভাইব্রেটরের গঠন:**

এতে $Q_1$ এবং $Q_2$ নামক দুটি NPN ট্রানজিস্টর থাকে। $Q_1$-এর কালেক্টর একটি ক্যাপাসিটর ($C$)-এর মাধ্যমে $Q_2$-এর বেসের সাথে যুক্ত থাকে। আর $Q_2$-এর কালেক্টর রোধ ($R_1$)-এর মাধ্যমে $Q_1$-এর বেসের সাথে যুক্ত থাকে। $Q_2$-এর বেস টাইমিং রোধ $R$-এর মাধ্যমে $V_{CC}$-এর সাথে যুক্ত থাকে, যা নিশ্চিত করে যে সাধারণ অবস্থায় $Q_2$ অন এবং $Q_1$ অফ থাকবে (এটি এর স্থায়ী অবস্থা)।

**কার্যনীতি:**

১. **স্থায়ী অবস্থা:** $R$-এর মাধ্যমে বায়াস পেয়ে $Q_2$ সম্পূর্ণ অন থাকে। এর কালেক্টর ভোল্টেজ কম হওয়ায় $Q_1$ অফ থাকে। এসময় ক্যাপাসিটর $C$ প্রায় $V_{CC}$ মানে চার্জ হয়।

২. **অস্থায়ী অবস্থা:** $Q_1$-এর বেসে বাহ্যিক পজিটিভ ট্রিগার পালস দেওয়া হলে এটি অন হয়। ফলে এর কালেক্টর ভোল্টেজ $0\text{ V}$-এ নেমে যায়। এই নেগেটিভ ভোল্টেজ ড্রপ $C$-এর মাধ্যমে $Q_2$-এর বেসে পৌঁছায় এবং $Q_2$-কে অফ করে দেয়। $Q_2$ অফ হলে এর কালেক্টর ভোল্টেজ বেড়ে যায় যা $Q_1$-কে অন থাকতে সাহায্য করে।

৩. **পুনরুদ্ধার:** এ অবস্থায় ক্যাপাসিটর $C$, রোধ $R$-এর মাধ্যমে ডিসচার্জ হয়ে বিপরীত দিকে চার্জ হতে থাকে। $Q_2$-এর বেস ভোল্টেজ $+0.7\text{ V}$-এ পৌঁছালে এটি পুনরায় অন হয় এবং $Q_1$-কে অফ করে সার্কিটকে তার স্থায়ী অবস্থায় ফিরিয়ে আনে। এই পালসের সময়কাল হলো $T = 0.69 RC$।

**ব্যবহার:**

ডিলে সার্কিট, পালস স্ট্রেচার, টাইমার এবং অনিয়মিত সিগন্যাল থেকে সুষম পালস তৈরিতে ব্যবহৃত হয়।

### 2. (b) Find an expression for switching time and frequency of oscillation of an astable multivibrator.

#### English Answer:

Let the astable multivibrator have timing components $R_1, C_1$ connected to the base of $Q_2$ and $R_2, C_2$ connected to the base of $Q_1$.

**1. Switching Time (Pulse Width):**

During the quasi-stable state when $Q_2$ is OFF, the capacitor $C_1$ charges through $R_1$ towards $+V_{CC}$. The initial voltage across the capacitor is approximately $-V_{CC}$ (due to the sudden switching drop) and it aims for $+V_{CC}$. The transistor $Q_2$ will turn ON when the capacitor voltage reaches $V_{BE(sat)} \approx 0\text{ V}$.

The general voltage equation for a charging capacitor is:

$$V_c(t) = V_{\text{final}} - (V_{\text{final}} - V_{\text{initial}}) e^{-t / \tau}$$

Substituting $V_{\text{final}} = V_{CC}$, $V_{\text{initial}} = -V_{CC}$, $\tau = R_1 C_1$, and setting $V_c(t) = 0$ for the switching instant:

$$0 = V_{CC} - (V_{CC} - (-V_{CC})) e^{-t / R_1 C_1}$$

$$0 = V_{CC} - 2V_{CC} e^{-t / R_1 C_1}$$

$$e^{-t / R_1 C_1} = 0.5$$

Taking the natural logarithm on both sides:

$$\frac{-t}{R_1 C_1} = \ln(0.5) = -0.693$$

Therefore, the time $T_1$ (duration $Q_2$ is OFF) is:

$$T_1 = 0.693 R_1 C_1$$

Similarly, the time $T_2$ (duration $Q_1$ is OFF) is:

$$T_2 = 0.693 R_2 C_2$$

**2. Frequency of Oscillation:**

The total period is $T = T_1 + T_2 = 0.693(R_1 C_1 + R_2 C_2)$.

For a symmetrical astable multivibrator ($R_1 = R_2 = R$ and $C_1 = C_2 = C$), the period becomes:

$$T = 1.38 RC$$

The frequency $f$ is:

$$f = \frac{1}{T} = \frac{1}{1.38 RC}$$

#### বাংলা উত্তর:

ধরি, অ্যাস্টেবল মাল্টিভাইব্রেটরের $Q_1$ এবং $Q_2$ ট্রানজিস্টরের বেসের সাথে যুক্ত টাইমিং উপাদানগুলো যথাক্রমে $R_2, C_2$ এবং $R_1, C_1$।

**১. সুইচিং টাইম (পালসের সময়কাল):**

যখন $Q_2$ অফ থাকে, তখন ক্যাপাসিটর $C_1$, রোধ $R_1$-এর মাধ্যমে $+V_{CC}$-এর দিকে চার্জ হতে থাকে। ক্যাপাসিটরের প্রাথমিক ভোল্টেজ থাকে $-V_{CC}$ এবং এটি $+V_{CC}$-এর দিকে চার্জ হয়। ট্রানজিস্টর অন হওয়ার জন্য টার্গেট ভোল্টেজ হলো প্রায় $0\text{ V}$।

ক্যাপাসিটরের চার্জিং সমীকরণ হলো:

$$V_c(t) = V_{\text{final}} - (V_{\text{final}} - V_{\text{initial}}) e^{-t/RC}$$

মান বসিয়ে পাই:

$$0 = V_{CC} - (V_{CC} - (-V_{CC})) e^{-t / R_1 C_1}$$

$$0 = V_{CC} - 2V_{CC} e^{-t / R_1 C_1}$$

$$e^{-t / R_1 C_1} = 0.5$$

উভয়পক্ষে $\ln$ নিয়ে পাই:

$$\frac{t}{R_1 C_1} = -\ln(0.5) = 0.693$$

সুতরাং, $Q_2$ অফ থাকার সময়:

$$T_1 = 0.693 R_1 C_1$$

একইভাবে, $Q_1$ অফ থাকার সময়:

$$T_2 = 0.693 R_2 C_2$$

**২. কম্পাঙ্ক (Frequency):**

মোট পর্যায়কাল $T = T_1 + T_2 = 0.693(R_1 C_1 + R_2 C_2)$।

সুষম মাল্টিভাইব্রেটরের ক্ষেত্রে ($R_1 = R_2 = R$ এবং $C_1 = C_2 = C$), $T = 1.38 RC$।

কম্পাঙ্ক

$$f = \frac{1}{T} = \frac{1}{1.38 RC}$$

### 2. (c) Find the time period, duty cycle and the frequency of an astable multivibrator when $R_1 = 20\text{ k}\Omega$, $R_2 = 30\text{ k}\Omega$ and $C_1 = C_2 = C = 0.01\ \mu\text{F}$.

#### English Answer:

**Given:**

- $R_1 = 20\text{ k}\Omega = 20 \times 10^3\ \Omega$
    
- $R_2 = 30\text{ k}\Omega = 30 \times 10^3\ \Omega$
    
- $C_1 = C_2 = 0.01\ \mu\text{F} = 0.01 \times 10^{-6}\text{ F}$
    

**Calculation:**

**1. Time Period ($T$):**

$$T_1 = 0.693 R_1 C_1 = 0.693 \times 20 \times 10^3 \times 0.01 \times 10^{-6} = 138.6 \times 10^{-6}\text{ s} = 138.6\ \mu\text{s}$$

$$T_2 = 0.693 R_2 C_2 = 0.693 \times 30 \times 10^3 \times 0.01 \times 10^{-6} = 207.9 \times 10^{-6}\text{ s} = 207.9\ \mu\text{s}$$

Total Period $T = T_1 + T_2 = 138.6\ \mu\text{s} + 207.9\ \mu\text{s} = 346.5\ \mu\text{s}$

**2. Duty Cycle ($D$):**

Assuming $T_1$ represents the active HIGH state (pulse width):

$$D = \left(\frac{T_1}{T}\right) \times 100\% = \left(\frac{138.6}{346.5}\right) \times 100\% = 40\%$$

_(If $T_2$ is considered the active state, $D = 60\%$)_.

**3. Frequency ($f$):**

$$f = \frac{1}{T} = \frac{1}{346.5 \times 10^{-6}\text{ s}} \approx 2886\text{ Hz} \approx 2.886\text{ kHz}$$

#### বাংলা সমাধান:

**১. পর্যায়কাল ($T$):**

$T_1 = 0.693 \times 20\text{ k}\Omega \times 0.01\ \mu\text{F} = 138.6\ \mu\text{s}$

$T_2 = 0.693 \times 30\text{ k}\Omega \times 0.01\ \mu\text{F} = 207.9\ \mu\text{s}$

মোট পর্যায়কাল $T = 138.6 + 207.9 = 346.5\ \mu\text{s}$

**২. ডিউটি সাইকেল ($D$):**

ধরি $T_1$ হলো HIGH অবস্থা:

$D = \frac{138.6}{346.5} \times 100\% = 40\%$

**৩. কম্পাঙ্ক ($f$):**

$f = \frac{1}{346.5 \times 10^{-6}} \approx 2886\text{ Hz} \approx 2.886\text{ kHz}$

### 2. (d) Draw the Schmitt trigger circuit and sketch its output response for triangular input signal.

#### Circuit Diagram:

Plaintext

```
           + VCC
             |
       +-----+-----+-------+
       |           |       |
     [Rc1]       [Rc2]     |
       |           |       |
       +---[R1]----+--o Vout
       |           |
       |           |
     |/          |/
 Vin-|Q1         |Q2
     |\          |\
       |           |
       +-----+-----+
             |
            [Re]
             |
            GND
```

#### Output Response Sketch:

Plaintext

```
Input (Triangular Wave)
        UTP--.      .       .
            / \    / \     /
           /   \  /   \   /
        LTP-    .-     .-
          /      \    /
         .        .  .

Output (Square Wave)
 Vout_H +----+    +----+
        |    |    |    |
        |    |    |    |
 Vout_L +    +----+    +----
```

#### English Answer:

- **Circuit Description:** A basic transistor Schmitt trigger consists of two NPN transistors sharing a common emitter resistor $R_e$. The input is applied to the base of $Q_1$, and the collector of $Q_1$ is coupled to the base of $Q_2$. The output is typically taken from the collector of $Q_2$.
    
- **Output Response:** When a smooth rising triangular wave crosses the Upper Trigger Point (UTP), the output abruptly snaps to its opposite state (e.g., LOW for an inverting trigger, or HIGH for a non-inverting one). When the input falls back down and crosses the Lower Trigger Point (LTP), the output snaps back to its initial state. The result is a sharp rectangular/square wave.
    

#### বাংলা উত্তর:

- **সার্কিটের বর্ণনা:** একটি সাধারণ শ্মিট ট্রিগারে দুটি NPN ট্রানজিস্টর থাকে যাদের এমিটারগুলো একটি সাধারণ রোধ $R_e$-এর মাধ্যমে গ্রাউন্ডে যুক্ত থাকে। ইনপুট $Q_1$-এর বেসে দেওয়া হয় এবং $Q_1$-এর কালেক্টর $Q_2$-এর বেসের সাথে যুক্ত থাকে। আউটপুট $Q_2$-এর কালেক্টর থেকে নেওয়া হয়।
    
- **আউটপুট রেসপন্স:** ইনপুট হিসেবে ট্রায়াঙ্গুলার ওয়েভ দেওয়া হলে, যখন ইনপুট ভোল্টেজ বাড়তে বাড়তে আপার ট্রিগার পয়েন্ট (UTP) অতিক্রম করে, তখন আউটপুট খুব দ্রুত তার অবস্থার পরিবর্তন করে। আবার ইনপুট ভোল্টেজ কমতে কমতে লোয়ার ট্রিগার পয়েন্ট (LTP) অতিক্রম করলে আউটপুট আগের অবস্থায় ফিরে আসে। এর ফলে আউটপুটে একটি তীক্ষ্ণ বর্গাকার বা আয়তাকার তরঙ্গ পাওয়া যায়।
    

## B.Sc. (Hons) Part-IV Examination - 2020

### 2. (a) What are the basic differences among stable, monostable and bistable multivibrators?

_(Note: "stable" in the question paper is a typo for "astable")._

_(This question is identical to the solution provided in 2022 2(a). Please refer to 2022 2(a) for the detailed English and Bengali answer)._

### 2. (b) Describe the principal operation of a fixed bias transistor binary using necessary diagrams.

_(This question is identical to the solution provided in 2022 2(b). Please refer to 2022 2(b) for the detailed English and Bengali answer)._

### 2. (c) Why is the hysteresis desirable in a squaring circuit? Explain how Schmitt trigger circuit can be used for noise reduction.

#### English Answer:

- **Why Hysteresis is Desirable:** A squaring circuit converts a slowly varying signal (like a sine or triangle wave) into a sharp square wave. Hysteresis ensures that the circuit has two separate thresholds (UTP and LTP) for turning ON and OFF. This prevents the circuit from responding to unwanted high-frequency noise or minute ripples that often ride on the main signal.
    
- **Noise Reduction using Schmitt Trigger:** In a standard comparator without hysteresis, if the input signal has noise near the threshold voltage, the output will rapidly switch back and forth ("chatter"). A Schmitt trigger solves this. Once the signal crosses the UTP, the output switches. Even if noise causes the signal to dip slightly, it will not switch back unless it falls all the way past the LTP. The gap between UTP and LTP acts as a "dead zone" for noise, ensuring smooth, single-transition clean output waves.
    

#### বাংলা উত্তর:

- **স্কোয়ারিং সার্কিটে হিস্টেরেসিস কেন প্রয়োজন:** স্কোয়ারিং সার্কিট একটি ধীরগতির সিগন্যালকে (যেমন সাইন ওয়েভ) তীক্ষ্ণ স্কয়ার ওয়েভে পরিণত করে। হিস্টেরেসিস থাকার ফলে সার্কিটের অন এবং অফ হওয়ার জন্য দুটি আলাদা থ্রেশহোল্ড (UTP এবং LTP) থাকে। এটি মূল সিগন্যালের সাথে থাকা অনাকাঙ্ক্ষিত নয়েজ বা ছোট ছোট ভোল্টেজ পরিবর্তনকে আউটপুটে প্রভাব ফেলতে বাধা দেয়।
    
- **নয়েজ কমানোর জন্য শ্মিট ট্রিগারের ব্যবহার:** হিস্টেরেসিস ছাড়া একটি সাধারণ কম্পারেটরে, ইনপুট সিগন্যালে নয়েজ থাকলে আউটপুট বারবার অন-অফ হতে পারে (যাকে চ্যাটারিং বলে)। শ্মিট ট্রিগার এই সমস্যার সমাধান করে। সিগন্যাল একবার UTP অতিক্রম করলে আউটপুট পরিবর্তন হয়। এরপর নয়েজের কারণে সিগন্যাল কিছুটা কমে গেলেও আউটপুট আগের অবস্থায় ফেরে না, যতক্ষণ না তা LTP-এর নিচে নামে। UTP এবং LTP এর মাঝখানের এই গ্যাপটি নয়েজের জন্য একটি "ডেড জোন" হিসেবে কাজ করে, যা একটি পরিষ্কার এবং নিখুঁত আউটপুট তরঙ্গ নিশ্চিত করে।
    

## B.Sc. (Hons) Part-IV Examination - 2019

### 2. (a) What are the basic differences among relaxation oscillators?

_(This question is identical to 2022 2(a) and 2020 2(a). Relaxation oscillators include astable, monostable, and bistable multivibrators. Please refer to 2022 2(a) for the detailed answer)._

### 2. (b) Explain the working principles of a symmetrical astable multivibrator and draw its output waveforms.

_(This question is identical to 2023 2(b). Please refer to 2023 2(b) for the detailed English and Bengali explanation and circuit/waveforms)._

### 2. (c) What is a blocking oscillator? Mention some of its uses.

#### English Answer:

- **Blocking Oscillator:** A blocking oscillator is a relaxation oscillator that relies on a single transistor and heavy inductive positive feedback via a pulse transformer. It is characterized by generating an extremely narrow, high-power sharp pulse, followed by a long, deep cut-off (blocking) period during which the base capacitor discharges.
    
- **Uses:**
    
    1. Used as a pulse generator to produce very sharp, narrow, and high-power pulses.
        
    2. Used in radar and television circuits for sweep/time-base generation.
        
    3. Used as a trigger source for other synchronization circuits.
        
    4. Used in frequency division circuits.
        

#### বাংলা উত্তর:

- **ব্লকিং অসিলেটর:** ব্লকিং অসিলেটর হলো এক ধরনের রিলাক্সেশন অসিলেটর যা একটিমাত্র ট্রানজিস্টর এবং একটি পালস ট্রান্সফর্মারের মাধ্যমে শক্তিশালী ইনডাকটিভ পজিটিভ ফিডব্যাক ব্যবহার করে। এটি অত্যন্ত সরু এবং উচ্চ-ক্ষমতার তীক্ষ্ণ পালস তৈরি করে, যার পর একটি দীর্ঘ কাট-অফ বা ব্লকিং পিরিয়ড থাকে যখন বেস ক্যাপাসিটর ডিসচার্জ হয়।
    
- **ব্যবহার:**
    
    ১. খুব সরু, তীক্ষ্ণ এবং উচ্চ-ক্ষমতার পালস তৈরির জন্য পালস জেনারেটর হিসেবে।
    
    ২. রাডার এবং টেলিভিশনের সার্কিটে সুইপ বা টাইম-বেস তৈরিতে।
    
    ৩. অন্যান্য সিনক্রোনাইজেশন সার্কিটে ট্রিগার সোর্স হিসেবে।
    
    ৪. ফ্রিকোয়েন্সি ডিভিশন সার্কিটে এটি ব্যবহৃত হয়।