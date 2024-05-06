# Cost Estimation

2 formulas we must memorize (20 pts in exam on COCOMO)

* Predicting the resources required for a software development process

4 ways to measure productivity

### Fundamental estimation questions
* How much effort is requried to complete an activtiy?
* How much calendar time isneed to complete an activity
* What is the total cost of an acitvity?
* project estimation and scheduling and interleaved management activities 

Goal when setting project estimation with customer, extend the due date as much as possible
- if it takes 4 months to finish extends to a year and haggle for 6 months

Fiscal vs Physical

Fiscal is realistic: i.e. we actually work 5 hours a day not 8

Calendar time is useless

## Software cost components (IMPORTANT)
4 things
* Hardware and software costs
* Travel and (entertainment) training costs (TTN / T & E)
* Effort costs (the dominate factor in most projects) (MAJOR IMPORTANT ONE)
	* salaries of engineers involved in proj
	* Social and insurance costs
* Effort costs must take overheads into account
	* cost of building, heating, lighting
	* costs of networking and communication
	* cost of shared facilities

### Software pricing factors
- Market opportunity
- cost estimates
- contractual terms
- Requirements volatility
- Financial Health

## Productivity measures (IMPORTANT)
- **Size related**: (line of code) (COCOMO calls it source line of code // not commented code but runtime code)
	- Based on some output from the software process. This may be lines of delievered source code, object code instructions, etc.
- **Function related**: (you look at functions, Inputs and outputs, screens)
	- based on an estimate of the functionality of the delievered software. Function-points are the best known of this type of measure

### Measurement problems
- Estimating the size of the measure
- estimating total number of programmerm onths which have elapsed
- Estimating contractor productivity (e.g. documentation team) and incorporating this estimate in overall estimate

### Functions points
screens (not lines of code)

### Object points
* Number of seperate screens
* number of reports
* number of 3gl modules that must be developed to supplement the 4gl code

## Factors affecting productivity
- Application domain experience
	- Knowledge of the application domain is essential for effective software devlopment. Engineeers who already understand a domain are likely to be most productive 
- Process quality 
	- Dev process used can hava significant effect on productivty
- project size
	- Larger a rpoject the more time required for team communications. less time available for dev. so individual productivity is reduced.
- technology support working environment
	- Good support technolgoy such as CASE tools, supportive config. management systems. (can improve productivity)
- Working enviornment
	- a quiet working evnironement with private workl areas contributes to improved productivity

## Estimation techniques (IMPORTANT)
4 ways we do estimations

what are the 4 estimation tech.
* Algorithmic cost modelling
* expert judgement
* estimation by analogy 
* price to win

### Algorithmic code modelling
uses formula

### Expert judgement
How long does this take to do this or that, oh john knows because he's an expert

advantage: cheap
disadvantage: verry inaccurate if theres no experts

### Estimation by analogy
Comparison to previous project w/ more or less (if a small took us 4 months big will take 6)

advantages: accurate project data to compare
disadvantages: inaccurate if first project

### Pricing to win
- The approach may seem unethical and unbuisnesslike
- however, when detail information is lacking it may be the only appropriate strategy 
- The project cost is agreed based on an outline proposal and dev. constrained by that cost
- Detailed specification may be negotiated or an evolutionary approach used for system development

### Management Options
1. Use existing hardware dev system and team.
2. Processor and memory upgrade
3. Memory upgrade only
4. More experienced staff
5. New devlopment system
6. Staff with hardware experience

### Project duration & Staffing
- time required is independent of the number of peoplel working on the project.
- Hiring is a lot like marrying (its difficult to find people)

## Staffing requirements
- Staff required cant be computed by diving the dev. time by the req. schedule
- The number of people working on a project varies depending on the phase of the proj.
- more people who work != fast development 

# COCOMO

## Highlights
6 important items (7th item optional)

**COCOMO = Constructive Cost model**
Barry Bohiem (BANE) -> invented COCOMO 

1. SLOC (Source Line of Code)
	1. What is definition of SLOC
		1. Only source line of code delievered to customer count 
		2. Source lines created by project staff not a tool
		3. 1 line of code == 1 logical line of code
		4. Declarations are counted
		5. Comments are not counted
2. Scale Drivers (MUST REMEMBER THESE)
	1. 5 scale drivers are (Big picture, MACRO):
		1. Precendentedness
		2. Development Flexibility
		3. Architecture / Risk Resolution
		4. Team Cohesion 
		5. Process Maturity
3. Cost Drivers (Don't have to remember)
	1. 17 cost drivers (MICRO)
4. Effort Equation (MOST IMPORTANT)
	1. Effort = 2.94 * EAF * (KSLOC)^E
		1. Where EAF = effort adjustment factor derived from cost drivers
		2. E is an exponent derived from the five scale factors
		3. KSLOC -> KiloSLOC (x10^-3) (given 8000x10-3 SLOC or 8 Kilo SLOC)
			1. ex. Effort = 2.94 * (1.0) * (8)^1.0997 = 28.9 person months
5. Schedule Equation (MOST MOST IMPORTANT)
	1. Duration = 3.67 * (EFFORT)^SE
		1. Where Effort: is the effort from the COCOMO effort equation
		2. SE is the schedule equation exponent derived from the five scale drivers
			1. ex. Duration = 3.67 * (42.3)^.3179 = 12.1 month's 
6. Average Staffing 
	1. Average staffing = (EFFORT) / (DURRATION) 
		1. ex. Average Staffing = (42.3 Person months) / (12.1 months) = 3.5 people 

What does cocomo stand for?
what are the 6 parts of cocomo?

