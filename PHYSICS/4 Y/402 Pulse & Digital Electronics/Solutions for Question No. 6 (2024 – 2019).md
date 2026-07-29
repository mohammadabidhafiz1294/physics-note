## B.Sc. (Hons) Part-IV Examination - 2024

### 6. (a) Explain the difference between combinational and sequential circuits.

#### English Answer:

| **Feature**           | **Combinational Circuit**                            | **Sequential Circuit**                                                                    |
| --------------------- | ---------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| **Output Dependency** | The output depends solely on the **present inputs**. | The output depends on the **present inputs** as well as **past outputs** (present state). |
| **Memory**            | It does not have any memory elements.                | It contains memory elements (like flip-flops or latches) to store past states.            |
| **Feedback**          | There is no feedback path from output to input.      | It must have a feedback path from the output back to the input.                           |
| **Clock Signal**      | Operations are not controlled by a clock.            | Operations are typically synchronized by a clock signal.                                  |
| **Examples**          | Adders, Subtractors, Multiplexers, Decoders.         | Counters, Shift Registers, Flip-Flops.                                                    |

#### বাংলা উত্তর:

|**বৈশিষ্ট্য**|**কম্বিনেশনাল সার্কিট (Combinational Circuit)**|**সিকুয়েনশিয়াল সার্কিট (Sequential Circuit)**|
|---|---|---|
|**আউটপুটের নির্ভরতা**|এর আউটপুট শুধুমাত্র **বর্তমান ইনপুটের** উপর নির্ভর করে।|এর আউটপুট **বর্তমান ইনপুট** এবং **পূর্ববর্তী আউটপুট** (বর্তমান অবস্থা) উভয়ের উপর নির্ভর করে।|
|**মেমরি**|এতে কোনো মেমরি উপাদান থাকে না।|পূর্বের অবস্থা ধরে রাখার জন্য এতে মেমরি উপাদান (যেমন ফ্লিপ-ফ্লপ) থাকে।|
|**ফিডব্যাক**|আউটপুট থেকে ইনপুটে কোনো ফিডব্যাক পথ থাকে না।|আউটপুট থেকে ইনপুটে অবশ্যই একটি ফিডব্যাক পথ থাকে।|
|**ক্লক সিগন্যাল**|এর কাজ ক্লক সিগন্যাল দ্বারা নিয়ন্ত্রিত হয় না।|এর কাজ সাধারণত ক্লক সিগন্যাল দ্বারা সিঙ্ক্রোনাইজ করা হয়।|
|**উদাহরণ**|অ্যাডার, সাবট্রাক্টর, মাল্টিপ্লেক্সার, ডিকোডার।|কাউন্টার, শিফট রেজিস্টার, ফ্লিপ-ফ্লপ।|

### 6. (b) What is a JK flip-flop? Explain its working principle.

#### English Answer:

**JK Flip-Flop:** The JK flip-flop is a refinement of the basic SR flip-flop that eliminates the invalid or indeterminate state (where S=1 and R=1). The inputs 'J' and 'K' act similarly to 'Set' and 'Reset', but when both are HIGH (1), the flip-flop toggles its output state.

**Logic Diagram:**

Plaintext

```
           +----------------------------------------+
           |                                        |
           |      J o---|NAND|---+---\              |
           |            |  1 |   |NAND>o---o Q      |
           |      +-----|    | +-| 3 /  |           |
           |      |     +----+ | |      |           |
           +------+            | |      +-----------+--o To K's NAND
                  | CLK o------+ |      |           |
           +------+            | |      +-----------+--o To J's NAND
           |      |     +----+ | |      |           |
           |      +-----|    | | +---\  |           |
           |      K o---|NAND|-+-|NAND>o+--o Q'     |
           |            |  2 |   | 4 /              |
           +----------------------------------------+
```

**Working Principle:**

The JK flip-flop uses cross-coupled feedback from the outputs ($Q$ and $Q'$) back to the input NAND gates. The next state equation is:

$$Q_{n+1} = J \bar{Q}_n + \bar{K} Q_n$$

1. **$J=0, K=0$:** The inputs to gates 3 and 4 remain unchanged. The flip-flop holds its previous state (No Change).
    
2. **$J=0, K=1$:** If $Q$ was 1, the lower input gate becomes active, sending a LOW to the output latch, resetting $Q$ to 0 (Reset).
    
3. **$J=1, K=0$:** If $Q'$ was 1 (i.e., $Q=0$), the upper input gate becomes active, sending a LOW to the output latch, setting $Q$ to 1 (Set).
    
4. **$J=1, K=1$:** This is the toggle condition. If $Q=0$, the upper gate is enabled by $Q'=1$, setting $Q$ to 1. If $Q=1$, the lower gate is enabled, resetting $Q$ to 0. Thus, the output toggles on every clock pulse.
    

#### বাংলা উত্তর:

**JK ফ্লিপ-ফ্লপ:** JK ফ্লিপ-ফ্লপ হলো বেসিক SR ফ্লিপ-ফ্লপের একটি উন্নত রূপ, যা SR ফ্লিপ-ফ্লপের অবৈধ বা অসংজ্ঞায়িত অবস্থাকে (S=1, R=1) দূর করে। এর 'J' এবং 'K' ইনপুট যথাক্রমে 'Set' এবং 'Reset' এর মতো কাজ করে, কিন্তু যখন উভয় ইনপুট HIGH (1) হয়, তখন ফ্লিপ-ফ্লপটি টগল (toggle) বা অবস্থার পরিবর্তন করে।

**কার্যনীতি:**

JK ফ্লিপ-ফ্লপে আউটপুট ($Q$ এবং $Q'$) থেকে ইনপুট NAND গেটগুলোতে ফিডব্যাক দেওয়া হয়। এর ইকুয়েশন হলো:

$$Q_{n+1} = J \bar{Q}_n + \bar{K} Q_n$$

১. **$J=0, K=0$:** ফ্লিপ-ফ্লপটি তার পূর্বের অবস্থা ধরে রাখে (No Change)।

২. **$J=0, K=1$:** আউটপুট $Q$ রিসেট হয়ে 0 হয়ে যায় (Reset)।

৩. **$J=1, K=0$:** আউটপুট $Q$ সেট হয়ে 1 হয়ে যায় (Set)।

৪. **$J=1, K=1$:** এটি টগল অবস্থা। যদি পূর্বের আউটপুট $Q=0$ হয় তবে এটি 1 হবে, আর $Q=1$ হলে তা 0 হবে। অর্থাৎ, প্রতিটি ক্লক পালসে আউটপুট বিপরীত অবস্থায় চলে যায়।

### 6. (c) Sketch the timing diagram for a JK flip-flop, indicating the behavior of inputs and outputs.

#### English Answer:

Assuming a **Negative-edge triggered** JK Flip-Flop:

Plaintext

```
       ___     ___     ___     ___     ___     ___
CLK:  |   |___|   |___|   |___|   |___|   |___|   |___
        ↓       ↓       ↓       ↓       ↓       ↓
       _______         _______________         _______
J  :  |       |_______|               |_______|
               _______                 _______________
K  :  ________|       |_______________|
         Set    Reset      Toggle      Toggle   Hold
       _______         _______         _______________
Q  :  |       |_______|       |_______|               |
      0       1       0       1       0       0       0
```

- **Arrow (↓):** Active negative clock edge.
    
- **1st edge ($J=1, K=0$):** $Q$ becomes HIGH (Set).
    
- **2nd edge ($J=0, K=1$):** $Q$ becomes LOW (Reset).
    
- **3rd & 4th edge ($J=1, K=1$):** $Q$ Toggles state ($0 \rightarrow 1$ and $1 \rightarrow 0$).
    
- **5th edge ($J=0, K=0$):** $Q$ Holds its previous state (LOW).
    

#### বাংলা উত্তর:

একটি **নেগেটিভ-এজ ট্রিগারড** JK ফ্লিপ-ফ্লপের টাইমিং ডায়াগ্রাম উপরে দেখানো হয়েছে।

- **তীরচিহ্ন (↓):** ক্লক সিগন্যালের নেগেটিভ এজ নির্দেশ করে, যখন ফ্লিপ-ফ্লপ কাজ করে।
    
- ১ম এজে $J=1, K=0$ থাকায় আউটপুট $Q=1$ (Set) হয়।
    
- ২য় এজে $J=0, K=1$ থাকায় আউটপুট $Q=0$ (Reset) হয়।
    
- ৩য় ও ৪র্থ এজে $J=1, K=1$ থাকায় আউটপুট টগল (Toggle) করে, অর্থাৎ 0 থেকে 1 এবং 1 থেকে 0 হয়।
    
- ৫ম এজে $J=0, K=0$ থাকায় আউটপুট আগের অবস্থাই ধরে রাখে (Hold)।
    

### 6. (d) Explain the master-slave JK flip-flop and how it prevents race conditions in sequential circuits.

#### English Answer:

**Master-Slave JK Flip-Flop:**

A Master-Slave JK flip-flop is a cascaded combination of two SR (or JK) flip-flops: one acts as the "Master" and the other as the "Slave." They are driven by the same clock signal, but the clock for the slave is inverted.

**How it prevents Race-Around Condition:**

- **Race-Around Condition:** In a standard level-triggered JK flip-flop, if $J=1, K=1$ and the clock pulse width ($t_p$) is longer than the propagation delay of the flip-flop ($t_{pd}$), the output will toggle continuously back and forth (1-0-1-0...) within a single clock pulse. This unpredictable behavior is the race-around condition.
    
- **Master-Slave Prevention:** 1. During the HIGH level of the clock (CLK = 1), the Master flip-flop is active and responds to the $J$ and $K$ inputs. However, because the Slave's clock is inverted (CLK' = 0), the Slave is inactive. The final output ($Q$ and $Q'$) remains unchanged.
    
    2. During the LOW level of the clock (CLK = 0), the Master is disabled, locking its data. The Slave becomes active (CLK' = 1) and transfers the data from the Master to the final outputs.
    
    3. Because the outputs $Q$ and $Q'$ change only on the falling edge of the clock, the feedback to the $J$ and $K$ input gates is delayed until the master is fully disabled. This isolation ensures the flip-flop can toggle only _once_ per clock cycle, effectively eliminating the race-around condition.
    

#### বাংলা উত্তর:

**মাস্টার-স্লেভ JK ফ্লিপ-ফ্লপ:**

এটি দুটি ফ্লিপ-ফ্লপের সমন্বয়ে তৈরি, যার একটিকে "মাস্টার" (Master) এবং অন্যটিকে "স্লেভ" (Slave) বলা হয়। এগুলো একই ক্লক সিগন্যাল দ্বারা চালিত হয়, তবে স্লেভ ফ্লিপ-ফ্লপে ক্লক সিগন্যালটি ইনভার্ট (উল্টে) করে দেওয়া হয়।

**এটি যেভাবে রেস-এরাউন্ড অবস্থা (Race-Around Condition) রোধ করে:**

- **রেস-এরাউন্ড অবস্থা:** সাধারণ লেভেল-ট্রিগারড JK ফ্লিপ-ফ্লপে $J=1$ এবং $K=1$ হলে এবং ক্লক পালসের সময়কাল ফ্লিপ-ফ্লপের প্রোপাগেশন ডিলের চেয়ে বেশি হলে, একই ক্লক পালসের মধ্যে আউটপুট বারবার 1-0-1-0 পরিবর্তন হতে থাকে। একে রেস-এরাউন্ড অবস্থা বলে।
    
- **মাস্টার-স্লেভের মাধ্যমে সমাধান:** ১. যখন ক্লক পালস HIGH (1) থাকে, তখন মাস্টার সক্রিয় হয় এবং $J, K$ ইনপুট গ্রহণ করে। কিন্তু স্লেভের ক্লক ইনভার্টেড হওয়ায় স্লেভ নিষ্ক্রিয় থাকে। ফলে চূড়ান্ত আউটপুটে কোনো পরিবর্তন হয় না।
    
    ২. যখন ক্লক পালস LOW (0) হয়, তখন মাস্টার নিষ্ক্রিয় হয় এবং ইনপুট নেওয়া বন্ধ করে। এ সময় স্লেভ সক্রিয় হয় এবং মাস্টারের ডেটা চূড়ান্ত আউটপুটে ($Q$ ও $Q'$) স্থানান্তর করে।
    
    ৩. যেহেতু চূড়ান্ত আউটপুট শুধুমাত্র ক্লকের নেগেটিভ এজে (HIGH থেকে LOW তে নামার সময়) পরিবর্তিত হয়, তাই ইনপুটে ফিডব্যাক যেতে যেতে মাস্টার সম্পূর্ণ বন্ধ হয়ে যায়। ফলে একটি ক্লক পালসে আউটপুট মাত্র একবারই টগল করতে পারে এবং রেস-এরাউন্ড অবস্থা সম্পূর্ণ দূর হয়।
    

## B.Sc. (Hons) Part-IV Examination - 2023

### 6. (a) What is a clock signal, and why is it essential in sequential circuits?

#### English Answer:

- **Clock Signal:** A clock signal is a continuous, periodic square wave that oscillates between a HIGH state (logic 1) and a LOW state (logic 0). It acts as the timing mechanism or "heartbeat" for digital systems.
    
- **Essentiality in Sequential Circuits:** 1. **Synchronization:** It ensures that multiple flip-flops and components in a circuit change states simultaneously, coordinating complex operations.
    
    2. **Predictability:** Without a clock, transient noise or uneven signal delays (glitches) could cause false state changes. The clock ensures the circuit only reads inputs at precise, safe moments (the edges).
    
    3. **Timing Control:** It dictates the speed of the digital system and allows for orderly step-by-step data processing.
    

#### বাংলা উত্তর:

- **ক্লক সিগন্যাল (Clock Signal):** ক্লক সিগন্যাল হলো একটি পর্যায়বৃত্ত (periodic) স্কয়ার ওয়েভ যা অবিরত HIGH (লজিক 1) এবং LOW (লজিক 0) অবস্থার মধ্যে ওঠানামা করে। এটি ডিজিটাল সিস্টেমের টাইমিং মেকানিজম বা স্পন্দন হিসেবে কাজ করে।
    
- **সিকুয়েনশিয়াল সার্কিটে এর গুরুত্ব:**
    
    ১. **সিঙ্ক্রোনাইজেশন:** এটি নিশ্চিত করে যে সার্কিটের বিভিন্ন ফ্লিপ-ফ্লপ ও মেমরি উপাদানগুলো একই সাথে অবস্থার পরিবর্তন করবে, যা জটিল প্রক্রিয়াগুলো সঠিকভাবে সম্পন্ন করতে সাহায্য করে।
    
    ২. **পূর্বাভাসযোগ্যতা:** ক্লক ছাড়া সিগন্যালের অসামঞ্জস্যতা বা নয়েজের কারণে ভুল আউটপুট আসতে পারে। ক্লক সিগন্যাল নির্দিষ্ট সময়ে (edges) ইনপুট পড়তে বাধ্য করে, ফলে সার্কিট স্থিতিশীল থাকে।
    
    ৩. **টাইমিং নিয়ন্ত্রণ:** এটি ডিজিটাল সিস্টেমের গতি নির্ধারণ করে এবং ধাপে ধাপে সুশৃঙ্খলভাবে ডেটা প্রক্রিয়াকরণের অনুমতি দেয়।
    

### 6. (b) Explain the key differences between a latch and a flip-flop.

#### English Answer:

|**Feature**|**Latch**|**Flip-Flop**|
|---|---|---|
|**Triggering**|Level-triggered (changes state whenever the enable signal is HIGH or LOW).|Edge-triggered (changes state only at the rising or falling edge of the clock).|
|**Clock Signal**|Does not use a clock signal (uses an Enable signal).|Uses a clock signal for synchronization.|
|**Operation Mode**|Operates asynchronously. It is "transparent" when enabled.|Operates synchronously.|
|**Structure**|Constructed simply from logic gates (NAND/NOR).|Constructed from latches with added clocking and edge-detector circuitry.|

#### বাংলা উত্তর:

|**বৈশিষ্ট্য**|**ল্যাচ (Latch)**|**ফ্লিপ-ফ্লপ (Flip-Flop)**|
|---|---|---|
|**ট্রিগারিং**|এটি লেভেল-ট্রিগারড (এনাবল সিগন্যাল HIGH বা LOW থাকা অবস্থায় আউটপুট পরিবর্তন করতে পারে)।|এটি এজ-ট্রিগারড (ক্লকের শুধুমাত্র রাইজিং বা ফলিং এজে আউটপুট পরিবর্তন করে)।|
|**ক্লক সিগন্যাল**|কোনো ক্লক সিগন্যাল ব্যবহার করে না (এনাবল সিগন্যাল ব্যবহার করে)।|সিঙ্ক্রোনাইজেশনের জন্য ক্লক সিগন্যাল ব্যবহার করে।|
|**অপারেশন**|এটি অ্যাসিনক্রোনাসভাবে কাজ করে। এনাবল থাকলে এটি "স্বচ্ছ" (transparent) আচরণ করে।|এটি সিনক্রোনাসভাবে কাজ করে।|
|**গঠন**|লজিক গেট (NAND/NOR) দিয়ে সহজভাবে তৈরি করা হয়।|ক্লক এবং এজ-ডিটেক্টর সার্কিট যুক্ত করে ল্যাচ থেকে ফ্লিপ-ফ্লপ তৈরি করা হয়।|

### 6. (c) Describe the working principle of a clocked-SR flip-flop. Draw its logic diagram and truth table.

#### English Answer:

**Clocked SR Flip-Flop:** A clocked SR flip-flop is a basic SR latch with an added clock input that restricts the inputs from affecting the outputs unless the clock signal is HIGH.

**Logic Diagram:**

Plaintext

```
      S o-----|NAND 1|-------o S' 
              |      |         |
              +------+         +---|NAND 3|----o Q
                 |                 |      |
      CLK o------+-----------------+      |
                 |                 +------+
              +------+             |      |
              |      |         +---|NAND 4|----o Q'
      R o-----|NAND 2|-------o R'  |      |
```

**Working Principle:**

- The circuit uses two NAND gates (1 & 2) at the input to gate the clock signal.
    
- **When CLK = 0:** The outputs of NAND 1 and NAND 2 are forced to logic 1 regardless of $S$ and $R$. The SR latch (NAND 3 & 4) receives inputs (1,1), meaning "No Change". The flip-flop holds its state.
    
- **When CLK = 1:** The NAND 1 and NAND 2 outputs act as the complements of $S$ and $R$.
    
    - If $S=1, R=0$: The latch receives $S'=0, R'=1$, setting $Q=1$.
        
    - If $S=0, R=1$: The latch receives $S'=1, R'=0$, resetting $Q=0$.
        
    - If $S=1, R=1$: Both $S'$ and $R'$ become 0, forcing both $Q$ and $Q'$ to 1, which violates the complementary rule. This is the **invalid** state.
        

**Truth Table:**

|**CLK**|**S**|**R**|**Qn+1​ (Next State)**|**State**|
|---|---|---|---|---|
|0|X|X|$Q_n$|Hold (No Change)|
|1|0|0|$Q_n$|Hold (No Change)|
|1|0|1|0|Reset|
|1|1|0|1|Set|
|1|1|1|Invalid|Indeterminate|

#### বাংলা উত্তর:

**ক্লকড SR ফ্লিপ-ফ্লপ:** এটি একটি সাধারণ SR ল্যাচ, যার সাথে একটি ক্লক ইনপুট যুক্ত থাকে। ক্লক সিগন্যাল HIGH না হওয়া পর্যন্ত ইনপুটগুলো আউটপুটে কোনো প্রভাব ফেলতে পারে না।

**কার্যনীতি:**

- ইনপুটে দুটি NAND গেট (1 ও 2) ক্লক সিগন্যালকে নিয়ন্ত্রণ করে।
    
- **যখন CLK = 0:** $S$ ও $R$ এর মান যাই হোক না কেন, NAND 1 ও 2 এর আউটপুট 1 হয়। ফলে মূল ল্যাচ (NAND 3 ও 4) "No Change" অবস্থায় থাকে।
    
- **যখন CLK = 1:** * $S=0, R=0$ হলে, ফ্লিপ-ফ্লপ তার আগের অবস্থা ধরে রাখে (Hold)।
    
    - $S=1, R=0$ হলে, আউটপুট $Q=1$ হয় (Set)।
        
    - $S=0, R=1$ হলে, আউটপুট $Q=0$ হয় (Reset)।
        
    - $S=1, R=1$ হলে, ল্যাচের উভয় ইনপুট 0 হয়ে যায় যা আউটপুট $Q$ এবং $Q'$ উভয়কেই 1 করে দেয়। এটি একটি **অবৈধ (Invalid)** অবস্থা।
        

_(লজিক ডায়াগ্রাম এবং ট্রুথ টেবিলের জন্য উপরের ইংরেজি অংশটি অনুসরণ করুন)_

### 6. (d) Does a clocked SR flip-flop resolve the issues associated with a basic SR flip-flop?

#### English Answer:

A clocked SR flip-flop resolves **one** of the issues of a basic SR flip-flop but **fails to resolve the most critical one**.

- **Issue Resolved:** It solves the synchronization problem. The basic SR latch is transparent and changes state asynchronously. The clocked SR flip-flop synchronizes state changes with the clock pulse, making it suitable for complex sequential circuits.
    
- **Issue NOT Resolved:** It **does not** resolve the indeterminate/invalid state problem. If both $S=1$ and $R=1$ are applied when the clock is HIGH, it still forces both $Q$ and $Q'$ to 1, leading to an unpredictable next state. To fully resolve this, a JK flip-flop or D flip-flop is required.
    

#### বাংলা উত্তর:

ক্লকড SR ফ্লিপ-ফ্লপ বেসিক SR ফ্লিপ-ফ্লপের **একটি** সমস্যার সমাধান করলেও **সবচেয়ে বড় সমস্যাটি** সমাধান করতে পারে না।

- **যে সমস্যার সমাধান হয়:** এটি সিঙ্ক্রোনাইজেশনের সমস্যার সমাধান করে। বেসিক SR ল্যাচ যেকোনো সময় ইনপুট পরিবর্তনে সাড়া দেয়। কিন্তু ক্লকড SR ফ্লিপ-ফ্লপ শুধুমাত্র ক্লক পালসের উপস্থিতিতে কাজ করে, যা জটিল সার্কিটের জন্য উপযুক্ত।
    
- **যে সমস্যার সমাধান হয় না:** এটি $S=1, R=1$ এর **অবৈধ অবস্থার (Invalid State)** কোনো সমাধান করতে পারে না। ক্লক HIGH থাকা অবস্থায় উভয় ইনপুট 1 হলে এটি এখনও অনির্দিষ্ট আচরণ করে। এই সমস্যার সম্পূর্ণ সমাধানের জন্য JK বা D ফ্লিপ-ফ্লপ ব্যবহার করতে হয়।
    

## B.Sc. (Hons) Part-IV Examination - 2022

### 6. (a) Discuss different types of triggering.

#### English Answer:

In digital sequential circuits, triggering refers to the mechanism by which a clock signal initiates a state change in a flip-flop.

1. **Level Triggering:** The flip-flop responds to the input signals as long as the clock is at a specific logic level.
    
    - **Positive Level Triggering:** Responds when the clock is HIGH (logic 1).
        
    - **Negative Level Triggering:** Responds when the clock is LOW (logic 0).
        
2. **Edge Triggering:** The flip-flop responds to inputs only at the exact instant the clock signal transitions from one level to another.
    
    - **Positive-Edge Triggering:** Responds only during the transition from LOW to HIGH (rising edge).
        
    - **Negative-Edge Triggering:** Responds only during the transition from HIGH to LOW (falling edge).
        

#### বাংলা উত্তর:

ডিজিটাল সিকুয়েনশিয়াল সার্কিটে, ট্রিগারিং বলতে এমন একটি মেকানিজম বোঝায় যার মাধ্যমে ক্লক সিগন্যাল ফ্লিপ-ফ্লপের অবস্থা পরিবর্তন করে।

১. **লেভেল ট্রিগারিং:** ক্লক সিগন্যাল একটি নির্দিষ্ট লজিক লেভেলে যতক্ষণ অবস্থান করে, ততক্ষণ ফ্লিপ-ফ্লপ কাজ করে।

- **পজিটিভ লেভেল ট্রিগারিং:** ক্লক HIGH (1) থাকা অবস্থায় কাজ করে।
    
- **নেগেটিভ লেভেল ট্রিগারিং:** ক্লক LOW (0) থাকা অবস্থায় কাজ করে।
    
    ২. **এজ ট্রিগারিং:** ক্লক সিগন্যাল যখন একটি লেভেল থেকে অন্য লেভেলে পরিবর্তিত হয়, ঠিক সেই মুহূর্তেই ফ্লিপ-ফ্লপ কাজ করে।
    
- **পজিটিভ এজ ট্রিগারিং:** ক্লক LOW থেকে HIGH-তে ওঠার সময় (Rising edge) কাজ করে।
    
- **নেগেটিভ এজ ট্রিগারিং:** ক্লক HIGH থেকে LOW-তে নামার সময় (Falling edge) কাজ করে।
    

### 6. (b) What are sequential and combinational circuits?

_(Please refer to the detailed answer in **2024 - 6(a)** for both English and Bangla explanations.)_

### 6. (c) Discuss the construction and operation of a JK flip-flop.

_(Please refer to the detailed answer in **2024 - 6(b)** for both English and Bangla explanations.)_

### 6. (d) How many flip-flops are required to count from 0 to 256? What count will it hold after 257 counts?

#### English Answer:

- **Number of Flip-Flops:** To count from 0 to 256, the counter must be able to represent the decimal number 256. The maximum number represented by $n$ flip-flops is $2^n - 1$.
    
    - For $n=8$ flip-flops, max count = $2^8 - 1 = 255$ (counts 0 to 255).
        
    - For $n=9$ flip-flops, max count = $2^9 - 1 = 511$ (counts 0 to 511).
        
        Therefore, to reach the number 256, we require a minimum of **9 flip-flops**.
        
- **Count after 257 pulses:** Assuming the counter starts at 0 and increments by 1 for each pulse:
    
    - 1st count (pulse) $\rightarrow$ holds value 1.
        
    - 256th count (pulse) $\rightarrow$ holds value 256.
        
    - 257th count (pulse) $\rightarrow$ will hold the value **257** (Binary: `100000001`), assuming it is a standard 9-bit binary counter.
        
        _(Note: If the question implies a MOD-257 counter that resets after reaching 256, the 257th pulse would wrap it back to 0. However, in standard binary counting, it simply holds 257)._
        

#### বাংলা উত্তর:

- **ফ্লিপ-ফ্লপের সংখ্যা:** 0 থেকে 256 পর্যন্ত গণনা করতে কাউন্টারটিকে 256 সংখ্যাটি ধারণ করতে হবে। $n$ টি ফ্লিপ-ফ্লপ সর্বোচ্চ $2^n - 1$ পর্যন্ত গুণতে পারে।
    
    - 8টি ফ্লিপ-ফ্লপ দিয়ে $2^8 - 1 = 255$ পর্যন্ত (0-255) গোনা যায়।
        
    - 9টি ফ্লিপ-ফ্লপ দিয়ে $2^9 - 1 = 511$ পর্যন্ত গোনা যায়।
        
        সুতরাং, 256 সংখ্যাটি গণনার জন্য ন্যূনতম **9 টি ফ্লিপ-ফ্লপ** প্রয়োজন।
        
- **257 টি পালসের পর মান:** যদি কাউন্টারটি 0 থেকে শুরু হয় এবং প্রতিটি পালসে 1 করে বাড়ে:
    
    - ১ম পালসের পর মান হবে 1।
        
    - 256 তম পালসের পর মান হবে 256।
        
    - 257 তম পালসের পর এটি **257** মানটি ধারণ করবে (বাইনারিতে: `100000001`), যদি এটি একটি সাধারণ 9-বিট বাইনারি কাউন্টার হয়।
        

## B.Sc. (Hons) Part-IV Examination - 2021

### 6. (a) What is flip-flop? Discuss SET and clearing of a NAND gate latch.

#### English Answer:

**Flip-Flop:** A flip-flop is a bistable multivibrator, a digital sequential logic circuit capable of storing a single bit (0 or 1) of binary data. It has two stable states and remains in one state until triggered by an appropriate external input/clock.

**SET and Clearing of a NAND Gate Latch:**

A basic NAND latch uses active-LOW inputs, typically labeled $S'$ (Set) and $R'$ (Reset).

1. **SET Operation:** To set the latch (store a 1), a momentary LOW (0) is applied to the $S'$ input while $R'$ is kept HIGH (1). The 0 at the NAND gate forces the $Q$ output to 1. The feedback holds this 1 even after $S'$ returns to 1.
    
2. **CLEAR (Reset) Operation:** To clear the latch (store a 0), a momentary LOW (0) is applied to the $R'$ input while $S'$ is kept HIGH (1). This forces $Q'$ to 1, and the feedback forces $Q$ to 0.
    

#### বাংলা উত্তর:

**ফ্লিপ-ফ্লপ:** ফ্লিপ-ফ্লপ হলো একটি বাইস্টেবল মাল্টিভাইব্রেটর, যা ডিজিটাল সিকুয়েনশিয়াল সার্কিটে 1-বিট ডেটা (0 বা 1) মেমরিতে ধরে রাখতে ব্যবহৃত হয়। এর দুটি স্থিতিশীল অবস্থা থাকে এবং বাহ্যিক ট্রিগার প্রয়োগ না করা পর্যন্ত এটি তার অবস্থা ধরে রাখে।

**NAND ল্যাচের SET এবং Clear (Reset) প্রক্রিয়া:**

বেসিক NAND ল্যাচ অ্যাকটিভ-লো (Active-LOW) ইনপুটে কাজ করে, যাদের $S'$ এবং $R'$ দ্বারা নির্দেশ করা হয়।

১. **SET প্রক্রিয়া:** ল্যাচকে সেট করতে ($Q=1$ করতে) $R'$ কে HIGH (1) রেখে $S'$ ইনপুটে সাময়িকভাবে LOW (0) প্রয়োগ করা হয়। $S'=0$ হওয়ার ফলে $Q$ এর মান 1 হয়ে যায়। $S'$ পুনরায় 1 এ ফিরে গেলেও ল্যাচটি এই 1 মান ধরে রাখে।

২. **CLEAR (Reset) প্রক্রিয়া:** ল্যাচকে ক্লিয়ার করতে ($Q=0$ করতে) $S'$ কে HIGH (1) রেখে $R'$ ইনপুটে সাময়িকভাবে LOW (0) প্রয়োগ করা হয়। ফলে $Q'$ 1 হয়ে যায় এবং ফিডব্যাকের মাধ্যমে $Q$ এর মান 0 হয়ে যায়।

### 6. (b) Discuss the construction and working principle of a clocked-SR flip-flop. Mention the problems associated with SR flip-flops.

_(For the construction and working principle, please refer to the detailed answer in **2023 - 6(c)**)._

#### English Answer (Problems associated with SR flip-flops):

The primary problem associated with an SR flip-flop is the **invalid or indeterminate state**.

When both Set ($S$) and Reset ($R$) inputs are HIGH (1) simultaneously, both outputs $Q$ and $Q'$ are forced to the same logic level (typically 1 in NAND-based, 0 in NOR-based), violating the rule that outputs must be complements of each other. Furthermore, if $S$ and $R$ transition back to 0 simultaneously from this state, it creates a race condition, making the final state completely unpredictable.

#### বাংলা উত্তর (SR ফ্লিপ-ফ্লপের সমস্যাসমূহ):

SR ফ্লিপ-ফ্লপের প্রধান সমস্যাটি হলো এর **অবৈধ বা অসংজ্ঞায়িত অবস্থা (Invalid State)**।

যখন Set ($S$) এবং Reset ($R$) উভয় ইনপুট একসাথে HIGH (1) হয়, তখন $Q$ এবং $Q'$ উভয় আউটপুটই একই মান (NAND এর ক্ষেত্রে 1) ধারণ করে। এটি ফ্লিপ-ফ্লপের মৌলিক নিয়মের পরিপন্থী (আউটপুট দুটি একে অপরের পরিপূরক হতে হবে)। তাছাড়া, এই অবস্থা থেকে $S$ ও $R$ একসাথে 0 তে নেমে গেলে একটি রেস কন্ডিশন (Race condition) তৈরি হয়, যার ফলে আউটপুট কী হবে তা আগে থেকে অনুমান করা অসম্ভব হয়ে পড়ে।

### 6. (c) Draw the input and output waveforms of a negative edge-triggered SR flip-flop.

#### English Answer & Waveform:

In a negative edge-triggered SR flip-flop, the state changes _only_ on the falling edge (HIGH to LOW transition) of the clock pulse.

Plaintext

```
       ___     ___     ___     ___     ___     ___
CLK:  |   |___|   |___|   |___|   |___|   |___|   |___
          ↓       ↓       ↓       ↓       ↓       ↓
       _______                 _______
S  :  |       |_______________|       |_______________
               _______                 _______
R  :  ________|       |_______________|       |_______

Q  :  ________|---------------|_______|---------------
      Initial | Set           | Reset | Set
      (Q=0)   | (Q=1)         | (Q=0) | (Q=1)
```

- **Edge 1:** $S=1, R=0 \implies Q$ becomes 1.
    
- **Edge 2:** $S=0, R=1 \implies Q$ becomes 0.
    
- **Edge 3:** $S=0, R=0 \implies Q$ holds 0.
    
- **Edge 4:** $S=1, R=0 \implies Q$ becomes 1.
    

#### বাংলা উত্তর:

একটি নেগেটিভ এজ-ট্রিগারড SR ফ্লিপ-ফ্লপে আউটপুট শুধুমাত্র ক্লক পালসের ফলিং এজে (HIGH থেকে LOW তে নামার সময়) পরিবর্তিত হয়। (উপরের টাইমিং ডায়াগ্রামটি আঁকতে হবে)। ডায়াগ্রামে তীর চিহ্ন (↓) দিয়ে নেগেটিভ এজ বোঝানো হয়েছে।

- প্রথম নেগেটিভ এজে $S=1, R=0$ থাকায় $Q$ সেট (1) হয়।
    
- দ্বিতীয় এজে $S=0, R=1$ থাকায় $Q$ রিসেট (0) হয়।
    

## B.Sc. (Hons) Part-IV Examination - 2020

### 6. (a) Compare Combinational logic circuits and Sequential logic circuits.

_(Please refer to the detailed table in **2024 - 6(a)** for both English and Bangla explanations.)_

### 6. (b) i) What are different types of flip-flop? ii) Discuss J-K flip-flop.

#### English Answer:

**i) Different types of flip-flops:**

1. **SR Flip-Flop (Set-Reset):** Basic memory element, has an invalid state when S=1, R=1.
    
2. **JK Flip-Flop:** Overcomes the SR invalid state by toggling when J=1, K=1.
    
3. **D Flip-Flop (Data/Delay):** Has only one input (D). The output $Q$ follows $D$ at the clock edge. Used extensively in registers.
    
4. **T Flip-Flop (Toggle):** Has one input (T). When T=1, it toggles on the clock edge; when T=0, it holds the state. Used in counters.
    

**ii) Discuss J-K flip-flop:**

_(Please refer to the detailed answer in **2024 - 6(b)** for construction, working principle, and Bangla translation)._

#### বাংলা উত্তর:

**i) ফ্লিপ-ফ্লপের প্রকারভেদ:**

১. **SR (Set-Reset) ফ্লিপ-ফ্লপ:** বেসিক মেমরি, S=1, R=1 অবস্থায় এটি অবৈধ আচরণ করে।

২. **JK ফ্লিপ-ফ্লপ:** SR এর ত্রুটি দূর করে, J=1, K=1 হলে এটি টগল (অবস্থা পরিবর্তন) করে।

৩. **D (Data) ফ্লিপ-ফ্লপ:** এর একটি মাত্র ইনপুট (D) থাকে, ক্লক এজে আউটপুট সরাসরি ইনপুটকে অনুসরণ করে।

৪. **T (Toggle) ফ্লিপ-ফ্লপ:** T=1 হলে ক্লক এজে আউটপুট বিপরীত হয়, T=0 হলে আগের অবস্থা ধরে রাখে।

**ii) JK ফ্লিপ-ফ্লপের বর্ণনা:** _(২০২৪ সালের ৬(b) এর উত্তর অনুসরণ করুন)_।

### 6. (c) Define the following parameters in FF operations: (i) Set-up time; (ii) Clock-to-Output time.

#### English Answer:

1. **Set-up Time ($t_s$):** The minimum time duration for which the input data signal must be maintained stable _before_ the active clock transition (edge) occurs, to guarantee reliable recognition of the data. If the input changes within the setup time, the flip-flop may become metastable.
    
2. **Clock-to-Output Time ($t_{pd}$ or $t_{co}$):** Also known as propagation delay. It is the time required for the flip-flop output ($Q$) to change state and stabilize _after_ the active edge of the clock signal has occurred.
    

#### বাংলা উত্তর:

১. **সেট-আপ টাইম (Set-up time, $t_s$):** ক্লক সিগন্যালের অ্যাকটিভ এজ (active edge) আসার _আগে_ ইনপুট ডেটাকে ন্যূনতম যে সময় পর্যন্ত স্থিতিশীল (stable) থাকতে হয়, তাকে সেট-আপ টাইম বলে। এই সময়ের মধ্যে ডেটা পরিবর্তন হলে ফ্লিপ-ফ্লপ সঠিকভাবে ডেটা পড়তে পারে না।

২. **ক্লক-টু-আউটপুট টাইম (Clock-to-Output time, $t_{co}$):** একে প্রোপাগেশন ডিলেও বলা হয়। ক্লক সিগন্যালের অ্যাকটিভ এজ ঘটার _পর_ ফ্লিপ-ফ্লপের আউটপুট পরিবর্তিত হয়ে স্থিতিশীল হতে যে সময় লাগে, তাকে ক্লক-টু-আউটপুট টাইম বলে।

## B.Sc. (Hons) Part-IV Examination - 2019

### 6. (a) Describe the operation of SR flip-flop. Why is a clocking flip-flop important in digital system?

#### English Answer:

**Operation of SR Flip-Flop:**

An SR (Set-Reset) flip-flop has two inputs, S and R.

- **$S=0, R=0$:** The flip-flop holds its current state $Q_n$ (No change).
    
- **$S=0, R=1$:** The flip-flop resets, forcing output $Q$ to 0.
    
- **$S=1, R=0$:** The flip-flop sets, forcing output $Q$ to 1.
    
- **$S=1, R=1$:** This is an invalid/forbidden state where both $Q$ and $Q'$ are forced to the same logic level.
    

**Importance of Clocking:**

In a digital system, a clocking flip-flop is crucial because it introduces **synchronization**. Without a clock, a flip-flop reacts asynchronously to any change or transient noise (glitches) at its inputs. Clocking ensures that state changes occur only at discrete, predictable moments (the clock edges). This allows signals across complex circuits enough time to stabilize, preventing timing errors and ensuring reliable data transfer between different stages of a system.

#### বাংলা উত্তর:

**SR ফ্লিপ-ফ্লপের অপারেশন:**

SR (Set-Reset) ফ্লিপ-ফ্লপের দুটি ইনপুট থাকে, S এবং R।

- **$S=0, R=0$:** ফ্লিপ-ফ্লপটি পূর্বের অবস্থা ধরে রাখে (Hold)।
    
- **$S=0, R=1$:** ফ্লিপ-ফ্লপটি রিসেট (Reset) হয়, অর্থাৎ আউটপুট $Q=0$ হয়।
    
- **$S=1, R=0$:** ফ্লিপ-ফ্লপটি সেট (Set) হয়, অর্থাৎ আউটপুট $Q=1$ হয়।
    
- **$S=1, R=1$:** এটি একটি অবৈধ (Invalid) অবস্থা।
    

**ডিজিটাল সিস্টেমে ক্লকিং ফ্লিপ-ফ্লপের গুরুত্ব:**

ডিজিটাল সিস্টেমে ক্লক অত্যন্ত গুরুত্বপূর্ণ কারণ এটি **সিঙ্ক্রোনাইজেশন** নিশ্চিত করে। ক্লক ছাড়া ফ্লিপ-ফ্লপ ইনপুটের যেকোনো ছোট পরিবর্তন বা নয়েজে সাড়া দিতে পারে। ক্লক ব্যবহার করলে সার্কিটের অবস্থা কেবল একটি নির্দিষ্ট ও পূর্বনির্ধারিত মুহূর্তেই (ক্লক এজে) পরিবর্তিত হয়। এর ফলে সার্কিটের বিভিন্ন অংশের সিগন্যাল স্থিতিশীল হওয়ার জন্য পর্যাপ্ত সময় পায় এবং ডেটা ট্রান্সফারে কোনো ভুল হয় না।

### 6. (b) Draw the input and output waveforms of a negative edge triggered SR flip-flop.

_(Please refer to the detailed answer and ASCII waveform provided in **2021 - 6(c)**)._

### 6. (c) Define propagation delay and hold time in flip-flop operations.

#### English Answer:

1. **Propagation Delay ($t_{pd}$):** The time interval required for the output of a flip-flop to transition and settle to its new logic state after the active edge of the clock (or an asynchronous preset/clear) has been applied.
    
2. **Hold Time ($t_h$):** The minimum time duration for which the input data signal must be maintained stable _after_ the active clock transition (edge) has occurred. This ensures the flip-flop reliably captures the intended data without it changing prematurely.
    

#### বাংলা উত্তর:

১. **প্রোপাগেশন ডিলে (Propagation Delay):** ক্লক সিগন্যালের অ্যাকটিভ এজ প্রয়োগ করার পর, ফ্লিপ-ফ্লপের আউটপুট পরিবর্তিত হয়ে নতুন অবস্থায় পৌঁছাতে এবং স্থিতিশীল হতে যে সময়ের প্রয়োজন হয়, তাকে প্রোপাগেশন ডিলে বলে।

২. **হোল্ড টাইম (Hold Time, $t_h$):** ক্লক সিগন্যালের অ্যাকটিভ এজ ঘটার _পর_ ইনপুট ডেটাকে ন্যূনতম যে সময় পর্যন্ত অপরিবর্তিত বা স্থিতিশীল রাখতে হয়, তাকে হোল্ড টাইম বলে। এটি নিশ্চিত করে যে ফ্লিপ-ফ্লপটি সঠিকভাবে ডেটা ক্যাপচার করেছে।