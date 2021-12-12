---
title: "Day1: Warm Up"
chapter: true
weight: 10
---

# Day1 Assignment

Day1 is for ramping up. No hurry. 

### Learning Objcetives
- Get familiar with AWS Products
- Set up development environment for the rest days 
- Reseach on the different applications of TSP problem in real-world
- Onboarding to Quantum Computing

### Deliver Result
- 1 PPT Slide: Find at least 5 real scenarios for the applications of TSP 
- 1 PPT Slide: Find at least 2 technologies for implementing quantum computing
- Demo: Successfully setup environment and launch the project UI in browser

---
#### Get Familiar with AWS Products

First, let's have an overview of AWS. Browse through [AWS Official Webpage](https://aws.amazon.com/). 

* [What is Cloud Computing](https://aws.amazon.com/what-is-cloud-computing/?nc1=f_cc)
* [AWS Cloud Products](https://aws.amazon.com/products/) 

In this two weeks, you will use three AWS Products. 

 * [Amazon WorkSpaces](https://aws.amazon.com/workspaces/) is used as a host to run the python project.
 * [Amazon SageMaker](https://aws.amazon.com/sagemaker/) is used for running the given Notebooks, where you learn algorithms step-by-step.
 * [Amazon Braket](https://aws.amazon.com/braket/) is used for accessing quantum computing resources. 



### Setup Development Environment

**Step 1**  : Download workspace client from https://clients.amazonworkspaces.com/.

**Step 2** : Log into Amazon WorkSpaces with the given registration code. (If you don't have the code, ask your mentor.)

**Step 3** : After login, you will see the desktop user interface. Now you are using a Amazon Linux system.

**Step 4** : Open a Terminal window.

**Step 5** : Execute the following commands in the Terminal to checkout project GitHub Repository and start running the project.
```
git clone  https://github.com/guming3d/TSP-workshop-Original.git
cd TSP-workshop-Original
pip3 install -r requirements.txt
python3 source/flask_app.py
```
**Step 6** : Open a web browser in the WorkSpace, visit http://127.0.0.1:5000, you should see a Web UI.

![Web UI](/k12.interncamp.assignment.book/images/tsp_web_ui.png)
---
### Research about TSP Applications

### What Is the Traveling Salesman Problem?

The traveling salesman problem (TSP) is a problem that asks, with a list of stops and the distances between each of them, what is the shortest path/possible route that visits each location and returns to the origin?

![Traveling Salesman Problem](/k12.interncamp.assignment.book/images/tsp_problem.png)

For decades the TSP has been a challenge for many businesses that rely on route planning.

With just a starting point and a few stops, planning a route can seem complicated enough.

But once you start planning routes throughout the country, it reaches an almost unthinkable level of complexity.

This is what a route would look like if planned to every city in the US with over 500 inhabitants:

![Large Traveling Salesman Problem](/k12.interncamp.assignment.book/images/large_tsp_problem.png)

Just imagine the number of possible routes you could take when a single possible solution is this complex.

#### Why the Traveling Salesman Problem Is Still Hard to Solve in 2022

Mathematician Karl Menger discovered the TSP in 1930, over 90 years ago.

Since then, there have been many suggested solutions and algorithms. But they often struggle with the sheer scale, since the number of possible sales routes increases exponentially with each new stop.

And the truth is, real route planning in 2021 for real businesses is more complex than just a list of stops — making things even more complicated.

In the real world, it’s not as easy as simply finding the shortest route.

#### It’s not just about destinations and distance, there are many other factors in play

It’s not as easy as just taking a list of addresses and creating a route. 

A field sales rep, delivery driver, or technician also has to consider a lot of other factors, like time windows, vehicle capacities, and more.

#### Delivery time windows and planned sales meetings

What if your delivery drivers or salesperson have planned delivery times or sales meetings? Then it’s not enough to just consider the distance, you also have to factor in when they should be at each location.

This adds a whole new level of complexity, and is a challenge that most route planners simply can’t handle.

This particular instance of the problem is also known as the Vehicle Routing Problem with Time Windows (VRPTW). 

#### Required vehicle capacities or technician qualifications

For deliveries, each package that you plan for can have specific requirements in terms of shipping and handling, from refrigeration to unloading dimensions.

You also have to consider the overall loading capacity of each vehicle.

But even for maintenance and field service businesses, you have to consider the unique qualifications of each technician, and whether they match a job.

This is also known as the Capacitated Vehicle Routing Problem (CVRP).

#### Planning efficient routes that include both pickups and deliveries

If your business delivers any sort of reusable packaging or recyclable materials to your customers, chances are that reverse logistics are a huge priority.

To maximize the efficiency of your business, you want to integrate both pickup and delivery into all planned routes.

This adds another dimension and a level of complexity that most route optimization tools can’t handle.

This is also referred to as the Pick-up and Delivery Vehicle Routing Problem (PDVRP)

#### Considering priority of leads, existing clients, and deliveries

To run a business efficiently and keep VIP customers satisfied, you also need to make sure your staff prioritize things the right way.

If your routes don’t consider priority, every customer will be treated the same. So you risk alienating loyal customers if you suddenly switch to an automated solution that can’t handle that.

#### Balancing workloads between multiple drivers

Of course, when planning routes for multiple drivers, you also have to consider their workloads.

Drivers are only human, and have a maximum shift length of 14 hours and mandatory breaks.

What good is an “efficient route” if it’s not possible for a driver to handle it within the allotted time?

Good workload balancing tools will help you reduce overtime and cut driver costs, and make sure all drivers are HOS-compliant at all times.

#### Playing with the code for the simplified TSP problem

**Step 1**  : After logging into your AWS console and click the link for [Amazon Braket](https://console.aws.amazon.com/braket/home?region=us-east-1#/)

**Step 2**  : Next, click the button to [Create Notebook](https://console.aws.amazon.com/braket/home?region=us-east-1#/create-notebook-instance)

**Step 3**  : Let us create a notebook instance and fill the name with ` k12-interncamp-tsp-quantum`

![Notebook with name](/k12.interncamp.assignment.book/images/notebook_name.png)

**Step 4** Select Instance type. Braket notebook provides multiple instance types of different computational power and prices. The default setting is enough for most of our chapters.

**Step 5** Choose create the role for this notebook since this is the first time you use this service

![Create role](/k12.interncamp.assignment.book/images/create_role.png)

**Step 6** Checkout the given GitHub Repo. A Jupyter notebook version of this book for fitting SageMaker is available at ` https://github.com/AoyuQC/k12-interncamp-tsp-quantum.git `. We can specify this GitHub repository URL to let Braket notebook clone this repository during instance creation. After that, Please click the button to crete the notebook.

![Repo link](/k12.interncamp.assignment.book/images/repo_link.png)

**Step 7** It may take a few minutes before the instance is ready. When it is ready, you can click on the “Open Jupyter” link.

![notebook ready](/k12.interncamp.assignment.book/images/notebook_ready.png)

**Step 8** Open the notebook and go to the k12-interncamp-tsp-quantum/application/tsp/Introduction_to_TSP.ipynb to learn something about TSP

![introduction to tsp](/k12.interncamp.assignment.book/images/tsp_intro.png)

**Step 9** After finishing your work, do not forget to stop the instance to avoid extra cost.

After all this practice, let's do some background research. Find at least 5 real-world problem related to TSP. You should be able to describe the use cases. 

---
### Onboarding to Quantum Computing

We will try to solve TSP problem with quantum computing(QC) resource in the second week. Today, we hope you get a basic concept of QC. Please watch the videos belows:


* Quantum Computers Explained in a Way Anyone Can Understand (15 minutes) [download link ](https://wx.mail.qq.com/ftn/download?func=3&key=9ec8af62d52fcb1eacbb19623166363966c15e6033663639441800000453550a56561a5207070314550003071e045700001a0250555f06015406025557567139184302111d0559544c6642035d1243544174580f4313425c134417274b165a5808595206130f5819001760034a4677571858590713255757416259065614454d0059534c5e16022d690e7a7e7c1d40579603900a246b954a1a1854c0&code=a77b3f69&k=9ec8af62d52fcb1eacbb19623166363966c15e6033663639441800000453550a56561a5207070314550003071e045700001a0250555f06015406025557567139184302111d0559544c6642035d1243544174580f4313425c134417274b165a5808595206130f5819001760034a4677571858590713255757416259065614454d0059534c5e16022d690e7a7e7c1d40579603900a246b954a1a1854c0&fweb=1&cl=1) 
<a href="http://www.youtube.com/watch?feature=player_embedded&v=zhQItO6_WoI
" target="_blank"><img src="http://img.youtube.com/vi/zhQItO6_WoI/0.jpg" 
alt="QC introduction" width="120" height="90" border="3" /></a>

* Is Now the Right Time for QC? (30 minutes) [download link](https://wx.mail.qq.com/ftn/download?func=3&key=c9c7c638877ac415fbb44b386333393259f5a03e613339321317045e54025a05055e4809560a5a1f020b5c0f4c515a535715065b59005c07530c575b07576b324f4c504b4f50565f1b79326b41415c127f56135d0f471900060a55182840195c594f454c095619405f5f0d4c4147505f53181157415641425a57175d41424c53584c10554150565f464d11510f54175f460c71b7999b4b5d9785244f1ec228cdf87fd5dd9bc92c&code=68e8a392&k=c9c7c638877ac415fbb44b386333393259f5a03e613339321317045e54025a05055e4809560a5a1f020b5c0f4c515a535715065b59005c07530c575b07576b324f4c504b4f50565f1b79326b41415c127f56135d0f471900060a55182840195c594f454c095619405f5f0d4c4147505f53181157415641425a57175d41424c53584c10554150565f464d11510f54175f460c71b7999b4b5d9785244f1ec228cdf87fd5dd9bc92c&fweb=1&cl=1)
<a href="http://www.youtube.com/watch?feature=player_embedded&v=_ltGOs7aN3U
" target="_blank"><img src="http://img.youtube.com/vi/_ltGOs7aN3U/0.jpg" 
alt="QC introduction" width="120" height="90" border="3" /></a>

* When will quantum computers become reality? (1.1 hours) [download link](https://wx.mail.qq.com/ftn/download?func=3&key=9b9aea65d7289f1ea9e94c6533616239d560766c31616239414a57035552015a00004f0400035b14500154551c59510e534804070554075c07500653575055391d1157161f020d5449320a005f4115500809421444000c4d110842065e0c124c100010161103075a0b080745430403550d111b4b5c11562d80e5c9f88705d50fd13b6fcf0865698125e07051&code=debe1ab9&k=9b9aea65d7289f1ea9e94c6533616239d560766c31616239414a57035552015a00004f0400035b14500154551c59510e534804070554075c07500653575055391d1157161f020d5449320a005f4115500809421444000c4d110842065e0c124c100010161103075a0b080745430403550d111b4b5c11562d80e5c9f88705d50fd13b6fcf0865698125e07051&fweb=1&cl=1)
<a href="http://www.youtube.com/watch?feature=player_embedded&v=3YasK0s9c18
" target="_blank"><img src="http://img.youtube.com/vi/3YasK0s9c18/0.jpg" 
alt="QC introduction" width="120" height="90" border="3" /></a>

---
### For your reference (optional)
Do you know the latest event about AWS? 

* Checkout the [2021 Re:Invent](https://reinvent.awsevents.com/keynotes/?nc2=h_reik) , an annual event of AWS. 10-year Anniversary! 
* Adam Selipsky's Keynote (~2h)
<a href="http://www.youtube.com/watch?feature=player_embedded&v=WGA2P_oH5Xc
" target="_blank"><img src="http://img.youtube.com/vi/WGA2P_oH5Xc/0.jpg" 
alt="Adam Selipsky's session" width="120" height="90" border="3" /></a>
