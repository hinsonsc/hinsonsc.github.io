# Homework 3: Chapters 11 and 12
	
		11.4:	What is the common characteristic of all architectural styles that are geared to
			supporting software fault tolerance?
	
			They all have software diversity. This means they have redundant services that mean if one implementation fails, there are some number of programs that are still running that keep that service going.

		11.7:	It has been suggested that the control software for a radiation therapy machine, used to treat patients with cancer, should be implemented using N-version programming. Comment on whether or not you think this is a good idea.
	
			N-Version programming is mainly for systems that require high availibility, whereas RTMs are only used for a short amount of time, thus having reliability measures that will assure the patients get the correct doses of radiation is much more important (such as a seperate system to monitor output and can E-Stop the ETM)


		11.9: 	Explain why you should explicitly handle all exceptions in a system that is intended to have a high level of availability.

			High availibility systems usually are high-uptime systems, thus are the most likely to run into errors as they would be running 99.5-99.9% of the time. Thus they need resilience to faults, a way to combat faults is to use exceptions to allow for the system to fail gracefully, log the error, and attempt to restart the service if needed.

		12.5:	A train protection system automatically applies the brakes of a train if the speed limit for a segment of track is exceeded, or if the train enters a track segment that is currently signaled with a red light. There are two critical-safety requirements for this train protection system:
				The train shall not enter a segment of track that is signaled with a red light.
				The train shall not exceed the specified speed limit for a section of track.
			Assuming that the signal status and the speed limit for the track segment are transmitted to on-board software on the train before it enters the track segment, propose five possible functional system safety requirements.
		1.	An alarm shall sound if a software anomaly is detected
		2.	While alarm sounds, the brakes shall be applied until anomaly is fixed
		3.	If speed reaches maximum and is accelerating, the brakes shall apply
		4.	If a red light is detected, apply brakes
		5.	Check functionality of system every 5 minutes
