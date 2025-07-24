---
title: Five questions on the backburner
author: JOL
date: '2025-07-24'
lastmod: '2025-07-24'
categories:
  - topics
  - backburner
tags:
  - proposition
  - storage
  - scaling
  - minerals
  - energysheds
---

When you spend two and a half years trying to crossbreed engineering with policy in energy systems, you necessarily find yourself asking a lot of questions. These are some of the questions that have stuck with me over time, and that a quick google didn't resolve. I'm working on some of them, or on posing them to more people. Collective intelligence!

1. How can we move from an environmentalism that opposes to one that proposes?
2. What are the scaling laws of power systems?
3. How will energy storage be distributed between garages, industrial yards, neighborhoods, substations, and generators?
4. What will be the temporal and spatial extent of the world's energysheds?
5. How much matter are we processing to make today's (energy) tech, and at what point are urban deposits better than natural ones?


## 1. Towards an environmentalism that proposes
Environmentalism of preservation has slowed fossil fuel growth and environmental damage. Taken to the extreme, it can backfire and prevent {{< sidenote "generally good" >}}Context matters: sometimes preservation does avoid damage from "good" things. I'm not saying you should pour concrete for wind turbines over every frog-rich wetland, or [blow up 46,000-year-old rock shelters](https://antar.org.au/issues/cultural-heritage/the-destruction-of-juukan-gorge/) in the name of more iron ore mining. But you *should* be able to build multi-story housing in semi-detached neighborhoods in a housing crisis, or [build transmission lines](https://www-tagesschau-de.translate.goog/wirtschaft/energie/stromtrassen-genehmigungen-bundesnetzagentur-stromautobahnen-100.html?_x_tr_sl=fr&_x_tr_tl=en&_x_tr_hl=en-US&_x_tr_pto=wapp) to bring wind power across your country and reduce gas dependence...{{< /sidenote >}} things from getting built, too. This could be [housing in California](https://www.nytimes.com/2025/06/30/us/california-environment-newsom-ceqa.html) or battery plants on an old contaminated munitions site.

We need an environmentalism that {{< sidenote "builds." >}}I stole this phrase from [this](https://www.economist.com/leaders/2023/04/05/the-case-for-an-environmentalism-that-builds) 2023 article in The Economist, even though they've gone soft on economic inequality and *why* people sometimes oppose projects. {{< /sidenote >}}  We don't solve climate change by winding down fossil fuel usage *unless we build what will replace it*. To me, the crux is that we have enshrined rights to opposition in the name of preservation. What is needed now is the counterbalancing duty to propose, because every opposition increases the burden on others. 

If you *refuse* wind in your backyard, other people will have to see it, and more of it too. Because you're not likely going to consume less power, but it must come from *somewhere*. If you block a train track, are you sure the car traffic that remains because there's no train doesn't impose a greater burden on all the communities through which those cars drive{{< sidenote "?">}}[This](https://www.motherjones.com/environment/2023/04/yimby-nimby-progressives-clean-energy-infrastructure-housing-development-wind-solar-bill-mckibben/) article in Mother Jones by Bill McKibben expands on the argument for "YIMBYism" and the consequences purity has.{{< /sidenote >}}

A duty to propose is sleek, but proposition is costly and difficult. Most groups with rights to opposition do not have the resources for proposition. Can a village of 1,000 souls compete with a billion-dollar corporate project team? What I'm thinking about now is how we can maintain the rights we've fought for while empowering those approached by proponents to say "not quite, but instead, we could...". I think that kind of community-scale self-determination is important if we're to build the infrastructure and machines that prosperity within planetary boundaries requires.

## 2. Scaling laws of power systems
Geoffrey West's work on [scaling laws in living systems](https://santafe.edu/news-center/news/geoffrey-wests-long-anticipated-book-scale-emerges) inspires me to wonder about how power systems scale. More concretely, what kinds of nonlinear relationships can we surmise from the top down about the behavior of important metrics as we change the size of components, or the size of the overall system?

For an example of the "scale" that might impact power systems, consider residential energy demand as a function of population. If you assume each person lives in the same kind of dwelling, then it's linear. If you assume there's a mix of dwellings, then to estimate the answer from the bottom-up, you have to know the types of dwellings people live in, how well they're insulated, how many walls are exposed to ambient air, how big those walls are, and so on... This might be fine as a backwards-looking measurement, but this gets increasingly tricky if your job is to forecast future residential energy demand as a function of demographic projections. Are linear correlations enough? Can we use urbanization patterns from elsewhere to predict what kinds of dwellings people will move into, and to what extent there will be rebound effects from lower home electricity bills? Can this complex relationship between population and energy consumption be captured by a computationally "cheap" power law instead of multiple interacting sub-models?

For another example, consider [how grids fail](https://wiki.santafe.edu/images/e/e6/Blumsack_SFI_CSSS_2019.pdf) as Seth Blumsack summarizes it. One piece of equipment breaks down, line loads increase somewhere in the network, something melts down or switches off automatically, and then we spend a lot of time doing root cause analysis because propagation in electrical networks is ill-understood. In this area, blackout frequency and numbers of customers impacted has been shown to follow a [power law](https://doi.org/10.1109/TCSI.2004.834513). How might this change as we add stochastic generators (wind and solar), storage devices, and increase the number of attack vectors for bad actors? If it follows a power law, can we better understand the types of risks we're opening ourselves up to *without* having to model every second of the year while we perform {{< sidenote "capacity expansion?">}} I bring up capacity expansion models because they are used to find least-cost pathways to a decarbonized energy system. Unfortunately, that makes them very computationally expensive even if you only represent a few hundred hours in the year--forget getting to resolutions where you can model accurate AC and DC power flow transients!{{< /sidenote >}}

Empirical, predictive top-down power laws might be of use as we try to decide what to build. They could help us assess tradeoffs in power system architecture with less compute. When utilities say "can't be done" to deep renewables integration yet the (academic) policy wonks yell on rooftops that it's the cheapest way, clearly there's a need to be met.

## 3. Energy storage's many forms
In garages, it's EVs or small wall-mounted battery packs. Maybe even hot water tanks.

In industrial yards, it might be fleets of EV buses or vans, or the batteries needed to deal with the surge in power demand those generate when they plug in. 
 
In neighborhoods, citizens might come together to own a community battery that sits on a concrete pad, curbside. It'll soak up solar from homes and dispatch back below the substation.

In substations, utilities might install one on the low-voltage side to deal with new loads and thus defer transformer upgrades. They might also tack them onto transmission lines to increase uptime. 

In power plants, storage might be paired with wind or solar so it can deliver power at times of high prices. 

Behind the industrial fence, storage might shave peaks in {{< sidenote "demand">}}Some industries might even store heat to substitute natural gas in their processes. They might not be able to use this heat storage to feed back into the grid, but controllable demand reduction at times of high prices is itself a form of "generation" from an economic standpoint.{{< /sidenote >}} and act as a peaker if the expansive rooftops of warehouses and factories are used for solar generation that fills up the batteries.

How much of each form will lead to a least-cost, greatest-benefit energy system? And, importantly, the greatest benefit for whom? For the shareholders of regulated-return utilities, or for households lucky enough to own their home? How can we bring in everyone?

Are we better off leveraging the economies of scale of EV battery cell manufacturing, or those from centralizing power infrastructure? Is the cost of the wires to bring stored power to consumers too high relative to centralization savings? What about the costs of coordinating all of this via price signals and all the {{< sidenote "algorithmic overhead" >}}Can we even keep those markets "honest"? Declan Kelly of Currently Speaking raises the question of [market concentration via algorithmic ubiquity](https://currentlyspeaking.substack.com/p/hot-chips-algorithms-and-electricity): if everyone trades using the same heuristics, do we get into upward price spirals and price fixing like in U.S. potato markets? Electrons aren't potatoes, but this question makes sense, trust me!{{< /sidenote >}} involved? Can we make it easy and just for everyone, not just technology nerds who like to turn their appliances into gadgets?

## 4. The temporal and spatial extent of the world's energysheds
A watershed means the area where water inflows drain to a common body of water. An {{< sidenote "energyshed,">}}See [John Evarts' thesis on the topic](https://dalspace.library.dal.ca/bitstream/handle/10222/71377/Evarts-John-MES-SRES-April-2016.pdf) if you want the formal definition and sophisticated discussion of the concept.{{< /sidenote >}} by analogy, is the area where energy production (the inflow) is balanced with energy consumption (the common drain).

Today, the vast majority of energy, in the form of fossil fuels, is produced in relatively few countries. So, today, few places are autarkic in energy terms. We might in fact be a single big energyshed. Tomorrow, the ubiquity of sunshine and wind might mean more places can self-supply. Will they? How much? What's the trade-off? How "porous" will those boundaries be between energysheds? How much do those answers depend on the availability of energy storage technologies, which transform present self-supply into future self-supply?

The answer depends on national security concerns, {{< sidenote "equality concerns," >}}Imagine every northern European coastline being lined with wind turbines, while every southern European field is covered in solar panels, while the middle is criss-crossed by dense transmission lines. Cost-optimal, yes, but uneven distribution of the "burdens", so to speak. {{< /sidenote >}} and practical ones. It might be "best" to build transmission lines to connect continents, but if it takes too long and people want control over their energy supply, separate energysheds might prevail. This kind of question is studied by folks like [Evelina Trutnevyte and Jean-Philipp Sasse](https://doi.org/10.1016/j.apenergy.2019.113724), or [Fabian Neumann and Tom Brown](https://www.sciencedirect.com/science/article/pii/S2589004223007794?via%3Dihub#fig7), using models which allow "near-optimality". Are we willing to pay the prices of energetic insulation? Do people realize they are material? This is, in a way, related to local opposition to broadly beneficial projects in #1.

## 5. Matter streams, tech minerals and urban mines
We need minerals to build the machines that will collect the sun and the wind, and store it for later. We know this. People like to throw up graphics of the mass of oil and gas combustion products compared to the mass of minerals required to build an electric future. Those miss the point of all the ore that gets processed to refine those minerals, as well as all the earth that's moved to extract the oil and the coal and the gas in the first place.

Which is bigger? Does it matter? From a climate change standpoint, [harmonized life cycle assessments](https://www.nrel.gov/analysis/life-cycle-assessment.html) suggest solar and wind are a slam-dunk compared to gas, coal, and diesel. But, as we know, there are other ways to harm the environment: acidification, eutrophication, water and soil contamination, biodiversity loss, and so on. What does the picture look like if we consider those?

The optimist in me believes arguments that recycling and material re-use will reduce the size of this problem from virgin material extraction. Recycling also moves us away from an extractive mineral industry that is mired in human rights violations that occur far away from the electric opulence an economically motivated transition promises. Recycling could mean we repeat this exploitative pattern closer to home--but then it's up to us to not be hypocrites in our own backyard.

Practically, this might even mean digging for minerals in landfills one day. When might that day come? How do landfills compare with virgin ores in terms of (recoverable) mineral grades? What can we do when designing products to make recovery from mixed waste easier? Is there a tradeoff between performance and recyclability that we can optimize for? Does the energy intensity of material production increase with recycling? What happens to the life cycle impact(s) if it does? Again, does it matter when compared to the fossil alternatives we have?

## An invitation
I've outlined five big areas where I feel both uncertain and intrigued. Some are more applied than others. I'm sure the questions have at least partial answers today. If you have an inkling of what they might be, or want to tell me what I've forgotten to consider, shoot me an email at julien.otis-laperriere@mail.mcgill.ca.