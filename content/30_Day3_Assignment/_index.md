---
title: "Day3: Quantum Computing Basics"
chapter: true
weight: 30
---

# Day3 Assignment

Day3 is for learning the basics of quantum computing development in the cloud

### Learning Objcetives
- Get familiar with AWS Products
- Set up development environment for the rest of days 
- Understand the application of TSP problem in real-world through research
- Onboarding to Quantum Computing

### Deliver Result
- 1 PPT Slide: Find at least 5 real scenarios for the application of quantum computing
- 1 PPT Slide: Describe the progress/limitation of quantum computing
- 1 PPT Slide: Describe how to build a model based on quantum gates (anzats,objective function, training) 
- Go through the notebooks in quantum-computing-algorithm/basics/gate and finish the assignment in quantum-computing-algorithm/basics/gate/pennylane/1_Build_Your_Gate.ipynb

---

#### Get Familiar with AWS Products

First, let's have an overview of AWS. Browse through [AWS Official Webpage](https://aws.amazon.com/). 

* [What is Cloud Computing](https://aws.amazon.com/what-is-cloud-computing/?nc1=f_cc)
* [AWS Cloud Products](https://aws.amazon.com/products/) 

In this two weeks, you will use three AWS Products. 

 * [Amazon WorkSpaces](https://aws.amazon.com/workspaces/) is used as a host to run the python project.
 * [Amazon SageMaker](https://aws.amazon.com/sagemaker/) is used for running the given Notebooks, where you learn algorithms step-by-step.
 * [Amazon Braket](https://aws.amazon.com/braket/) is used for accessing quantum computing resources. 


---

### Build your own quantum gate


**Step 1**  : Download workspace client from https://clients.amazonworkspaces.com/.

**Step 2** : Log into Amazon WorkSpaces with the given registration code. (If you don't have the code, ask your mentor.)


{{% notice Note %}}
<p style='text-align: left;'>
The examples and sample code provided in this workshop are intended to be consumed as instructional content. The crendentials is given for camp learning experience, please do not share it with others.
</p>
{{% /notice %}}

**Step 3** : After login, you will see the desktop user interface. Now you are using a Amazon Linux system.

**Step 4** : Open a Terminal window.

**Step 5** : Execute the following commands in the Terminal to checkout project GitHub Repository and start running the project.
```
git clone  https://github.com/guming3d/TSP-workshop-Original.git
cd TSP-workshop
pip3 install -r requirements.txt
python3 source/flask_app.py
```
**Step 6** : Open a web browser in the WorkSpace, visit http://127.0.0.1:5000, you should see a Web UI.

---
### Onboarding to Quantum Computing

We are trying to learn building model in braket. Please watch the following videos for knowledge.

* [Exploring quantum computing today with Amazon Braket (30 minutes)](https://wx.mail.qq.com/ftn/download?func=3&key=9dc79161d02ccd1eafb41a61346530395115d46536653039471702075504070f515d190353035214560e07031b5d050b01150457505d085d070e01040f5164391b4c011218065f544f796332161755192b5642045811100b520a0441731d40550d4a5d0f5145414c035640145b4553560f4841155f0b5719165750004f454750165014205b044a560c187613570e554d4c5544552211a455ad2c2f3112843a1daf01fb1719e34584ee&code=b84a6e09&k=9dc79161d02ccd1eafb41a61346530395115d46536653039471702075504070f515d190353035214560e07031b5d050b01150457505d085d070e01040f5164391b4c011218065f544f796332161755192b5642045811100b520a0441731d40550d4a5d0f5145414c035640145b4553560f4841155f0b5719165750004f454750165014205b044a560c187613570e554d4c5544552211a455ad2c2f3112843a1daf01fb1719e34584ee&fweb=1&cl=1)
* [Pennylane Intrdocution (5 minutes)](https://wx.mail.qq.com/ftn/download?func=3&key=9d9c1631d371c410afef4a3137383937e3d7ae3035383937474c0050505908045a5a4903535b0c1a5650060418015f04014e5007030a0b5553075653560b18371b1751421b5b565a4f34015d5657545242170b11655d57591b2f055f50165447567705c1954028e6fca0aaa6769a3b5047ed45119c9a&code=bcd15897&k=9d9c1631d371c410afef4a3137383937e3d7ae3035383937474c0050505908045a5a4903535b0c1a5650060418015f04014e5007030a0b5553075653560b18371b1751421b5b565a4f34015d5657545242170b11655d57591b2f055f50165447567705c1954028e6fca0aaa6769a3b5047ed45119c9a&fweb=1&cl=1)
* [Pennylane and Amazon Braket (50 minutes)](https://wx.mail.qq.com/ftn/download?func=3&key=cdcd9b33d32cc416ffbe183337653931c1d1dc2335653931171d065605575a05010b1b0a00520d1c0654505218075b03061f520b05510b0750510257005265314b4603401b06565c1f637e52560e190302000713701750521279534046095c43d0b2a27f50044b5f5b5c51136410585f46475b1378045a595b5c534015355c5f5c4b7a525b0019505c5616725804435e5c127441540e5c451c5f460721850b5d79de5d4345586c4d7021590dddd70eb6ce&code=22635e91&k=cdcd9b33d32cc416ffbe183337653931c1d1dc2335653931171d065605575a05010b1b0a00520d1c0654505218075b03061f520b05510b0750510257005265314b4603401b06565c1f637e52560e190302000713701750521279534046095c43d0b2a27f50044b5f5b5c51136410585f46475b1378045a595b5c534015355c5f5c4b7a525b0019505c5616725804435e5c127441540e5c451c5f460721850b5d79de5d4345586c4d7021590dddd70eb6ce&fweb=1&cl=1)

---
### For your reference (optional)
Do you know the latest event about AWS? 

* Checkout the [2021 Re:Invent](https://reinvent.awsevents.com/keynotes/?nc2=h_reik) , an annual event of AWS. 10-year Anniversary! 
* Adam Selipsky's Keynote (~2h)
<a href="http://www.youtube.com/watch?feature=player_embedded&v=WGA2P_oH5Xc
" target="_blank"><img src="http://img.youtube.com/vi/WGA2P_oH5Xc/0.jpg" 
alt="Adam Selipsky's session" width="120" height="90" border="3" /></a>
