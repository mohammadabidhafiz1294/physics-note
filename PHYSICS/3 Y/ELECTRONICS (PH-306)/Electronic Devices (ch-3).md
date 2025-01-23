

### AC Current Coupling

AC coupling, also known as capacitor coupling or capacitively coupled coupling, is a technique used in electronic circuits to separate the direct current (DC) component from the alternating current (AC) component of a signal.

In AC coupling, a coupling capacitor is placed in series with the input or output of a circuit. The capacitor acts as a high-pass filter, allowing only the AC component of the signal to pass through while blocking the DC component. The AC component is coupled, or transmitted, to the next stage or circuit, while the DC component is blocked or attenuated.

The purpose of AC coupling is to remove any DC offset or bias present in a signal, enabling the circuit to operate more effectively with AC signals. It is commonly used in applications such as audio amplifiers, where it is necessary to remove any DC voltage present in the input signal before amplification. AC coupling allows for the amplification and processing of the AC signal without distortion or saturation.

It is important to choose an appropriate value for the ***coupling capacitor, considering the desired frequency response*** and the impedance of the connected stages. The capacitor value is selected such that it allows the desired AC frequencies to pass through while attenuating lower frequencies, including the DC component. The choice of capacitor value influences the cutoff frequency and the overall frequency response of the circuit.

AC coupling through a capacitor is a widely used technique in electronic circuits, providing a means to isolate the AC and DC components of a signal and enable effective signal processing and amplification.

![[ac vs dc coupling in capacitor.png]]

### Transistor Biasing

Transistor biasing refers to the process of establishing the correct operating conditions or bias point for a transistor amplifier circuit. The biasing ensures that the transistor operates in its linear region, allowing for proper amplification and signal processing. The biasing process involves setting the appropriate DC voltages and currents at the transistor's terminals (base, emitter, and collector) to establish the desired operating point.

There are different biasing methods used for transistor circuits, but two common techniques are fixed bias and self-bias.

1. Fixed Bias: In fixed bias, a DC voltage source is directly connected to the base-emitter junction, typically through a resistor. This resistor, known as the biasing resistor or base bias resistor, provides the necessary bias voltage. The value of the bias resistor is chosen based on the desired bias current, taking into account the transistor's characteristics. The collector current is determined by the load resistor connected to the collector terminal.
    
2. Self-Bias (Emitter Bias): In self-bias, the transistor's biasing is achieved by connecting a resistor from the base terminal to the emitter terminal. This resistor is called the emitter resistor or biasing resistor. The voltage drop across the emitter resistor biases the transistor. The base-emitter junction acts as a diode, and the emitter resistor introduces negative feedback, stabilizing the bias point. The collector current is determined by the load resistor connected to the collector terminal.

The values of the biasing resistors are chosen carefully to achieve the desired operating point, taking into account factors such as desired collector current, transistor characteristics, and stability considerations. The biasing resistors ensure that the transistor operates in its active region, avoiding cutoff or saturation.

Transistor biasing is crucial for achieving stable and linear amplification. Proper biasing ensures that the transistor remains in a region where small changes in input signal result in linear and undistorted output signals. The specific biasing method used depends on the application and circuit requirements, such as the desired bias stability, temperature variations, and power dissipation considerations.

## BJT (Bipolar Junction Transistor)

If we join together two individual signal diodes back-to-back, this will give us two PN-junctions connected together in series which would share a common _Positve_, (P) or _Negative_, (N) terminal. The fusion of these two diodes produces a three layer, two junction, three terminal device forming the basis of a **Bipolar Junction Transistor**, or **BJT** for short.

Transistors are three terminal active devices made from different semiconductor materials that can act as either an insulator or a conductor by the application of a small signal voltage. The transistor’s ability to change between these two states enables it to have two basic functions: “switching” (digital electronics) or “amplification” (analogue electronics). Then bipolar transistors have the ability to operate within three different regions:

- Active Region   –   the transistor operates as an amplifier and Ic = β*Ib
- Saturation   –   the transistor is “Fully-ON” operating as a switch and Ic = I(saturation)
- Cut-off   –   the transistor is “Fully-OFF” operating as a switch and Ic = 0

![bipolar transistor](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran42a.jpg "Bipolar Transistor")

A Typical  
Bipolar Transistor

The word Transistor is a combination of the two words Transfer Varistor which describes their mode of operation way back in their early days of electronics development. There are two basic types of bipolar transistor construction, PNP and NPN, which basically describes the physical arrangement of the P-type and N-type semiconductor materials from which they are made.

The **Bipolar Transistor** basic construction consists of two PN-junctions producing three connecting terminals with each terminal being given a name to identify it from the other two. These three terminals are known and labelled as the Emitter ( E ), the Base ( B ) and the Collector ( C ) respectively.

Bipolar Transistors are current regulating devices that control the amount of current flowing through them from the Emitter to the Collector terminals in proportion to the amount of biasing voltage applied to their base terminal, thus acting like a current-controlled switch. As a small current flowing into the base terminal controls a much larger collector current forming the basis of transistor action.

The principle of operation of the two transistor types PNP and NPN, is exactly the same the only difference being in their biasing and the polarity of the power supply for each type.

### Bipolar Transistor Construction

![[BJT terminals.png|white]]

The construction and circuit symbols for both the PNP and NPN bipolar transistor are given above with the arrow in the circuit symbol always showing the direction of “conventional current flow” between the base terminal and its emitter terminal. The direction of the arrow always points from the positive P-type region to the negative N-type region for both transistor types, exactly the same as for the standard diode symbol.

## Bipolar Transistor Configurations

As the **Bipolar Transistor** is a three terminal device, there are basically three possible ways to connect it within an electronic circuit with one terminal being common to both the input and output signals. Each method of connection responding differently to its input signal within a circuit as the static characteristics of the transistor vary with each circuit arrangement.

- Common Base Configuration   –   has Voltage Gain but no Current Gain.
- Common Emitter Configuration   –   has both Current and Voltage Gain.
- Common Collector Configuration   –   has Current Gain but no Voltage Gain.

## The Common Base (CB) Configuration

As its name suggests, in the **Common Base** or grounded base configuration, the BASE connection is common to both the input signal AND the output signal. The input signal is applied between the transistors base and the emitter terminals, while the corresponding output signal is taken from between the base and the collector terminals as shown. The base terminal is grounded or can be connected to some fixed reference voltage point.

The input current flowing into the emitter is quite large as its the sum of both the base current and collector current respectively therefore, the collector current output is less than the emitter current input resulting in a current gain for this type of circuit of “1” (unity) or less, in other words the common base configuration “attenuates” the input signal.

### The Common Base Transistor Circuit

<img src="https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran2.gif "Common Base Configuration"" style="background-color:white;" />


This type of amplifier configuration is a non-inverting voltage amplifier circuit, in that the signal voltages Vin and Vout are “in-phase”. This type of transistor arrangement is not very common due to its unusually high voltage gain characteristics. Its input characteristics represent that of a forward biased diode while the output characteristics represent that of an illuminated photo-diode.

Also this type of bipolar transistor configuration has a high ratio of output to input resistance or more importantly “load” resistance ( RL ) to “input” resistance ( Rin ) giving it a value of “Resistance Gain”. Then the voltage gain ( Av ) for a common base configuration is therefore given as:

### Common Base Voltage Gain

![common base transistor gain](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran30.gif "Common Base Transistor Voltage Gain")

Where: Ic/Ie is the current gain, alpha ( α ) and RL/Rin is the resistance gain.

The common base circuit is generally only used in single stage amplifier circuits such as microphone pre-amplifier or radio frequency ( Rƒ ) amplifiers due to its very good high frequency response.

#### **Common base output characteristics**

It is the curve between collector current IC and collector base voltage VCB at constant emitter current IE .Collector current is taken along y – axis and collector base voltage along x – axis.

![](https://specbee.net/wp-content/uploads/2022/06/output-common-base-300x268.jpg)

The collector current varies with  only at very low voltages and the transistor is never operate in this region. When the value of VCB is resist above 1 to 2 volt the collector current becomes constant. That means now IC is independent of VCB and depends upon IE only.

A very large change in collector base voltage produces only a small change in collector current. This means the output resistance very high.

So output resistance ro = ΔVCB / ΔIC    , at constant IE .

## The Common Emitter (CE) Configuration

In the **Common Emitter** or grounded emitter configuration, the input signal is applied between the base and the emitter, while the output is taken from between the collector and the emitter as shown. This type of configuration is the most commonly used circuit for transistor based amplifiers and which represents the “normal” method of bipolar transistor connection.

The common emitter amplifier configuration produces the highest current and power gain of all the three bipolar transistor configurations. This is mainly because the input impedance is LOW as it is connected to a forward biased PN-junction, while the output impedance is HIGH as it is taken from a reverse biased PN-junction.

### The Common Emitter Amplifier Circuit

<img src="https://www.electronics-tutorials.ws/wp-content/uploads/2021/03/tran3.gif "Common Emitter Configuration"" style="background-color:white;" />
In this type of configuration, the current flowing out of the transistor must be equal to the currents flowing into the transistor as the emitter current is given as Ie = Ic + Ib.

As the load resistance ( RL ) is connected in series with the collector, the current gain of the common emitter transistor configuration is quite large as it is the ratio of Ic/Ib. A transistors current gain is given the Greek symbol of Beta, ( β ).

As the emitter current for a common emitter configuration is defined as Ie = Ic + Ib, the ratio of Ic/Ie is called Alpha, given the Greek symbol of α. Note: that the value of Alpha will always be less than unity.

Since the electrical relationship between these three currents, Ib, Ic and Ie is determined by the physical construction of the transistor itself, any small change in the base current ( Ib ), will result in a much larger change in the collector current ( Ic ).

Then, small changes in current flowing in the base will thus control the current in the emitter-collector circuit. Typically, Beta has a value between 20 and 200 for most general purpose transistors. So if a transistor has a Beta value of say 100, then one electron will flow from the base terminal for every 100 electrons flowing between the emitter-collector terminal.

By combining the expressions for both Alpha, α and Beta, β the mathematical relationship between these parameters and therefore the current gain of the transistor can be given as:

![bipolar transistor alpha beta relationship](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran31.gif "Bipolar Transistor Alpha Beta Relationship")

![common emitter current gain](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran25.gif "Common Emitter Current Gain")

Where: “Ic” is the current flowing into the collector terminal, “Ib” is the current flowing into the base terminal and “Ie” is the current flowing out of the emitter terminal.

Then to summarise a little. This type of bipolar transistor configuration has a greater input impedance, current and power gain than that of the common base configuration but its voltage gain is much lower. The common emitter configuration is an inverting amplifier circuit. This means that the resulting output signal has a 180o phase-shift with regards to the input voltage signal.

#### **Common emitter input characteristics**

![](https://specbee.net/wp-content/uploads/2022/06/input-common-emitter-300x212.jpg)

It is the curve between base current and base emitter voltage a constant collector emitter **[voltage](https://en.wikipedia.org/wiki/Voltage)**.

Keeping VCE is constant the base current value note for various values of VBE .then plotting the readings taking IB along y – axis and VBE along x – axis. This characteristic same as the forward bias diode curve. As compare to common base IB increases less rapidly with VBE .

Therefore input resistance of a common emitter circuit is higher than common base circuit.

Input resistance ri = ΔVBE / ΔIB   ,  at constant VCE . The value of input resistance is the order of a ( few 100 Ω )

#### **Common emitter output characteristics**

![](https://specbee.net/wp-content/uploads/2022/06/output-common-emitter-configuration-2-300x278.jpg)

It is the curve between collector current  and collector emitter voltage  at constant base current IB .                                                Keeping the base current IB constant and then collector current is note for various value of VCE .Then plotting the readings taking IC along y – axis and VCE along x – axis .

The collector current IC varies with VCE for VCE between 0 and 1Volt only after this IC becomes almost constant and independent of VCE .This value of VCE up to which collector current IC changes with VCE is called the knee voltage ( Vknee ).The transistor are always operated in the region above knee voltage. 

However a small increase in IC with increasing VCE is cause by the collector depletion layer getting and capture in a few of more majority charge carrier before hole.

For any value of VCE above knee voltage collector current IC ≅ β × IB .Where β is the current amplification factor for common emitter connection.

 Output resistance ro = ΔVCE / ΔIC  at constant IB .So the output resistance is the order of 50 kΩ.

## The Common Collector (CC) Configuration

In the **Common Collector** or grounded collector configuration, the collector is connected to ground through the supply, thus the collector terminal is common to both the input and the output. The input signal is connected directly to the base terminal, while the output signal is taken from across the emitter load resistor as shown. This type of configuration is commonly known as a **Voltage Follower** or **Emitter Follower** circuit.

The common collector, or emitter follower configuration is very useful for impedance matching applications because of its very high input impedance, in the region of hundreds of thousands of Ohms while having a relatively low output impedance.

### The Common Collector Transistor Circuit

<img src="https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran4.gif "Common Collector Configuration"" style="background-color:white;" />

The common emitter configuration has a current gain approximately equal to the β value of the transistor itself. However in the common collector configuration, the load resistance is connected in series with the emitter terminal so its current is equal to that of the emitter current.

As the emitter current is the combination of the collector AND the base current combined, the load resistance in this type of transistor configuration also has both the collector current and the input current of the base flowing through it. Then the current gain of the circuit is given as:

### The Common Collector Current Gain

<img src="https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran32.gif "Common Collector Gain"" style="background-color:white"/>

![Common Collector Current Gain](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran32a.gif "Common Collector Current Gain")

This type of bipolar transistor configuration is a non-inverting circuit in that the signal voltages of Vin and Vout are “in-phase”. The common collector configuration has a voltage gain of about “1” (unity gain). Thus it can considered as a voltage-buffer since the voltage gain is unity.

The load resistance of the common collector transistor receives both the base and collector currents giving a large current gain (as with the common emitter configuration) therefore, providing good current amplification with very little voltage gain.

Having looked at the three different types of bipolar transistor configurations, we can now summarise the various relationships between the transistors individual DC currents flowing through each leg and its DC current gains given above in the following table.

#### **Common collector input characteristics**

![](https://specbee.net/wp-content/uploads/2022/06/input-characteristics-common-collector-1-300x213.jpg)

It is the curve between base **[current](https://en.wikipedia.org/wiki/Electric_current)**  and base collector voltage  a constant emitter collector voltage . Here in this curve the input variable is IB , VCB and the output variable VCE is present.

IB = Input Current , VCB = Input Voltage , VCE = Output Voltage

Keeping VCE is constant at 2V and the base current value is note for various value of VCB  Then plotting the readings taking IB along y – axis and VCB along x – axis. We again keeping VCE is constant at 4V and note down the base current value for different values of VCB, then plot the readings.

#### **Common collector output characteristics**

It is the curve between emitter current IE and emitter collector voltage VCE at constant base current IB . So in this curve we get 3 regions you can see in the graph.

![](https://specbee.net/wp-content/uploads/2022/06/output-common-collector-300x277.jpg)

So first we will keep the base current IB as constant and note the emitter **[current](https://en.wikipedia.org/wiki/Electric_current)** IE for various value of VCE . Now we will increase the base current from 0.  

When the base current is 0 then the transistor also 0 no current will flow, so we call it cut off region. Now the base current is 0, so we will gradually increase it from 0 to 5 μA, after that 10 μA, 15 μA like this, so from this we will call active region. And now the value of IB = 20 μA it means a lot of current is flowing, so obviously the transistor will also have a lot of current flowing through it, due to which we call saturation region.

### Relationship between DC Currents and Gains

|   |   |
|---|---|
|![transistor currents](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran75.gif "Transistor Currents")|![transistor alpha and beta equations](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran76.gif "Transistor Alpha and Beta Equations")|
|![transistor base currents](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran77.gif "Transistor Base Currents")|   |
|![transistor collector currents](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran78.gif "Transistor Collector Currents")|![transistor emitter currents](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/transistor-tran79.gif "Transistor Emitter Currents")|

Note that although we have looked at _NPN Bipolar Transistor_ configurations here, PNP transistors are just as valid to use in each configuration as the calculations will all be the same, as for the non-inverting of the amplified signal. The only difference will be in the voltage polarities and current directions.

## Bipolar Transistor Summary

Then to summarise, the behaviour of the bipolar transistor in each one of the above circuit configurations is very different and produces different circuit characteristics with regards to input impedance, output impedance and gain whether this is voltage gain, current gain or power gain and this is summarised in the table below.

### Bipolar Transistor Configurations

<img src="https://www.electronics-tutorials.ws/wp-content/uploads/2020/04/tran54.gif "Bipolar Transistor Configurations"" style="background-color:white"/>

with the generalised characteristics of the different transistor configurations given in the following table:

|   |   |   |   |
|---|---|---|---|
|Characteristic|Common  <br>Base|Common  <br>Emitter|Common  <br>Collector|
|Input Impedance|Low|Medium|High|
|Output Impedance|Very High|High|Low|
|Phase Shift|0o|180o|0o|
|Voltage Gain|High|Medium|Low|
|Current Gain|Low|Medium|High|
|Power Gain|Low|Very High|Medium|

In the next tutorial about **Bipolar Transistors**, we will look at the NPN Transistor in more detail when used in the common emitter configuration as an amplifier as this is the most widely used configuration due to its flexibility and high gain. We will also plot the output characteristics curves commonly associated with amplifier circuits as a function of the collector current to the base current.



 VCE = VCC − IC ( RC + RE )