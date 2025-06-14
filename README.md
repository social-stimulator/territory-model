# territory-model
Read Me 

The territory model 

This is a basic model developed for building coding skills in NetLogo
It attempts to model various clans competing for territory. 
Please ignore the code embedded for Graphics. 
Download and run on NetLogo app to see the visual representation of the model 

Rules of the Model 

Level 1 : Basic processes 
Environment has patches, containing the property resources, set randomly from 0-100 
Environment has a custom number of agents 
Agents use resources to produce energy, initial value set randomly from 0-100 
Agents use this energy to move in their environment, looking for patches with the highest values of resources to consume in their immediate vicinity. 
If the energy levels of an agent go below 0, the agent dies. 
In the current version of the model, the resources do not renew. This eventually leads to a situation with net 0 energy in the system. 

Level 2 : Introducing clans 
Each agent has a colour and belongs to a particular clan [one of green, blue, red, yellow 
Clans are groups of agents having the same colour and distributed to the same quadrant of the model. 
Agents of a particular clan can claim a patch by consuming the resources on that patch. Claiming a patch turns it into the color of the clan it was claimed by 
Agents can only consume resources from unclaimed patches, or patches claimed by their own clan. This leads to agents moving through the territory of opposing clans, but does not allow them to access their resources. 

Level 3 : Introducing hostility 
Clans can be turned hostile from a switch placed on the NetLogo interface. This enables the hostile clan to claim resources from other clans under particular conditions. After encountering a patch claimed by a different clan, the agent belonging to the hostile clan scans for the nearest agent of the opposing clan, and compares the energy levels of both the agents. If the hostile agent has more energy than the nearest agent of the opposing clan, the hostile agent takes the patch over and claims it for its own clan. Else, it passes through the patch without claiming any resources.

Features to be added ; 

Renewal rate for resources 

Reproduction in agents [if they reach a certain energy threshold 

Longer range of visibility for agents, enabling strategic movements towards areas with higher resources [ currently limited only to adjoining 8 patches 

Conditional hostility responses, triggered when a neighbouring clan turns hostile 

Comparison of the total energy levels of competing clans to determine the result of an attempt to takeover enemy territory.
