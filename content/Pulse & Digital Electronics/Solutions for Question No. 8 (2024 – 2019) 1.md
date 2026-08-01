## B.Sc. (Hons) Part-IV Examination - 2024

### 8. Write short notes on (any four):

#### a) Magnetic disc

**English:** A magnetic disk is a non-volatile storage device that uses magnetization to store digital data. It consists of circular platters coated with a magnetic material. Data is read and written using read/write heads that hover just above the spinning platters. The disk surface is logically divided into concentric circles called _tracks_, which are further divided into _sectors_. Data is stored as microscopic magnetized regions representing binary 1s and 0s. It provides massive storage capacity and allows for direct (random) access to data, making it widely used as hard disk drives (HDDs) in computer systems.

**Bangla:** ম্যাগনেটিক ডিস্ক হলো একটি নন-ভোলাটাইল স্টোরেজ ডিভাইস যা ডেটা সংরক্ষণের জন্য চৌম্বকত্ব ব্যবহার করে। এতে গোলাকার প্ল্যাটার থাকে যার ওপর চৌম্বকীয় পদার্থের প্রলেপ থাকে। ঘূর্ণায়মান প্ল্যাটারের উপর থাকা রিড/রাইট হেডের সাহায্যে ডেটা পড়া ও লেখা হয়। ডিস্কের পৃষ্ঠকে যৌক্তিকভাবে 'ট্র্যাক' নামক সমকেন্দ্রিক বৃত্তে এবং এরপর 'সেক্টর'-এ ভাগ করা হয়। ডেটাগুলো মাইক্রোস্কোপিক চৌম্বকীয় অঞ্চল হিসেবে লজিক ১ ও ০ আকারে সংরক্ষিত থাকে। এর স্টোরেজ ক্ষমতা অনেক বেশি এবং সরাসরি ডেটা অ্যাক্সেস করা যায় বলে কম্পিউটার সিস্টেমে হার্ড ডিস্ক (HDD) হিসেবে এর ব্যাপক ব্যবহার রয়েছে।

#### b) Digital recording technique

**English:** Digital recording is the process of converting continuous analog signals (like sound, music, or video) into a stream of discrete digital numbers (0s and 1s) and storing them on a magnetic, optical, or solid-state medium. The process involves sampling the analog signal at regular intervals and quantizing its amplitude into binary values using an Analog-to-Digital Converter (ADC). During playback, a Digital-to-Analog Converter (DAC) reconstructs the original analog signal. The primary advantage is high fidelity and immunity to noise; digital data can be copied endlessly without any degradation in quality.

**Bangla:** ডিজিটাল রেকর্ডিং হলো এমন একটি প্রক্রিয়া যেখানে নিরবচ্ছিন্ন অ্যানালগ সিগন্যালকে (যেমন- অডিও বা ভিডিও) ডিজিটালে (০ এবং ১) রূপান্তর করে ম্যাগনেটিক, অপটিক্যাল বা সলিড-স্টেট মাধ্যমে সংরক্ষণ করা হয়। এ প্রক্রিয়ায় অ্যানালগ সিগন্যালকে নির্দিষ্ট সময় পরপর স্যাম্পলিং করা হয় এবং অ্যানালগ-টু-ডিজিটাল কনভার্টার (ADC)-এর সাহায্যে বাইনারি মানে রূপান্তর করা হয়। প্লেব্যাক করার সময় ডিজিটাল-টু-অ্যানালগ কনভার্টার (DAC) পুনরায় মূল অ্যানালগ সিগন্যাল তৈরি করে। এর প্রধান সুবিধা হলো উচ্চ গুণমান এবং নয়েজ-মুক্ত হওয়া; গুণগত মান না কমিয়ে এর অসীম সংখ্যক কপি তৈরি করা যায়।

#### c) Clipping circuit

**English:** A clipping circuit (or clipper) is a non-linear wave-shaping circuit used to limit or "clip off" a specific portion of an input waveform without distorting the remaining part. It essentially limits the voltage level to a predetermined maximum or minimum value. Typically constructed using diodes and resistors, clippers can be positive (removing the positive peak), negative (removing the negative peak), or biased (removing portions above or below a specific reference DC voltage). They are widely used in FM transmitters to remove noise peaks, in TV receivers, and for component protection.

Plaintext

```
       R
 In o--[ ]--+-------o Out (Clipped Signal)
            |
           --- Diode (D)
           / \
           ---
            |
           GND
```

**Bangla:** ক্লিপিং সার্কিট (বা ক্লিপার) হলো একটি নন-লিনিয়ার ওয়েভশেপিং সার্কিট, যা ইনপুট তরঙ্গের বাকি অংশ অবিকৃত রেখে নির্দিষ্ট একটি অংশকে কেটে বাদ দেয় বা সীমিত করে। এটি মূলত ভোল্টেজ লেভেলকে একটি পূর্বনির্ধারিত সর্বোচ্চ বা সর্বনিম্ন মানে সীমাবদ্ধ রাখে। সাধারণত ডায়োড ও রেজিস্টর দিয়ে তৈরি ক্লিপারগুলো পজিটিভ (পজিটিভ অংশ কাটে), নেগেটিভ (নেগেটিভ অংশ কাটে) অথবা বায়াসড (একটি নির্দিষ্ট ডিসি ভোল্টেজের ওপর বা নিচের অংশ কাটে) হতে পারে। এগুলো এফএম (FM) ট্রান্সমিটারে নয়েজ কাটাতে, টিভি রিসিভারে এবং সার্কিটের সুরক্ষায় ব্যবহৃত হয়।

#### d) Shift register

**English:** A shift register is a sequential digital logic circuit primarily used for the storage and transfer of digital data. It is constructed by cascading a series of flip-flops (usually D-type) where the output of one flip-flop is connected to the input of the next. All flip-flops share a common clock signal, allowing data to shift one position to the left or right with each clock pulse. Shift registers are classified by their input/output methods: Serial-In Serial-Out (SISO), Serial-In Parallel-Out (SIPO), Parallel-In Serial-Out (PISO), and Parallel-In Parallel-Out (PIPO). They are heavily used in calculators, delay lines, and serial-to-parallel data conversion.

**Bangla:** শিফট রেজিস্টার হলো একটি সিকুয়েনশিয়াল ডিজিটাল লজিক সার্কিট, যা প্রধানত ডিজিটাল ডেটা সংরক্ষণ এবং স্থানান্তরের জন্য ব্যবহৃত হয়। এটি কয়েকটি ফ্লিপ-ফ্লপ (সাধারণত D টাইপ) সিরিজে যুক্ত করে তৈরি করা হয়, যেখানে একটির আউটপুট পরেরটির ইনপুটের সাথে যুক্ত থাকে। সব ফ্লিপ-ফ্লপে একটি কমন ক্লক সিগন্যাল থাকে, ফলে প্রতিটি ক্লক পালসে ডেটা ডানে বা বামে এক ঘর সরে যায় (Shift)। ডেটা ইনপুট ও আউটপুট পদ্ধতির ওপর ভিত্তি করে এটি ৪ প্রকার: SISO, SIPO, PISO এবং PIPO। এগুলো ক্যালকুলেটর, ডেটা ডিলে এবং সিরিয়াল-প্যারালাল ডেটা রূপান্তরে ব্যবহৃত হয়।

#### e) Active filter

**English:** An active filter is an electronic filter circuit that uses active components, such as operational amplifiers (op-amps), along with passive components like resistors ($R$) and capacitors ($C$) to filter out unwanted frequencies from a signal. Unlike passive filters, active filters do not use bulky and expensive inductors ($L$). The presence of the op-amp allows the filter to provide voltage gain, meaning the output signal can be amplified while being filtered. They offer high input impedance, low output impedance, and are easily tunable. Common types include Low-Pass, High-Pass, and Band-Pass active filters.

**Bangla:** অ্যাকটিভ ফিল্টার হলো এমন একটি ইলেকট্রনিক ফিল্টার সার্কিট, যা কোনো সিগন্যাল থেকে অনাকাঙ্ক্ষিত কম্পাঙ্ক দূর করতে প্যাসিভ উপাদান (রেজিস্টর ও ক্যাপাসিটর)-এর পাশাপাশি অ্যাকটিভ উপাদান, যেমন- অপারেশনাল এমপ্লিফায়ার (Op-amp) ব্যবহার করে। প্যাসিভ ফিল্টারের মতো এতে ভারী ও ব্যয়বহুল ইনডাক্টর ($L$) ব্যবহার করা হয় না। অপ-এম্প থাকায় এটি ভোল্টেজ গেইন প্রদান করতে পারে, অর্থাৎ ফিল্টার করার পাশাপাশি সিগন্যালকে বিবর্ধিতও করতে পারে। এর ইনপুট ইম্পিডেন্স বেশি এবং আউটপুট ইম্পিডেন্স কম হয়। অডিও প্রসেসিং এবং কমিউনিকেশন সিস্টেমে লো-পাস, হাই-পাস এবং ব্যান্ড-পাস অ্যাকটিভ ফিল্টারের ব্যাপক ব্যবহার রয়েছে।

## B.Sc. (Hons) Part-IV Examination - 2023

### 8. Write short notes on (any four):

#### a) Clamping circuit

**English:** A clamping circuit (or clamper) is a non-linear wave-shaping circuit that adds a DC offset voltage to an AC signal, shifting the entire waveform upward or downward without altering its original shape or peak-to-peak amplitude. Also known as a DC restorer, it typically consists of a capacitor, a diode, and a resistor. The capacitor charges to the peak voltage during the forward-biased state of the diode and subsequently acts as a battery, adding a DC level to the input signal. Clampers are categorized as positive clampers (shifting the wave above 0V) and negative clampers (shifting the wave below 0V).

Plaintext

```
          C
 In o----||----+-------o Out (Clamped Signal)
               |
              --- Diode (D)
              / \
              ---
               |
              GND
```

**Bangla:** ক্ল্যাম্পিং সার্কিট (বা ক্ল্যাম্পার) হলো একটি নন-লিনিয়ার ওয়েভশেপিং সার্কিট, যা ইনপুট এসি সিগন্যালের সাথে একটি নির্দিষ্ট ডিসি (DC) ভোল্টেজ যোগ করে সিগন্যালের মূল আকৃতি বা বিস্তার (peak-to-peak amplitude) পরিবর্তন না করেই তাকে উপরে বা নিচে স্থানান্তরিত করে। একে 'ডিসি রিস্টোরার'ও বলা হয়। এটি সাধারণত ক্যাপাসিটর, ডায়োড এবং রেজিস্টর দিয়ে তৈরি হয়। ডায়োডটি যখন ফরওয়ার্ড বায়াসড থাকে তখন ক্যাপাসিটরটি চার্জ হয় এবং পরবর্তীতে একটি ব্যাটারির মতো কাজ করে ইনপুটের সাথে ডিসি লেভেল যোগ করে। এটি পজিটিভ ক্ল্যাম্পার (তরঙ্গকে পজিটিভ দিকে তোলে) এবং নেগেটিভ ক্ল্যাম্পার (তরঙ্গকে নেগেটিভ দিকে নামায়) হতে পারে।

#### b) Industrial fabrication steps of IC

**English:** The fabrication of monolithic Integrated Circuits (ICs) involves complex chemical and photo-lithographic processes to build interconnected electronic components on a single silicon chip. The primary steps include:

1. **Wafer Preparation:** Growing a pure silicon crystal and slicing it into thin wafers.
    
2. **Epitaxial Growth:** Depositing a thin N-type silicon layer on a P-type substrate.
    
3. **Oxidation:** Growing a protective Silicon Dioxide ($SiO_2$) layer over the wafer.
    
4. **Photolithography:** Using UV light and photoresist to etch specific "windows" in the $SiO_2$ layer.
    
5. **Diffusion/Ion Implantation:** Adding P-type or N-type impurities through the windows to form transistors and diodes.
    
6. **Metallization:** Depositing a thin layer of aluminum to electrically interconnect the components.
    
7. **Packaging:** Cutting the wafer into individual dies and encapsulating them in plastic or ceramic packages.
    

**Bangla:** মনোলিথিক ইন্টিগ্রেটেড সার্কিট (IC) তৈরির জন্য একটিমাত্র সিলিকন চিপের ওপর রাসায়নিক এবং ফটোলিথোগ্রাফিক প্রক্রিয়ার মাধ্যমে ইলেকট্রনিক উপাদানগুলো তৈরি করা হয়। এর প্রধান ধাপগুলো হলো:

১. **ওয়েফার প্রস্তুতি:** বিশুদ্ধ সিলিকন ক্রিস্টাল তৈরি করে তা পাতলা চাকতি বা ওয়েফারে কাটা।

২. **এপিট্যাক্সিয়াল গ্রোথ:** P-টাইপ সাবস্ট্রেটের ওপর একটি পাতলা N-টাইপ সিলিকন স্তর তৈরি।

৩. **অক্সিডেশন:** ওয়েফারের ওপর সিলিকন ডাই-অক্সাইডের ($SiO_2$) একটি সুরক্ষামূলক স্তর তৈরি করা।

৪. **ফটোলিথোগ্রাফি:** অতিবেগুনি রশ্মি ব্যবহার করে $SiO_2$ স্তরে রাসায়নিকভাবে ছোট ছোট জানালা বা উইন্ডো তৈরি করা।

৫. **ডিফিউশন বা আয়ন ইমপ্লান্টেশন:** এই উইন্ডোগুলোর ভেতর দিয়ে নির্দিষ্ট ভেজাল (P বা N টাইপ) প্রবেশ করিয়ে ট্রানজিস্টর ও ডায়োড তৈরি করা।

৬. **মেটালাইজেশন:** উপাদানগুলোর মধ্যে বৈদ্যুতিক সংযোগ স্থাপনের জন্য অ্যালুমিনিয়ামের প্রলেপ দেওয়া।

৭. **প্যাকেজিং:** ওয়েফার কেটে আলাদা চিপ তৈরি করে প্লাস্টিক বা সিরামিকের প্যাকেজে আবদ্ধ করা।

#### c) Blocking oscillator

**English:** A blocking oscillator is a type of relaxation oscillator that uses a single amplifying active device (like a transistor) and relies heavily on inductive positive feedback through a pulse transformer. The circuit generates very narrow, sharp, high-power pulses followed by a relatively long "resting" or "blocked" (cut-off) period. During the ON period, the transformer provides regenerative feedback driving the transistor into deep saturation. Once the base capacitor charges fully or the transformer core saturates, the transistor rapidly cuts off, remaining blocked while the capacitor discharges. They are widely used as pulse generators, trigger sources, and in early CRT television sweep circuits.

**Bangla:** ব্লকিং অসিলেটর হলো এক ধরনের রিলাক্সেশন অসিলেটর, যা একটিমাত্র ট্রানজিস্টর এবং পালস ট্রান্সফর্মারের মাধ্যমে শক্তিশালী ইনডাকটিভ পজিটিভ ফিডব্যাক ব্যবহার করে কাজ করে। এই সার্কিটটি অত্যন্ত সরু এবং উচ্চ-ক্ষমতার পালস তৈরি করে, যার পর দীর্ঘ একটি কাট-অফ বা ব্লকিং (বিশ্রাম) সময় থাকে। ট্রানজিস্টরটি চালু হলে ট্রান্সফর্মারটি রিজেনারেটিভ ফিডব্যাক প্রদান করে একে দ্রুত স্যাচুরেশনে নিয়ে যায়। বেসের ক্যাপাসিটর পুরোপুরি চার্জ হলে বা ট্রান্সফর্মার স্যাচুরেটেড হলে ট্রানজিস্টরটি দ্রুত বন্ধ (Cut-off) হয়ে যায় এবং ক্যাপাসিটর ডিসচার্জ না হওয়া পর্যন্ত ব্লকড থাকে। এটি পালস জেনারেটর, ট্রিগার সোর্স এবং সিআরটি টিভির সুইপ সার্কিটে ব্যবহৃত হয়।

#### d) Static and dynamic memories

**English:** Semiconductor Random Access Memory (RAM) is classified into two main types: Static RAM (SRAM) and Dynamic RAM (DRAM).

- **SRAM (Static RAM):** Uses flip-flop circuits (cross-coupled inverters) to store each bit of data. It holds data indefinitely as long as power is applied without needing to be refreshed. SRAM is very fast and is typically used for CPU cache memory, but it is expensive and takes up more physical space per bit.
    
- **DRAM (Dynamic RAM):** Stores each bit of data as an electrical charge on a microscopic capacitor paired with a single transistor. Because capacitors slowly leak charge, DRAM requires continuous "refreshing" (reading and rewriting the data) thousands of times per second. DRAM is slower than SRAM but has a much higher storage density and lower cost, making it the standard choice for computer main memory.
    

**Bangla:** সেমিকন্ডাক্টর র‍্যাম (RAM) প্রধানত দুই প্রকার: স্ট্যাটিক র‍্যাম (SRAM) এবং ডাইনামিক র‍্যাম (DRAM)।

- **SRAM (স্ট্যাটিক র‍্যাম):** এটি ডেটা সংরক্ষণের জন্য ফ্লিপ-ফ্লপ সার্কিট ব্যবহার করে। বিদ্যুৎ সরবরাহ থাকা পর্যন্ত এটি ডেটা ধরে রাখে এবং কোনো রিফ্রেশের প্রয়োজন হয় না। এটি অত্যন্ত দ্রুতগতির এবং সাধারণত প্রসেসরের ক্যাশ মেমরি হিসেবে ব্যবহৃত হয়। তবে এটি বেশ ব্যয়বহুল এবং বেশি জায়গা নেয়।
    
- **DRAM (ডাইনামিক র‍্যাম):** এটি একটি অতি ক্ষুদ্র ক্যাপাসিটর এবং একটি ট্রানজিস্টরের সাহায্যে বৈদ্যুতিক চার্জ হিসেবে ডেটা সংরক্ষণ করে। ক্যাপাসিটর থেকে ধীরে ধীরে চার্জ লিক হয়ে যায় বলে একে প্রতি সেকেন্ডে হাজার হাজার বার "রিফ্রেশ" (পুনরায় চার্জ) করতে হয়। এটি SRAM-এর তুলনায় ধীরগতির হলেও এর ডেটা ধারণক্ষমতা অনেক বেশি এবং দাম কম হওয়ায় কম্পিউটারের প্রধান মেমরি হিসেবে এটি সর্বাধিক ব্যবহৃত হয়।
    

#### e) Digital recording technique

_(Please refer to the detailed answer in **2024 - 8(b)** for both English and Bangla explanations.)_

## B.Sc. (Hons) Part-IV Examination - 2022

### 8. Write short notes on (any four):

#### (a) Active filter

_(Please refer to the detailed answer in **2024 - 8(e)** for both English and Bangla explanations.)_

#### (b) SRAM and EPROM

**English:**

- **SRAM (Static Random Access Memory):** A volatile memory that uses bi-stable latching circuitry (flip-flops) to store each bit. It does not need periodic refreshing. It is extremely fast and is widely used for CPU cache, but has lower density and higher cost compared to DRAM.
    
- **EPROM (Erasable Programmable Read-Only Memory):** A non-volatile memory chip that retains its data when its power supply is switched off. It uses floating-gate transistors to store electrons. It can be erased by exposing the semiconductor die to strong Ultraviolet (UV) light through a clear quartz window on the top of the package. After erasure, it can be reprogrammed using a specialized electronic device.
    

**Bangla:**

- **SRAM (স্ট্যাটিক র‍্যাম):** এটি একটি উদ্বায়ী (volatile) মেমরি যা ডেটা ধরে রাখতে ফ্লিপ-ফ্লপ ব্যবহার করে। এর কোনো রিফ্রেশের প্রয়োজন হয় না এবং এটি খুব দ্রুত কাজ করে, তাই ক্যাশ মেমরিতে এটি ব্যবহৃত হয়।
    
- **EPROM (ইপিউরম):** এটি এক প্রকার নন-ভোলাটাইল মেমরি যা বিদ্যুৎ চলে গেলেও ডেটা ধরে রাখে। এই চিপের ওপর একটি স্বচ্ছ কোয়ার্টজ উইন্ডো থাকে। শক্তিশালী অতিবেগুনি রশ্মি (UV light) প্রয়োগ করে এর ভেতরের ডেটা মুছে ফেলা যায় এবং এরপর বিশেষ ডিভাইসের সাহায্যে পুনরায় প্রোগ্রাম করা যায়। এটি ফ্লোটিং-গেট ট্রানজিস্টর ব্যবহার করে ইলেকট্রন আটকে রেখে ডেটা সংরক্ষণ করে।
    

#### (c) Blocking oscillator

_(Please refer to the detailed answer in **2023 - 8(c)** for both English and Bangla explanations.)_

#### (d) K-map

**English:** A Karnaugh map (K-map) is a graphical tool used in digital electronics to simplify Boolean algebra expressions without needing to manually apply complex Boolean theorems. It consists of a grid of cells, where each cell represents a specific minterm (or maxterm) of the logical variables. The rows and columns are arranged according to Gray code, ensuring that only one variable changes state between any two adjacent cells. To simplify a Boolean expression, 1s are placed in cells corresponding to the true outputs of a truth table. Adjacent 1s are then visually grouped into pairs, quads (groups of 4), or octets (groups of 8). These groupings cancel out redundant variables, yielding the simplest possible sum-of-products (SOP) expression for circuit design.

**Bangla:** কার্নফ ম্যাপ (K-map) হলো বুলিয়ান অ্যালজেবরার সমীকরণগুলোকে সহজ করার একটি গ্রাফিক্যাল পদ্ধতি, যেখানে জটিল বুলিয়ান উপপাদ্য মনে রাখার প্রয়োজন হয় না। এটি কয়েকটি ঘরের (cell) সমন্বয়ে গঠিত একটি ছক, যার প্রতিটি ঘর লজিক্যাল ভেরিয়েবলের একটি মিনটার্মকে নির্দেশ করে। এর সারি ও কলামগুলো গ্রে কোড (Gray code) অনুযায়ী সাজানো থাকে, ফলে পাশাপাশি দুটি ঘরের মধ্যে মাত্র একটি ভেরিয়েবলের পার্থক্য থাকে। সমীকরণ সরল করতে ট্রুথ টেবিলের ১-গুলোকে ম্যাপের নির্দিষ্ট ঘরে বসানো হয়। এরপর পাশাপাশি থাকা ১-গুলোকে জোড় (pair), কোয়াড (৪টি) বা অক্টেটে (৮টি) গ্রুপ করা হয়। এই গ্রুপিংয়ের ফলে অপ্রয়োজনীয় ভেরিয়েবলগুলো বাদ যায় এবং সার্কিট ডিজাইনের জন্য সবচেয়ে সরল বুলিয়ান সমীকরণ পাওয়া যায়।

#### (e) Digital voltmeter

**English:** A Digital Voltmeter (DVM) is an electronic measuring instrument that measures AC or DC voltage and displays the result directly as a discrete numerical value, typically on a 7-segment LED or LCD display. Unlike traditional analog voltmeters that use a moving mechanical pointer, DVMs use an Analog-to-Digital Converter (ADC), such as a dual-slope integrator or successive approximation converter, to translate the continuous input voltage into a digital code. This code is then processed by a microcontroller or decoding logic to drive the display. DVMs provide much higher accuracy, better resolution, and eliminate human reading errors (parallax errors).

**Bangla:** ডিজিটাল ভোল্টমিটার (DVM) হলো এমন একটি ইলেকট্রনিক পরিমাপক যন্ত্র যা এসি (AC) বা ডিসি (DC) ভোল্টেজ মেপে তার মান সরাসরি সংখ্যায় এলইডি (LED) বা এলসিডি (LCD) পর্দায় প্রদর্শন করে। অ্যানালগ ভোল্টমিটারের মতো কাঁটা (pointer) ব্যবহারের বদলে এটি অ্যানালগ-টু-ডিজিটাল কনভার্টার (ADC) (যেমন- ডুয়াল স্লোপ ইন্টিগ্রেটর) ব্যবহার করে ইনপুট ভোল্টেজকে ডিজিটাল কোডে রূপান্তর করে। এরপর ডিকোডিং লজিকের সাহায্যে তা পর্দায় দেখানো হয়। ডিজিটাল ভোল্টমিটার অনেক বেশি নিখুঁত, এর রেজোলিউশন ভালো এবং এতে মানুষের পাঠ নেওয়ার ভুল (প্যারালাক্স ত্রুটি) হওয়ার কোনো সম্ভাবনা থাকে না।

## B.Sc. (Hons) Part-IV Examination - 2021

### 8. Write short notes on (any four):

#### (a) Industrial fabrication steps of IC

_(Please refer to the detailed answer in **2023 - 8(b)** for both English and Bangla explanations.)_

#### (b) RAM and ROM

**English:** Memory in digital systems is broadly categorized into RAM and ROM.

- **RAM (Random Access Memory):** It is a volatile read/write memory, meaning it loses its stored data when power is turned off. Data can be accessed from any location in the same amount of time. It is used as the primary working memory for a computer to hold actively running programs and data. RAM is further divided into SRAM (Static) and DRAM (Dynamic).
    
- **ROM (Read-Only Memory):** It is a non-volatile memory, meaning it retains its data even without power. During normal operation, data can only be read from it, not written to it. ROM is used to store critical system instructions, such as the computer's BIOS or firmware. Variants include PROM, EPROM, and EEPROM.
    

**Bangla:** ডিজিটাল সিস্টেমে মেমরি প্রধানত RAM এবং ROM এই দুই ভাগে বিভক্ত।

- **RAM (র‍্যাম):** এটি একটি ভোলাটাইল বা উদ্বায়ী রিড/রাইট মেমরি, অর্থাৎ বিদ্যুৎ চলে গেলে এর ডেটা মুছে যায়। যেকোনো স্থান থেকে সমান সময়ে ডেটা অ্যাক্সেস করা যায়। কম্পিউটারে চলমান প্রোগ্রাম ও ডেটা রাখার জন্য প্রধান মেমরি হিসেবে এটি ব্যবহৃত হয়। এটি প্রধানত SRAM এবং DRAM এই দুই প্রকার।
    
- **ROM (রম):** এটি একটি নন-ভোলাটাইল বা অনুদ্বায়ী মেমরি, অর্থাৎ বিদ্যুৎ না থাকলেও এতে ডেটা সংরক্ষিত থাকে। সাধারণ ব্যবহারে এখান থেকে শুধু ডেটা পড়া (Read) যায়, লেখা যায় না। কম্পিউটারের বেসিক ইনপুট-আউটপুট সিস্টেম (BIOS) বা ফার্মওয়্যারের মতো স্থায়ী প্রোগ্রাম সংরক্ষণে রম ব্যবহৃত হয়। এর প্রকারভেদের মধ্যে রয়েছে PROM, EPROM এবং EEPROM।
    

#### (c) Magnetic disk

_(Please refer to the detailed answer in **2024 - 8(a)** for both English and Bangla explanations.)_

#### (d) Digital clock

**English:** A digital clock is a sequential digital system that displays the time of day using numerical indicators (like 7-segment LED or LCD displays) rather than analog mechanical hands. The core operation relies on a series of electronic digital counters. A highly accurate crystal oscillator generates a high-frequency base signal, which is divided down to exactly 1 pulse per second (1 Hz). This 1 Hz clock signal is fed into a MOD-60 counter to keep track of seconds (0-59). The output of the seconds counter triggers another MOD-60 counter for minutes (0-59). Finally, the minutes counter triggers a MOD-12 or MOD-24 counter to display the hours. Decoders convert the binary outputs of these counters to drive the display segments.

**Bangla:** ডিজিটাল ক্লক হলো একটি সিকুয়েনশিয়াল ডিজিটাল সার্কিট সিস্টেম, যা অ্যানালগ কাঁটার বদলে 7-সেগমেন্ট এলইডি (LED) বা এলসিডি (LCD) ব্যবহার করে সরাসরি সংখ্যায় সময় প্রদর্শন করে। এর মূল কার্যপ্রণালী বিভিন্ন কাউন্টারের (Counter) ওপর নির্ভরশীল। প্রথমে একটি ক্রিস্টাল অসিলেটর থেকে প্রাপ্ত উচ্চ কম্পাঙ্কের সিগন্যালকে ভাগ (frequency division) করে ঠিক ১ হার্জ (১ সেকেন্ডে ১টি পালস) সিগন্যাল তৈরি করা হয়। এই ১ হার্জ সিগন্যালটি সেকেন্ড গণনার জন্য একটি MOD-60 কাউন্টারে (০-৫৯) দেওয়া হয়। সেকেন্ডের কাউন্টার প্রতি ৬০ সেকেন্ড পর মিনিটের MOD-60 কাউন্টারকে ট্রিগার করে। একইভাবে মিনিটের কাউন্টারটি একটি MOD-12 বা MOD-24 আওয়ার (ঘণ্টা) কাউন্টারকে ট্রিগার করে। কাউন্টারগুলোর বাইনারি আউটপুটকে ডিকোডারের সাহায্যে পর্দায় দেখানো হয়।

#### (e) Digital recording technique

_(Please refer to the detailed answer in **2024 - 8(b)** for both English and Bangla explanations.)_

## B.Sc. (Hons) Part-IV Examination - 2020

### 8. Write short notes on (any four):

#### i) Pulse parameters

**English:** An ideal pulse transitions instantaneously between two voltage levels, but practical (non-ideal) pulses have specific geometric characteristics known as pulse parameters:

1. **Rise time ($t_r$):** The time required for the pulse amplitude to rise from 10% to 90% of its maximum steady amplitude.
    
2. **Fall time ($t_f$):** The time required for the pulse amplitude to fall from 90% to 10% of its amplitude.
    
3. **Pulse Width/Duration ($W$ or $t_p$):** The time interval between the 50% amplitude points on the leading and trailing edges.
    
4. **Sag or Droop:** The fractional drop in the pulse amplitude along its flat top over time.
    
5. **Overshoot & Ringing:** The transient voltage spike and subsequent oscillations extending above the maximum amplitude level immediately after the rising edge.
    

**Bangla:** একটি আদর্শ পালস তাৎক্ষণিকভাবে দুটি লেভেলের মধ্যে ওঠানামা করে, কিন্তু বাস্তব পালস তরঙ্গের কিছু জ্যামিতিক বৈশিষ্ট্য থাকে, যাদের পালস প্যারামিটার বলে:

১. **রাইজ টাইম ($t_r$):** পালসের বিস্তার সর্বোচ্চ মানের ১০% থেকে ৯০%-এ পৌঁছাতে যে সময় লাগে।

২. **ফল টাইম ($t_f$):** পালসের বিস্তার সর্বোচ্চ মানের ৯০% থেকে কমে ১০%-এ নামতে যে সময় লাগে।

৩. **পালস প্রস্থ ($W$ বা $t_p$):** পালসের অগ্রগামী ও পশ্চাৎগামী প্রান্তের ৫০% বিস্তার বিন্দুর মধ্যবর্তী সময়কাল।

৪. **স্যাগ বা ড্রুপ (Sag/Droop):** পালস চলাকালীন সময়ে ফ্ল্যাট শীর্ষভাগের ভোল্টেজের ক্রমশ হ্রাস পাওয়াকে স্যাগ বলে।

৫. **ওভারশুট এবং রিংগিং:** রাইজিং এজের ঠিক পরেই কাঙ্ক্ষিত লেভেলের উপরে ভোল্টেজের ক্ষণস্থায়ী বৃদ্ধিকে ওভারশুট এবং এর ফলে সৃষ্ট দোলনকে রিংগিং বলে।

#### ii) Classifications of IC

**English:** Integrated Circuits (ICs) can be classified based on their manufacturing process and scale of integration.

- **Based on Fabrication:**
    
    1. **Monolithic ICs:** All active and passive components are formed on a single continuous silicon chip (Most common).
        
    2. **Hybrid/Multichip ICs:** Formed by interconnecting multiple separate chips on a common insulating substrate.
        
- **Based on Scale of Integration (Number of gates per chip):**
    
    1. **SSI (Small Scale Integration):** Contains up to 10 logic gates.
        
    2. **MSI (Medium Scale Integration):** Contains 10 to 100 logic gates (e.g., decoders, multiplexers).
        
    3. **LSI (Large Scale Integration):** Contains 100 to 10,000 logic gates (e.g., early microprocessors).
        
    4. **VLSI (Very Large Scale Integration):** Contains 10,000 to 1,000,000 logic gates (e.g., modern microcontrollers).
        
    5. **ULSI (Ultra LSI):** Contains more than 1 million gates.
        

**Bangla:** ইন্টিগ্রেটেড সার্কিট (IC)-কে এর তৈরির পদ্ধতি এবং উপাদান সংখ্যার ওপর ভিত্তি করে শ্রেণিবদ্ধ করা হয়।

- **তৈরির পদ্ধতির ওপর ভিত্তি করে:**
    
    ১. **মনোলিথিক আইসি:** সমস্ত উপাদান একটিমাত্র সিলিকন চিপের ওপর তৈরি করা হয়।
    
    ২. **হাইব্রিড আইসি:** একাধিক আলাদা চিপ বা উপাদান একটি কমন সাবস্ট্রেটের ওপর যুক্ত করে এটি তৈরি হয়।
    
- **স্কেল অফ ইন্টিগ্রেশন (লজিক গেটের সংখ্যা) অনুযায়ী:**
    
    ১. **SSI:** এতে ১০টির কম লজিক গেট থাকে।
    
    ২. **MSI:** এতে ১০ থেকে ১০০টি লজিক গেট থাকে (যেমন- ডিকোডার, মাল্টিপ্লেক্সার)।
    
    ৩. **LSI:** এতে ১০০ থেকে ১০,০০০টি লজিক গেট থাকে।
    
    ৪. **VLSI:** এতে ১০,০০০ থেকে ১০ লাখ লজিক গেট থাকে।
    
    ৫. **ULSI:** এতে ১০ লাখের বেশি গেট থাকে (যেমন- আধুনিক প্রসেসর)।
    

#### iii) Time base generator

**English:** A time-base generator (also known as a sweep generator) is an electronic circuit that produces an output voltage or current that varies linearly with time. The typical waveform produced is a sawtooth wave, characterized by a slow, linear rise in voltage (sweep time) followed by a rapid, almost instantaneous return to its initial starting value (retrace or flyback time). This linear sweep is crucially used in the horizontal deflection plates of a Cathode Ray Oscilloscope (CRO) to sweep the electron beam at a constant speed across the screen. This provides a uniform time axis ($x$-axis) to accurately display unknown time-varying input signals.

**Bangla:** টাইম বেস জেনারেটর (বা সুইপ জেনারেটর) হলো এমন একটি ইলেকট্রনিক সার্কিট, যা সময়ের সাথে সাথে রৈখিকভাবে (linearly) পরিবর্তিত হয় এমন আউটপুট ভোল্টেজ বা কারেন্ট তৈরি করে। এটি সাধারণত একটি করাত-দাঁতী (Sawtooth) তরঙ্গ তৈরি করে, যেখানে ভোল্টেজ ধীরে ধীরে রৈখিকভাবে বৃদ্ধি পায় এবং পরবর্তীতে হঠাৎ করে তার আদি অবস্থায় নেমে আসে। এই সার্কিটটি মূলত ক্যাথোড রে অসিলোস্কোপের (CRO) অনুভূমিক (Horizontal) ডিফ্লেকশন প্লেটে ব্যবহার করা হয়। এটি ইলেকট্রন বিমকে পর্দার ওপর দিয়ে ধ্রুব বেগে সরিয়ে নিয়ে যায়, যা একটি সুষম সময়ের অক্ষ (Time axis) তৈরি করে, যাতে অজানা সিগন্যালকে নিখুঁতভাবে প্রদর্শন করা যায়।

#### iv) Shift register

_(Please refer to the detailed answer in **2024 - 8(d)** for both English and Bangla explanations.)_

#### v) Active filter

_(Please refer to the detailed answer in **2024 - 8(e)** for both English and Bangla explanations.)_

## B.Sc. (Hons) Part-IV Examination - 2019

### 8. Write short notes on (any four):

#### (i) Active filter

_(Please refer to the detailed answer in **2024 - 8(e)** for both English and Bangla explanations.)_

#### (ii) Blocking oscillator

_(Please refer to the detailed answer in **2023 - 8(c)** for both English and Bangla explanations.)_

#### (iii) Time-base generator

_(Please refer to the detailed answer in **2020 - 8(iii)** for both English and Bangla explanations.)_

#### (iv) Shift register

_(Please refer to the detailed answer in **2024 - 8(d)** for both English and Bangla explanations.)_

#### (v) RAM and ROM

_(Please refer to the detailed answer in **2021 - 8(b)** for both English and Bangla explanations.)_