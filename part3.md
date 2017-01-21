# Part 3
## Grasp Planning using GraspIt!

This part gets you familiar with using GraspIt! for 

### (a)
Follow the instruction at the repo:

https://github.com/CURG/graspit_commander



### Demo to TAs
- Show grasp planning in GraspIt! and show the different properties of a planned grasp


gc = graspit_commander.GraspitCommander()
gc.clearWorld()
gc.loadWorld("pr2_mug")		
gc.clearWorld()
gc.loadWorld("plannerMug")
response = gc.planGrasps()
grasps = response.grasps

for idx, grasp in enumerate(grasps):
	gu.show_grasp(grasps,gc,idx)
	x = raw_input("1 for proceed, 0 for skip\n")
	if x != '1':
	continue