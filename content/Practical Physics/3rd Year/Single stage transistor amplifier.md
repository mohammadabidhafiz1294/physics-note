When only a single transistor is used with an associated circuit to amplify a weak signal, the circuit is known as a single stage transistor amplifier.    

The single stage transistor amplifier consists of a transistor, bias circuit and other auxiliary components. there are many stages in a practical amplifier, However such a complex circuits can be easily divided into separate single phase. 

By analyzing just one stage and using this single stage analysis, we can analyze complex circuits effectively. Therefore single stage amplifier analysis is very important to understand practical amplifier circuits.

![](https://specbee.net/wp-content/uploads/2022/04/ssta-1-2.webp)

In a single stage transistor amplifier, When a weak a. c. signal is given to the base of the transistor a small base current begins to flow. This happen because of the transistor action, a very large current start to flows through the collector load RC .

Since the value of the RC is very high, So a large voltage appears across the RC . Thus a weak signal applied in the base circuit gets amplified in the collector circuit. In this way a transistor acts as an amplifier.

For [**what is the filter circuit?**](https://specbee.net/filter-circuit/) 

### **Practical circuit of transistor amplifier**

![What is Single Stage Transistor Amplifier?](https://specbee.net/wp-content/uploads/2022/04/Untitled-design-1-300x169.webp)

The various circuit elements connected in this circuit are

1. **Biasing circuit**
2. **Input capacitor Cin**
3. **Emitter bypass capacitor CE**
4. **Coupling capacitor CC**

Now we will go through four different circuit elements, so let’s start :-

#### **(1) Biasing circuit :**

The resistance R1 , R2 and RE form the biasing and stabilization circuit.

#### **(2) Input capacitor Cin :**

In electrolytic capacitors Cin  is use to connect the signal to the base of the transistor. If this is not use the signal will come across the **[source](https://en.wikipedia.org/wiki/Source)** resistance R2 , and thus change the bias.

#### **(3) Emitter bypass capacitor CE :**

It is use in parallel with RE to provide a low reactance path to the amplified a. c. signal. If it is not use then amplified a. c. The signal flowing through RE will cause a voltage drop across it. Thereby reducing the output voltage.

#### **(4) Coupling capacitor C**C :

It connects one stage of amplification to the next. If it is not use then the bias condition of the next stage will change due to the shunting effect of RC.

So the coupling capacitor isolates D. C. from one stage to the next. So here Various circuit currents flowing through the amplifying circuit are **(i) Base current (ii) collector current and (iii) Emitter current.**

### **Base current** 

When no signal is applied to the base circuit d. c. The **[biasing](https://en.wikipedia.org/wiki/Biasing)** circuit causes the current to flow through IB when a. c. The signal is applied a. c. Base current ib also flows through.

So the total base current  iB = IB = ib .

### **Collector current**

When no signal is applied d. c. The collector current flows through the IC because of the biasing circuit when a. c. The signal is applied a. c. The **[collector current](https://en.wikipedia.org/wiki/Bipolar_junction_transistor)** also flows through the small ic .

So the total collector current  iC = IC + ic

### **Emitter current**

When no signal is apply d. c. **[Emitter current](https://en.wikipedia.org/wiki/Bipolar_junction_transistor)** flows through IE . So total emitter current IE is  iE = IE = ie .

### **What is a phase reversal ?**

The phase difference of 180 degrees between the signal voltage and the output voltage in a common emitter amplified is called phase reversal.

![What is Single Stage Transistor Amplifier?](https://specbee.net/wp-content/uploads/2022/04/Untitled-design-1-1-300x169.webp)

For **[transistor configuration](https://specbee.net/transistor-configuration/)**

### **DC and AC equivalent circuit of** **single stage transistor** **amplifier**

In the d. c. analysis we consider all the d. c. **[source](https://en.wikipedia.org/wiki/Source)** at the same time and work out the d. c. current and voltages in the circuit. In a. c. analysis we consider all the a. c. source at the same time and work out the a. c. current and voltages.

####  **(1) DC equivalent circuit** 

![What is Single Stage Transistor Amplifier?](https://specbee.net/wp-content/uploads/2022/04/DC-227x300-1.webp)

In d. c. **[equivalent circuit](https://en.wikipedia.org/wiki/Equivalent_circuit)** only d. c. conditions are to be considered. As in D.C. Current cannot flow through a capacitor so all capacitors look like open circuits. Therefore draw the equivalent circuit.

1. Reduce all a. c. sources to zero.
2. Open all the capacitor. 

#### **(2) AC equivalent circuit**

![](https://specbee.net/wp-content/uploads/2022/04/ac-300x150-1.webp)

In a. c. equivalent circuit only a. c. conditions are to be consider. Therefore in order to draw the a. c. equivalent circuit.

1. Reduce all d. c. sources to zero ( For example VCC = 0 ).
2. Short all the capacitor.

### **Load line analysis** **of single stage transistor amplifier**

The points lying on the load line give the possible value of VCE and IC in the output circuit. As in a transistor circuit both d. c. and a. c. condition exist, therefore there are two types of load line namely.

1. **d. c. load line**
2. **a. c. load line**

#### **(1)  d. c. load line** 

It is the line on the output characteristics of a transistor circuit which is the value of IC and VCE corresponding to zero signal or d. c. conditions.

![What is Single Stage Transistor Amplifier?](https://specbee.net/wp-content/uploads/2022/04/DC-LOAD-LINE-300x191-1.webp)

By applying  KVL ,  VCE = VCC − IC RC − IE RE 

                               or ,    VCE = VCC − IC ( RC + RE )

 VCC and (RC + RE ) are constant for the given circuit.

The value of VCE will be maximum when IC =0.

So maximum VCE = VCC .

It locate the first point B ( OB = VCC ) of the d. c. load line.

So the value of IC will be maximum, when VCE = 0.

VCC = IC (RC + RE )

Maximum IC = VCC / RC + RE

This locates the second point A (OA = VCC / RC + RE) of the d. c. load line.

Joining the points A and B, d. c. The load line AB has been constructed.

![](https://specbee.net/wp-content/uploads/2022/04/DC-LOAD-LINE1-300x178-1.webp)

Actual operating conditions in the circuit will be represent by the point where d. c. load line intersects the base current curve.

If IB = 5μA is set by the biasing circuit then ‘Q’ is the operating point as shown in figure.

#### **(2) a. c. load line** 

It is the line at output characteristic of a transistor circuit that gives the value of IC and VCE when the signal is applied.

![What is Single Stage Transistor Amplifier?](https://specbee.net/wp-content/uploads/2022/04/ac-load-line-300x186-1.webp)

To add a. c. for output characteristic of load line we again need two end point maximum VCE and maximum IC point.

Under the application of a. c. signal maximum

VCE = VCE + IC RAC 

RAC = RC || RL = RC RL / RC + RL

It locates the point ‘C’ of a. c. load line on VCE axis.

Maximum IC = IC + VCE / RAC

It locate the point ‘D’ of a. c. load line on the IC axis by connecting points ‘C’ and ‘D’ a. c. load line is construct.

![](https://specbee.net/wp-content/uploads/2022/04/AC-LOAD-LINE-1-300x278-1.webp)

### **What is the voltage gain in Single Stage Transistor Amplifier**

The voltage gain of the amplifier is the ratio of a. c. output voltage to the a. c. input signal voltage.

As a. c. signal is concerned load RC appears in parallel with RL . Therefore effective load line.

a. c. load, RAC = RC || RL = RC × RL / RC + RL

Output voltage , Vout = ic × RAC

Input voltage , Vin = ib × Rin

Voltage gain , Av = Vout / Vin 

Av = ic × RAC / ib × Rin = β × RAC / Rin 

**Where , ic / ib = β**

The power gain is  AP = ( ic )2 × RAC / ( ib )2  × Rin = β2 × RAC / Rin