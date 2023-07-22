# Assignment 2: Protests
In recent years the United States has experienced a surge of protests, in support of Black Lives Matter, gender equity, and many other social or political issues.

In this assignment, you will work with data from [Count Love](https://countlove.org/), data that is ocassionally [cited](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html) by the _New York Times_ when reporting on US demonstrations.

Through this assignment, you will be able to answer questions about protests, including:

* What were the most attended and least attended protests in the US in the last 5 years?
* How many protests occurred in Washington state?
* How did the number of protests in 2019 compare to 2020, and why?
* Why are people protesting in the US? What are the biggest motivators?

## Learning objectives
By completing the assignment, you will develop or skills for:

- **Version control** tools for managing code (git and GitHub)
- Writing documents with **markdown** syntax
- Coding in R
- Thinking critcally about data.

# 1. Critical Analysis & Reflection: Before You Code

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — that is, knowledge about the topic of the dataset. Sometimes the topic is very narrow; more often it is expansive, as in the case of CountLove. We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it. To get more familiar, we are going to begin by doing some background reading.

**Note:** Please write your answers below under the heading "Your Responses and Reflections."

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm).  **(R1a)** Based on the information in these pieces, why did the creators start collecting the CountLove data?

- Next, we would like you to read this [New York Times piece that uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) and that describes the Black Lives Matter protests that occurred in the summer of 2020. **(R1b)** Please summarize the main point or argument of this article.

Next, we're going to reflect about who collected this data, and what's actually inside it.

**(R1c)** Who collected and shared the CountLove data, and what do they do for a living?

**(R1d)** As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude?

**(R1e)** How and where does CountLove get their data about the protests?

**(R1f)** How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation?

**(R1g)** What are two central values of Count Love? Name and briefly describe them. (See the Envisioning Cards for a definition of "value".)

**(R1h)** Name and briefly describe one direct stakeholder and one indirect stakeholder (See the Envisioning Cards)?

# 2. Coding in R: Parts 1-6
**Instructions**. Assignment instructions and prompts are in this file: [analysis.R](analysis.R).

**Coding and reflection prompts**. You will find two kinds of prompts in [analysis.R](analysis.R):

* *Coding prompts*, which prompt you to write R code in [analysis.R](analysis.R).
* *Reflection prompts*, which prompt you to think and write in English below, in this file (README.md).

**Formatting Your Responses and Reflections**.

* When formatting your written responses and reflections below, please *retain* all
reflection prompt IDs (e.g., R1a, R2a, etc.).
* Fill in the elipses (...) with your own words.
* Remove expected word counts.
* To write clearly, use markdown code appropriately (e.g., **bold**, _italics_, and `code`). As appropriate, include images, links, and so forth.

**Questions?** As always, please post on Teams or ask your Instructor or Teaching Assistant.

:computer: Good coding!
   :writing_hand: Good critical thinking!
      :smile: Good-luck!

(_Updated: October 2022, Your Teaching Team_)

# 3. Critical Analysis & Reflection: After You Code

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

**(R1h)** How does the CountLove project embody one or more of these 4 forms of challenging power?

**(R1i)** What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)

**(R1j)** What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)

## Your Responses and Reflections

### Critical Analysis & Reflection: Before You Code (questions above)

* **(R1a)** The creators collect the CountLove data from local newspapers and television sites to build up long-term protections for the social issues across the United States, including civil rights, immigration, racial injustice, etc.
* **(R1b)** The main argument of the article shares the protest against racial injustice, especially in avoiding violence toward African-Americans. Black Lives Matter movement has been widespread in every single state of the US. Hundreds of thousands of people move onto the street, step across traditional fault boundaries, and beat down stereotypes to let the world have an in-depth awareness of the daily hardships faced by African-Americans.
* **(R1c)** Tommy Leung and Nathan Perkins, scientists and engineers with great interest in cvil responsibility and public policy, collected and shared the CountLove data. They were doing this for creating a reliable source of the ongoing protests and demonstrations in order to build a comfortable and supportive environment.
* **(R1d)** CountLove counts the demonstrations of protests that are not included in "regular business." It excludes awareness events, commemorative celebrations, historic reenactments, fundraising events, or political campaign rallies.
* **(R1e)** CountLove gets most of their data from crawling and citing primary sources. Daily local newspaper, television sites, or printed documents are used to record different protests.  
* **(R1f)** CountLove uses the most conservative estimation to record the number of attendance of a protest, where it interprets "a dozen" as 10, "hundreds" as 100, "thousands" as 1000; and so on. Due to the margin of error, CountLove cannot provide a precise number of attendance; therefore, some rigorous research studies might not use the estimated data for formal statistics because of the possible underestimated attendance.
* **(R1g)**
  * One of the central values of CountLove could be justice. The principle of CountLove establishment appeals to the world, understanding different protests in the long-term geographic and temporal trends. By communicating with the elected leaders, CountLove emphasizes the key point of justice, helping people to be aware of different social issues and find out the best solution as soon as possible.  
  * The other central value can be considered as system reliability, where the creators are attributed to useful sources to help the journalists and concerned citizens. The widespread dataset of protests can help the communities to build a diverse and empathetic country.
* **(R1h)**
  * Direct stakeholders for CountLove can be considered as journalists, who use these data as references and edit relevant productions on either paper works or websites on social media.
  * Indirect stakeholder for CuntLove are the neighbors who live in the protest area. They does not actually use the data of protests but still affect by the environment they stayed in. For example, neighbors can be impacted on the surrounding discussion of the protests or the heavy traffic it caused.

### Part 3: Locations (`analysis.R`)
* **(R3a)** There are 1375 protests that occurred in Washington State, and that number really surprise me a lot. Being a sophomore student in the University of Washington, I rarely see or hear about different protests, maybe only around 1 or 2 times per year. At the same time, I gradually recognize the liberty of the state, which strongly advocates the widespread of political and social activities.
* **(R3b)** I am surprise about using a single function once to apply on each element of the vector in the dataset. It actually wakes my curiosity to learn more different types of functions in summarizing and interpreting the data.
* **(R3c)** I notice that there are some misinterpreting spelling of the name of the states, recognizing the capital letter, in this case, such as wA and WA, co and CO, etc. The better way to solve this quality issue is to go through the entire dataset to figure out whether they are considered the same state or not. If they are the same, I would like to combine and group them together for better clarification.

### Critical Analysis & Reflection: After You Code (questions above)
* **(R7h)** CountLove embodies both achievements of collecting and analyzing. Generating the protest data from reports in print or video, a set of tools has been used for crawling, extracting information; and categorizing articles. Along with the process of machine techniques, the data, which used to separate to everywhere else, are now grouped and organized into date, location, number of attendees, and the summarized title for the events. CountLove also provides a reliable platform to record the social issues at the back of each protest, such as healthcare, civil rights, immigration, and so on. It offers spaces for people with different career backgrounds (politics, military, media, education) to pay attention and take action.
* **(R7i)** The most surprising thing I learned from this analysis is how different functions extract specific needs from the giant dataset. Therefore, I am more curious and looking forward to applying the data analysis skills I learned to many different data types. Besides, I am always excited to learn the upcoming knowledge, exploring and solving the mysteries in the information age.
* **(R7j)** I am very interested in articles and sources that provide on CountLove data for giving readers a better understanding of different protests. I would like to go through two or three articles on each topic if I have time. And, I believe that reading can me an in-depth insight into the background information and brainstorming each protest at that time. By comparing the articles from different topics of events, I can also recognize what type of writing is favored to be selected and extracted by CountLove.
