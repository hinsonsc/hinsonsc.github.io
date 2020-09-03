#Homework 3: Chapter's 11 and 12

	11.4 What is the common characteristic of all architectural styles that are geared to supporting software fault tolerance?
		These systems usually have redundancy, meaning they have extra hardware and software built into their architecture.
	11.7 It has been suggested that the control software for a radiation therapy machine, used to treat patients with cancer, should be implemented using N-version programming. Comment on whether or not you think this is a good suggestion. 
		I believe it’s a good idea as it introduces redundancy and language diversity to the control software
	11.9 Explain why you should explicitly handle all exceptions in a system that is intended to have a high level of availability. 
		Exceptions in a critical system must be addressed and handled explicitly to make sure all issues that caused the exception aren’t allowed to continue, which it might if it were ignored or implicitly handled.
	12.5 A train protection system automatically applies the brakes of a train if the speed limit for a segment of track is exceeded, or if the train enters a track segment that is currently signaled with a red light (i.e., the segment should not be entered). There are two critical-safety requirements for this train protection system: 
		The train shall not enter a segment of track that is signaled with a red light. 
		The train shall not exceed the specified speed limit for a section of track. 
	Assuming that the signal status and the speed limit for the track segment are transmitted to on-board software on the train before it enters the track segment, propose five possible functional system requirements for the onboard software that may be generated from the system safety requirements.
		1.	An alarm shall sound if a software anomaly is detected
		2.	While alarm sounds, the brakes shall be applied until anomaly is fixed
		3.	If speed reaches maximum and is accelerating, the brakes shall apply
		4.	If a red light is detected, apply brakes
		5.	Check functionality of system every 5 minutes
