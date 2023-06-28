Your firm is interested in answering 3 main questions:  
• Is the drug effective in decreasing the systolic blood pressure?  
![[Pasted image 20230320113159.png]]
Initial looks:
- Medication, directly lowers blood pressure
- Pain medication, directly increases blood pressure

![[Pasted image 20230320113445.png]]
- P-value = 0, means we reject the null hypothesis
	- Reject that there is no difference, meaning  that  the drug has an effect / makes a difference on the blood pressure

- More information about the direct effect could be acquired through regression analysis



• Is the effectiveness of the drug affected by a pain medication that is  
commonly prescribed to elderly?  
![[Pasted image 20230320113917.png]]
- The drug lowers blood pressure
- Pain medication may increase the blood pressure, but due to the high p-value we cannot reject the null hypothesis that is has an effect
- Combination of pain medication and drug has an effect (decreases the effect of the drug by 7) (as it increases the blood pressure by 7)


• Is the effectiveness of drug dependent on the gender of the participant?  



- For women, the effect of the drug is more effective, as the interaction effect is -5.42 on top of the effect of the drug and the effect on blood pressure of being female


##### How would you design the experiment to be able to answer the above  questions?
- Population is elderly --> ensure sample is somewhat representative (only recruit e.g. people over 65)
- Lab experiment
	- Testing drugs would benefit from a controlled environment where it's easier to account for extraneous variables
	- Easier to measure/observe the variables and their effect
- Between-subject Experiment
	- Treatment group which receives the drug vs. control group that receives a placebo
	- Randomization to reduce bias (in terms of the participants in which group)
		- If the pain medication is given this should also be random between the groups
- Full-factorial design
Treatment Condition | Drug | Medicine | Gender
-----------------------|----|------|-------
1 | No | No | Male
2| No | No | Female
3 | No | Yes | Male
4 | No | Yes | Female
5 | Yes | No | Male
6| Yes | No | Female
7| Yes | Yes | Male
8 | Yes | Yes | Female






