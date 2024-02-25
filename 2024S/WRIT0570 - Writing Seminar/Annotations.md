---
date: 2024-02-24
type: note
tags: 
---

# Article 1
[The hidden costs of AI: Impending energy and resource strain | Penn Today](https://penntoday.upenn.edu/news/hidden-costs-ai-impending-energy-and-resource-strain)

This article focuses on the energy and resource costs that AI computing will bring in the near-term future. According to Professor Deep Jariwala and Benjamin Lee at the University of Pennsylvania, AI will bring about massive challenges in memory and energy usage. This is useful for my research because it confirms that there is a problem in accelerating AI developments, and that experts in AI, computing, and electrical engineering agree that this a major problem that is being under looked.

Intro:
- As AI become more elaborate and data-intensive, two things begin to scale up exponentially: the need for more memory storage and the need for more energy.
- The rise of AI, Big Data, and cloud computing has led to significant growth in data centers.
- Recent NVIDIA earnings' report state a 404% growth in data center revenues within the past 10 years.
- Moore’s law states that the number of transistors on a chip—the parts that control the flow of electrons on a semiconductor material—doubles every two or so years.
- Dennard’s scaling suggests that doubling the number of transistors effectively means shrinking them but also maintaining their power density, so smaller chips meant more energy-efficient chips.

Problem:
- Regarding memory, an estimate from the Semiconductor Research Corporation, a consortium of all the major semiconductor companies, posits that if we continue to scale data at this rate, which is stored on memory made from silicon, we will outpace the global amount of silicon produced every year. So, pretty soon we will hit a wall where our silicon supply chains won’t be able to keep up with the amount of data being generated.
- Couple this with the fact that in 2018 our computers consumed roughly 1-2% of the global electricity supply, and in 2020, this figure was estimated to be around 4–6%. If we continue at this rate, by 2030, it's projected to rise between 8-21%, further exacerbating the current energy crisis.
- Companies like Amazon, Google, and Meta have been building more and more of these massive facilities all over the country. In fact, data center power and carbon emissions associated with data centers doubled between 2017 and 2020. Each facility consumes in the order of 20 megawatts up to 40 megawatts of power, and most of the time data centers are running at 100% utilization, meaning all the processors are being kept busy with some work. So, a 20-megawatt facility probably draws 20 megawatts fairly consistently—enough to power roughly 16,000 households.
- Then there’s the embodied carbon footprint, which is associated with construction and manufacturing. This hearkens back to building new semiconductor foundries and packaging all the chips we’ll need to produce to keep up with increasing compute demand. These processes in and of themselves are extremely energy-intensive, expensive and have a carbon impact at each step.
- Moore's Law and Dennard's scaling have started to slow down for several reasons related to the physical limits of the materials we use.

Solutions:
- Each computational task is a transaction between memory and processing that requires some energy. Deep Jariwala's lab is trying to figure out ways to make each operation use fewer watts of power. One way to reduce this metric is through tightly integrating memory and processing units because these currently exist in two separate locations that are millimeters to centimeters apart so electricity needs to travel great distances to facilitate computation which makes it energy and time inefficient. We call it vertically heterogenous-integrated architecture, and developing this is key to reducing energy consumption.

Conclusions:
- Our computers and other devices are becoming insatiable energy beasts that we continue to feed. That’s not to say AI and advancing it needs to stop because it’s incredibly useful for important applications like accelerating the discovery of therapeutics. We just need to remain cognizant of the effects and keep pushing for more sustainable approaches to design, manufacturing, and consumption.

# Article 2
[Brain organoid reservoir computing for artificial intelligence | Nature Electronics](https://www.nature.com/articles/s41928-023-01069-w)

This article focuses on a new method of computing: using biology to create biologics-based computing. This method will bring about a new form of energy-efficiency and power-efficiency previously unseen in traditional silicon chips. This is useful for my research because it is 1 very interesting and unique method of solving this problem of creating more energy-efficient, power-efficient, and climate friendly semiconductor chip. This will be 1 of the 3 major ways to tackle the issue I am exploring in my white paper: "Current methods and solutions to solving the energy demands caused by the explosive growth of AI".

Intro:
- AI success is driven by the development of artificial neural networks (ANNs).
- Slowing of Moore's law places limitations of current AI hardware, and thus new developments in AI hardware is needed.
- The human brain is a complex 3D biological network of 200 billion cells, linked by hundreds of trillions of synapses, and expands 20 watts while AI hardware consumes about 8 million watts to drive a comparative ANN. [Source](https://www.nature.com/articles/s41586-021-04362-w)
- Brain organoid are in-vitro 3D aggregates created through the self-organization and differentiation of human iPSC cells.

Problem:
- Training ANNs on current AI computing hardware is energy intensive and time consuming.
- A key problem is the physical separation of data from data processing units. This is the von Neumann bottleneck.
- Current computing approaches require high training cost to process and learn information from noisy data.

Solution:
- The brain can effectively process and learn information from noisy data at minimal training cost through neuronal plasticity and neurogenesis, and thus avoids large energy demands.
- The brain fuses data storage and processes within biological neural networks, which bypasses von Neumann bottleneck issues. Current neuromorphic chips use memristors to mimic BNNs.
- Current neuromorphic chips can have been used in computer vision and speech recognition. [Source1](https://doi.org/10.1038%2Fncomms15199), [Source2](https://doi.org/10.1038%2Fs41928-017-0002-z), [Source3](https://doi.org/10.1038%2Fs41928-019-0313-3)
- This article leverages "reservoir computation" and the unsupervised learning ability of organoid neural networks in a brain organoid. [Fig. 1: Brainoware with unsupervised learning for AI computing. | Nature Electronics](https://www.nature.com/articles/s41928-023-01069-w/figures/1)
- The Brainoware was created by mounting a brain organoid onto a MEA chip. The human brain organoid had early and mature neurons, astrocytes, and neuron progenitor cells, and early development of brain-like structures. The ONN received inputs via external electrical stimulation and sent outputs via evoked neural activity.
- They used a "conventional reservoir computing hardware," but ONNs benefit because the organoid can function as an adaptive living reservoir to conduct unsupervised learning - and thus improve computing performance over the long run. This is due to neuroplasticity.
- Physical reservoir properties of Brainoware was tested ([Image](https://www.nature.com/articles/s41928-023-01069-w/figures/2)):
	- Nonlinear dynamics: by checking the resposne of ONNs to bipolar voltage pulse stimulations of different pulse times and voltages. The evoked neuronal activity was recorded as a raster plot. They found that after a single voltage pulse stimulation, the evoked electrical response can be fitted with a sigmoid function.
	- Fading memory: applying pulses with different times and voltages - found that longer pulses with higher voltage led to stronger evoked resopnse and relaxation dynamics.
	- Spatial information processing: spatial info was converted into spatial patterns of simulation pulses, and raster plots of evoked signals showed active storage and gradual loss of different spatial information over time.
- Brainoware could perform real-world time-series tasks such as speech recognition ([Image](https://media.springernature.com/lw685/springer-static/image/art%3A10.1038%2Fs41928-023-01069-w/MediaObjects/41928_2023_1069_Fig3_HTML.png?as=webp)):
	- Distinguished vowels from sentences. Audio clips were converted into spatiotemporal sequences of stimulation bipolar pulses and applied to Brainoware. Evoked ONN activity was recorded and fed into a logistic regression function for classification, then trained and optimized.
	- A confusion matrix was recorded to test for accuracy pre-training and post-training.

Conclusion:
- Human brain organoid can self-organize and form functional ONNs to create reservoir computing hardware that can self-learn due to plasticity. This approach means less time and energy consumption and less heat production compared to current AI hardware.
- Limitations include:
	- Generation and maintenance of organoid - suffer from high heterogeneity, low generation throughput, necrosis/hypoxia
	- Peripheral equipment needed to power Brainoware (CO2 incubator, computer) still consumes considerable power.
	- Soft and flexible MEAs/electrodes to interface the entire organoid will allow greater manipulation of greater neurons.

Methods:
- Cortical organoids generated from human iPSCs adapted from [Protocol1](https://doi.org/10.1016%2Fj.stem.2019.08.002) and [Protocol2](https://doi.org/10.1002%2Fadvs.202200475). More information here: [Link](https://static-content.springer.com/esm/art%3A10.1038%2Fs41928-023-01069-w/MediaObjects/41928_2023_1069_MOESM1_ESM.pdf)
- Ethical handling of stem cells and organoids followed from WiCell Institute and Indiana University Biosafety Committee.
- MaxOne MEA System was used for interfacing. Python and Maxlive were used to analyze information. Maxlive generates stimulation sequence and recording the activity, Python extracts and processes the spikes.
- The input layer converts info (images, audio clips, time series) into spatiotemporal sequences of electrical stimulation pulses to the organoid (reservoir layer), which receives the inputs and the neural activities (represents the reservoir state) was fed into the decoding function (linear regression or logistic regression) as an output for classification, recognition, prediction, etc.

# Article 3
[Reservoir computing with brain organoids | Nature Electronics](https://www.nature.com/articles/s41928-023-01096-7)

# Article 4
[How thermal management is changing in the 1 kW chip age • The Register](https://www.theregister.com/2023/12/26/thermal_management_is_changing/)

# Article 5
[Pathways to cellular supremacy in biocomputing | Nature Communications](https://www.nature.com/articles/s41467-019-13232-z)

# Article 6
[Computing Power and the Governance of AI | GovAI Blog](https://www.governance.ai/post/computing-power-and-the-governance-of-ai)

# Article 7
[Navigating the High Cost of AI Compute | Andreessen Horowitz](https://a16z.com/navigating-the-high-cost-of-ai-compute/)

# Article 8
[Bridging Biological and Artificial Neural Networks with Emerging Neuromorphic Devices: Fundamentals, Progress, and Challenges - Tang - 2019 - Advanced Materials - Wiley Online Library](https://onlinelibrary.wiley.com/doi/10.1002/adma.201902761)

This article explores bridging biology with ANNs for emerging neuromorphic chip designs. This is useful for my research because it is the main focus of my paper, which essentially argues for the push towards neuromorphic-inspired chip designs. This article is important for giving a broad overview of the fundamentals of this chip design, the progress in recent decades, and why this hasn't taken off.

Intro: 
- The boom of AI is driven by GPUs to implement the training of ANNs and back propagation.
- Brain computing is a new computing paradigm to enable massively parallel analog computing.
- The human brain is a mesh of different neural networks organized to support computational functions like vision, audition, emotion, etc. The basic unit is a neuron, which has dendrites to receive inputs and axons to send outputs, connected by synapses.

Problem:
- The speed and energy efficiency of silicon CMOS-based computing hardware is approaching its theoretical limit - hindered by the slowing of Moore's law scaling and the von Neumann bottleneck, which increases the cost for big data movements.
- The performance gap between memory and processors is known as the memory wall problem, and is expanding.
- Even though IBM and Intel neuromorphic chips bypasses the von Neumann bottleneck, they use complex circuit architectures that are power-hungry, and have limits in scalability due to silicon shortages and CMOS scaling problem.

Solution:
- This new type of "resistive processing unit" (RPU) can provide a 30000x acceleration compared to current CPU/GPU in training deep neural networks (DNNs).
- IBM's TrueNorth chip and Intel's Loihi chips include "neuromorphic cores" with spiking neural units based on spike neural networks.
- The nervous system use two very important principles - parallel streams and hierarchical processing - to organize computations.