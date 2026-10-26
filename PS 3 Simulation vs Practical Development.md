
I  would choose a hybrid approach - combining simulation led design and rapid physical prototyping. Obviously , simulation will have to come first and then the physical design. 

## Advantages and Limitations of Each 
- Simulation Led : 
	- Advantages : Expense is drastically lowered, allowing rapid comparison and strict mathematical precision. It will help identify many problems before the manufacturing process even begins. 
	- Disadvantage : Real world effects may be missed depending on the skill of the designer (ex : ansys mein number of nodes optimize karna). Incorrect assumptions may burn the entire project down. Complex simulations may need significant resources and may drop precision (ex : xfoil mein converge hi nhi ho rha).
	- Ex : XFLR5 for airfoil analysis, ANSYS for detailed structural and fluid flow studies. 
- Practical led : 
	- Advantage : Several times an over engineered model, coming from the simulation faces many manufacturing challenges. Hardware - motor , esc compatibility can be verified.
	- Disadvantage : Repeatedly building and dismantling requires high material cost and consumes lot of time. 

## Comparison 
-  Cost : Simulation led will be more cost effective. 
- Time : Simulation led again. 
- Accuracy : For simulations it will depend on the mathematical models , assumptions and data. Physical build will measure the actual behavior under tested conditions. 
- Changes : Simulation led can be changed in a few clicks. 
- Final performance : Simulation led will help optimize the theoretical design and physical build will confirm the performance. 

## Parameters to check 
- From simulation we can check the lift and drag characteristics, as I have done from XFOIL. We can also study the structural strength and deformation. We can also check the pitching moment , static stability of different configurations. 
- From physical model we can check the actual mass and cog , verify the servo optimization , structural stiffness and flight performance. 

## Simulation is Good but Physically its Bad 
- Actual mass may be greater than the simulated value , messing up the lift and drag calculations. 
- The installed propulsion is delivering lesser thrust than predicted. 
- Incorrect airfoil or wing geometry , misalignment , are physical parameters which may have manufacturing defect. 
- Voltage sag , excessive current flow, power system fault and shielding issues might have occurred. 
- Assumptions of air density , propeller dynamics might have been wrong. 
- Diagnostic Plan : 
	- Verify the aircraft total mass and CG. 
	- Check the alignment of wings , wing dimensions and propulsion system. 
	- Confirm Motor ,  ESC , battery all match the specifications. 
	- Verify the wheel alignment , elevator direction , control mechanics are good enough. 
	- Lastly , just look at its performance and change one variable at a time. 


## Tools 
- XFLR5 -- for airfoil , wing and preliminary analysis. 
- ANSYS -- for structural and fluid flow analysis 
- SolidWorks -- CAD. 

## Validate Simulations Using Measurements
- First , we must record the simulated values for mass , stall speed , thrust , current consumption and other relevant parameters, then we match the test conditions by making the air density , battery state , test speed and configuration as comparable as possible. 
- Then we can check the % error and investigate the discrepancies. 
- If the measured thrust is lower than expected then we should inspect the motor operating point , ESC performance before changing the entire aerodynamic design. 


## Workflow 
- First , we define the requirements , constraints of the problem statement. 
- Then we must estimate the aircraft mass , wing loading , lift , stall speed , L/D , power req. , battery capacity , CG range. 
- Then open up XFLR5 , SolidWorks and evaluate structural loads using ANSYS. 
- Select the design that satisfies the performance requirements by comparing wing area , aspect ratio , airfoil , tail configuration and propulsion setup. 
- Manufacture it , lets goooo. 
- Recheck the actual mass , structure , cg . 
- Check the motor and propeller operation , current consumption , bettery under load. 
- Test it out in suitable weather conditions and flying area .
- Identify performance gaps and change one variable at a time 
- Repeat from step 3 , if required. 

