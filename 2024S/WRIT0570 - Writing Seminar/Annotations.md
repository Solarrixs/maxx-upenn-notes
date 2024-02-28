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

This article explores a concept for computing using brain organoids under the reservoir computing model. This article is important for my research because it highlights one method to utilize the human brain for actual computing purposes, and demonstrates both its benefits and limitations over current methods.

Intro:
- Several groups are developing brain-like, energy efficient biocomputers using brain organoids with electrical sensors and tools for signal processing and decoding.
- With advances in cell culturing techniques, bioengineering technologies, and AI, biological computing is poised to emerge.
- Brain organoids can be stimulated electrically, chemically, or optically.
- Reservoir computing is a framework for training recurrent neural networks (RNNs). The reservoir is fixed, and only readout weights are trained.

Problem:
- It's hard to develop and maintain brain organoids with the following features needed for optimal compute:
	- Being able to maintain high complexity of large and interconnected neuron network supported by non-neuronal brain cells
	- Energy sources and efficient techniques for maintaining culture temp and culture medium
	- Maintaining cultures require resource-intensive incubators with temperature and environmental control and skilled biologists. However, with continued miniaturization and maturation of cell culturing platforms, this will be a problem that can be solved.

Solution:
- Brain stimuli can be recorded using shanks, high density MEAs, mesh electrodes, shell electrodes and nanowires.

Conclusions:
- In the next few years, increasingly complex neural systems that can interact with AI environments will emerge, and generate massive energy savings.

# Article 4
[How thermal management is changing in the 1 kW chip age • The Register](https://www.theregister.com/2023/12/26/thermal_management_is_changing/)

This article explores the slowing down of Moore's law and the heat inefficiencies of current silicon based CMOS chip designs. This is useful for my research because it focuses on the problem of using silicon based CMOS chip designs - which suffers from 3 major bottlenecks: heat dissipation, memory gap performances from von Neumann bottlenecks, and slowing of Moore's Law with limited supply of silicon. It will make up a bulk of the problem surrounding my white paper.

Intro:
- AI chips and chips in general release heat as a byproduct of computing.

Problem:
- Nvidia GH200 AI chips use kilowatts of energy.
- There is a trend of increasing 0.5 - 1 kW of rack units for systems. This means 21-24 kW of thermal load needs to be dissipated (which is obtainable).
- Hotter chips requires faster fans that draws more power - using up to 20% of the system power in some cases.
- New racks requires multi-kW cooling systems: upto 40+ kW of power for cooling.
- AMD's accelerators jump from 560W to 760W. That's a sizable increase.

Solution:
- Liquid cooling offers efficient cooling mechanisms.

Conclusion:
- Chips will get hotter and this trend is likely to continue. New methods in cooling will need to be developed for these chips.

# Article 5
[AI's Climate Impact Goes beyond Its Emissions | Scientific American](https://www.scientificamerican.com/article/ais-climate-impact-goes-beyond-its-emissions/)

Problem:
- "Training and running an AI system requires a great deal of computing power and electricity, and the resulting carbon dioxide emissions is one way AI can affect the climate"

# Article 6
[Computing Power and the Governance of AI | GovAI Blog](https://www.governance.ai/post/computing-power-and-the-governance-of-ai)

Although focusing on the regulation of AI through computing power as a metric, it still explores a good problem of computing power. This article assists in my research as I can understand the basis behind computing power, which essentially is the main problem behind energy-inefficient chip architecture. This article is taken from "Computing Power and the Governance of AI" from 19 researchers globally, including several from OpenAI.

Intro:
- Computing power drives AI progress. The amount of compute used to train AI systems has increased 350 million times in the past 13 years.
- Across LLMs, Go, protein folding, and autonomous vehicles, vast amounts of compute power was needed.
- There is many scaling laws: performance on training objective increases as the amount of compute used to train a model increases.
- Numbers of operations (FLOP) measures compute.
- Current AI systems and models require the doubling of compute every 6 months.
- [Image](https://assets-global.website-files.com/614b70a71b9f71c9c240c7a7/65cb86a074a06055791f02e9_ucMaHPVGyL9o4brHsIlmNiTb7TrtFOLzGpyCtEm6aR9CEqVAiltVT1UOawTibe5fesBj0vKLXXGKmvh5JI3_Nm7MuMmifyWSroiHcFDunIWVp0a53YPy_4igwCRrQX-xdQToP4CYfN-pxwr939DFYQY.jpeg)
- Compute is distributed from production, provision, and usage to final deployment: [Image](https://assets-global.website-files.com/614b70a71b9f71c9c240c7a7/65cb90abfced58be2e835b3d_CPGAI_Figure_The-Compute-Supply-Chain.jpg)

# Article 7
[Navigating the High Cost of AI Compute | Andreessen Horowitz](https://a16z.com/navigating-the-high-cost-of-ai-compute/)

Similar to the above article, this article focuses on compute as a key driver of AI progress. However, since compute is physically bounded to AI progress, measuring compute provides insights into the state of AI in 2023 and beyond. This article assists in my research for the reasons above - understanding the basis of AI energy demands and supply.

Intro:
- AI is compute-bound. More compute directly results in a better product.
- Most AI models are based on transformers. For a model with p parameters for an input and an output sequence of n tokens, then 2np is the number of FLOPs. Training a model takes 6p FLOPS per n token as well. Total training cost can be estimated.
- A 175B parameter model will need over 1TB of data in memory. This exceeds any GPUs in existence today and requires the model to be split across multiple cards.

Problem:
- According to a16z, the supply of compute is so constrained that demands outstrips it by a factor of 10x. Therefore, access to compute at the lowest cost is a determining factor for the success of AI companies.
- Companies spend 80% of their total capital on compute resource.
- [Tim Dettmer's analysis](https://timdettmers.com/2023/01/16/which-gpu-for-deep-learning/) allows one to calculate the price/performance analysis of GPUs for your own data center.

Solution:
- Large compute buyers commit minimum spending and minimum time commitments (1-3 years).
- GPU cost by cloud provider: [Image](https://a16z.com/wp-content/uploads/2023/04/3.-Prices-for-common-GPU-types-by-cloud-provider.png)
- GPU performance will increase at a slower rate; Moore's Law is semi-intact but power is a limiting factor instead. However, the growth of the AI industry and number of AI developers will fuel a demands for GPUs. There is no sign that the GPU shortage we have today will abate in the near future.

# Article 8
[Bridging Biological and Artificial Neural Networks with Emerging Neuromorphic Devices: Fundamentals, Progress, and Challenges - Tang - 2019 - Advanced Materials - Wiley Online Library](https://onlinelibrary.wiley.com/doi/10.1002/adma.201902761)

This article explores bridging biology with ANNs for emerging neuromorphic chip designs. This is useful for my research because it is the main focus of my paper, which essentially argues for the push towards neuromorphic-inspired chip designs. This article is important for giving a broad overview of the fundamentals of this chip design, the progress in recent decades, and why this hasn't taken off.

Intro: 
- The boom of AI is driven by GPUs to implement the training of ANNs and back propagation.
- Brain computing is a new computing paradigm to enable massively parallel analog computing.
- The human brain is a mesh of different neural networks organized to support computational functions like vision, audition, emotion, etc. The basic unit is a neuron, which has dendrites to receive inputs and axons to send outputs, connected by synapses.
- Neurons act as capacitors with reconfigurable resistors. The firing of a neuron is the generation of an action potential, once there is sufficient excitation over a certain threshold and period.

Problem:
- The speed and energy efficiency of silicon CMOS-based computing hardware is approaching its theoretical limit - hindered by the slowing of Moore's law scaling and the von Neumann bottleneck, which increases the cost for big data movements.
- The performance gap between memory and processors is known as the memory wall problem, and is expanding.
- Even though IBM and Intel neuromorphic chips bypasses the von Neumann bottleneck, they use complex circuit architectures that are power-hungry, and have limits in scalability due to silicon shortages and CMOS scaling problem.

Solution:
- This new type of "resistive processing unit" (RPU) can provide a 30000x acceleration compared to current CPU/GPU in training deep neural networks (DNNs).
- IBM's TrueNorth chip and Intel's Loihi chips include "neuromorphic cores" with spiking neural units based on spike neural networks.
- The nervous system use two very important principles - parallel streams and hierarchical processing - to organize computations.
- Multiple new paradigms in ANNs: DNNs, RNNs, and SNNs. SNNs use neuron spiking to transmit information with floating point numbers, and information is encoded in the timing and frequency of spikes. This is called event-based processing. The powerful and simple model for a spiking neuron is a leaky integrate and fire model (LIF).
- Neurons that "fire together wire together" and is what leads to synaptic plasticity to accelerate learning. There are multiple models of biological learning: Hebbian learning equation, the STDP equation, and memory engramming.
- There are many implementations of "learning":
	- Unsupervised learning: using unlabeled data to find relationships between elements in the dataset (for example, Hebbian learning)
	- Supervised learning
	- Reinforcement learning
	- Reservoir computing - for time series. Employs dynamic reservoirs with short term memory to project features from inputs into outputs.
	- Deep learning - one-shot and few-shot learning. "Traditionally supervised deep learning has achieved great success when a large labeled dataset is available. However, humans can learn an object category even when only one or few instances are shown. Even at a young age of six, one has learned almost all of the 10 to 30 thousand object categories in the world. This is due not only to the computational power of human brains, but also to the ability to synthesize and learn new object classes from limited information about different, previously learned classes. One-shot and few-shot learning aim to achieve a similar goal."

Conclusion:
- A brain-based paradigm of computing will be massively efficient due to highly parallel streams and hierarchical processing
- The brain can leverage DNNs and SNNs extremely well, and self-learn based on the Hebbian principle, which can be mathematically deconstructed, and is therefore feasible to for compute.
- The brain somehow does "one shot learning" extremely well, and handles unsupervised data extremely well.

# Article 9
[The AI Boom Could Use a Shocking Amount of Electricity | Scientific American](https://www.scientificamerican.com/article/the-ai-boom-could-use-a-shocking-amount-of-electricity/)

Problem:
- "Around the globe, data centers currently account for about 1 to 1.5 percent of global electricity use, according to the International Energy Agency. And the world’s still-exploding boom in artificial intelligence could drive that number up a lot—and fast."
- "A peer-reviewed analysis published in Joule is one of the first to quantify the demand that is quickly materializing. A continuation of the current trends in AI capacity and adoption are set to lead to NVIDIA shipping 1.5 million AI server units per year by 2027. These 1.5 million servers, running at full capacity, would consume at least 85.4 terawatt-hours of electricity annually—more than what many small countries use in a year." This research was conducted by Alex de Vries, a data scientist at the central bank of the Netherlands and a Ph.D. candidate at Vrije University Amsterdam, where he studies the energy costs of emerging technologies.
- "If you were to fully turn Google’s search engine into something like ChatGPT, and everyone used it that way—so you would have nine billion chatbot interactions instead of nine billion regular searches per day—then the energy use of Google would spike. Google would need as much power as Ireland just to run its search engine."
- The energy consumption used by AI goes into training, deployment (inference), and cooling energy usage. Global data centers, on average, will add 50 percent to the energy cost just to keep the machines cool. There are data centers that perform even worse than that.

# Article 10
[The carbon impact of artificial intelligence | Nature Machine Intelligence](https://www.nature.com/articles/s42256-020-0219-9)

Problem:
- The United Nations has called climate change a “defining crisis of our time”, and, according to the Climate Reality Project, 97% of climate scientists concur that human activity is its main driver. The key mitigation pathways to avoiding a global environmental catastrophe include bringing emissions to zero by the middle of the twenty-first century, and limiting the average global warming to 1.5 °C.
- AI is itself a significant emitter of carbon. This message reached the attention of a general audience in the latter half of 2019 when researchers at the University of Massachusetts Amherst analyzed various natural language processing (NLP) training models available online to estimate the energy cost in kilowatts required to train them. Converting this energy consumption in approximate carbon emissions and electricity costs, the authors estimated that the carbon footprint of training a single moderately-sized language model is equal to around 300,000 kg of carbon dioxide emissions. This is of the order of 125 round-trip flights between New York and Beijing.
- OpenAI research lab revealed that the compute used in various large AI training models had been doubling every 3.4 months since 2012.
- The Red AI trend: for a linear gain in performance, an exponentially larger model is required, which can come in the form of increasing the amount of training data or the number of experiments, thus escalating computational costs, and therefore carbon emissions.
- Amazon’s emissions increased by 15% last year. Microsoft is using nuclear energy to power their data centers.
- At Virginia, USA, the data centre hub of the world, only 1% of electricity comes from renewable sources.
- AI is an ‘energy gobbler’ given the complexity and energy consumption that goes behind the Deep Learning models. Researchers estimate that 285,000 kgs of CO2e are emitted from training just one Machine Learning algorithm which is five times the lifetime of a car emission.

Solution:
- This is definitely something that people are working on, be it via more efficient GPUs or by buying renewable energy credits for the carbon that was produced by neural network training. Using renewable energy grids for training neural networks is the single biggest change that can be made. It can make emissions vary by a factor of 40, between a fully renewable grid and a fully coal grid.
- The actionable recommendations from the UMass team are similar — for example, the authors encourage researchers to prioritize computationally efficient hardware and algorithms.

# Article 11
[How Big Will AI Models Get? - IEEE Transmitter](https://transmitter.ieee.org/how-big-will-ai-models-get/)

Intro:
- GPT1 had 117 million parameters.
- GPT3 was trained on nearly 45 terabytes of text data, and has more than 175 billion parameters.
- Current AI models exceed 1.6T parameters - the largest being 174T parameters.
- In NLP alone, the largest models have gone from having 94 million parameters in 2018, to 100 billion parameters in early 2020.

Problem:
- Although solutions include better hardware and software developments, the trend of increasing AI model size does not appear to be ceasing.

# Article 12
[Parameters in notable artificial intelligence systems](https://ourworldindata.org/grapher/artificial-intelligence-parameter-count#reuse-this-work)

Image/graph resource for "Parameters in notable artificial intelligence systems"
- Exponential parameters in notable AI systems
- Number of high parameter AI models developed in the past 3 years
- Linear correlation of model parameters with training complexity