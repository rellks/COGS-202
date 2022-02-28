### Introduction
A common approach to analyzing EEG data is as a dynamical system, where the state of the system is the combination of all variables describing that system at any given time, and the dynamics of the system describe the change of state over time (Khanna et al., 2015). If we look at momentary states of the system based on changes in brain activity, we can parse EEG data into a limited number of quasi-stable states, or “microstates” (Lehmann et al., 1987). Analysis of microstates has favored resting-state EEG data, so much is uncertain about the nature of microstates in task-driven events. There still exists much disagreement on the number of microstates and topographies of electromagnetic charge of the microstates during ERP tasks. The proposed study will explore the nature of microstates in both visual and auditory-driven tasks to better understand how many and what kind of microstates exist in said tasks.

### Methods
Participants would be recruited from the UC Merced undergraduate population pool, receiving either course credit or cash. Participants would be screened for history of neurological or psychological illnesses and handedness.
	  
Procedure for this task would include participating in 2 tasks: 1 visual and 1 auditory oddball task. Oddball tasks are “the most common EEG paradigm” (Kappenman and Luck, 2010), allowing results to be generalized across many similar tasks in the field. The visual oddball would consist of 2 types of stimuli: letters or numbers. Participant would be instructed to press one button for one stimuli, and another button for the other. The type of stimuli participants would see would vary between blocks; letters may appear 80% of the time and numbers, 20% (i.e. the oddball). The same procedure would occur for the auditory oddball, but the 2 types of stimuli would be a low and high tone. Oddballs and presentation of blocks would be counterbalanced across participants. Participants would also undergo resting-state EEG data collection to establish baseline brain activity.
	
EEG acquisition would take place using a 32 channel EEG cap. Data would be preprocessed in MATLAB, using EEGLAB (Delorme and Makeig, 2004) and ERPLAB Toolbox (Lopez-Calderon and Luck, 2014). Data would be processed in Microstate EEGLAB Toolbox (Poulsen et al., 2018), where preprocessed data would be concatenated by taking the grand average ERPs and microstate segmentation would take place to fit the best amount of microstates and topographies that best represent the data.

### Results
Statistical fields reported would include Global Explained Variance (GEV) and the averaged spatial correlation (Corr), which reflect the extent to which the microstates found can explain the given data. Statistics would also be calculated for the basic temporal dynamics of the microstates, including Occurrence, Duration, and Coverage. Data from subjects’ first block of tasks would then be used to train a classifier that would be able to predict trial accuracy based on what microstate a participant was in. Creating a successful classifier would validate microstate segmentation and assignment, as well as align with previous literature (see: Britz and Michel, 2010; Britz et al. 2014).
	
Expected results would include high GEV and Corr, but high temporal dynamic statistics for only 1, possibly 2, microstates since this is a task-oriented study and one microstate would likely dominate for the given task. Expected results would also include a successful classification model. Ideally, this model would also be tested and run successfully from oddball data collected outside of this study, further increasing its validation and generalizability.

### Conclusion
Successful findings from this proposed study would offer preliminary results to the understanding of microstates and their nature in task-oriented situations. This study would potentially lay the foundation for future research in this domain, providing replicable results and the needs for expansion on the current proposed hypothesis.

### References

Britz J, Diaz Hernandez L, Ro T, Michel CM. EEG-microstate dependent emergence of perceptual awareness. Frontiers in behavioral neuroscience. 2014; 8:163. [PubMed: 24860450]

Britz J, Michel CM. Errors can be related to pre-stimulus differences in ERP topography and their concomitant sources. NeuroImage. 2010; 49:2774–2782. [PubMed: 19850140]

Delorme A, Makeig S. EEGLAB: an open source toolbox for analysis of single-trial EEG dynamics including independent component analysis. J Neurosci Methods. 2004 Mar 15;134(1):9-21. doi: 10.1016/j.jneumeth.2003.10.009. PMID: 15102499.

Kappenman, E. S., & Luck, S. J. (2010). The effects of electrode impedance on data quality and statistical significance in ERP recordings. Psychophysiology, 47(5), 888–904. https://doi.org/10.1111/j.1469-8986.2010.01009.x

Khanna, A., Pascual-Leone, A., Michel, C. M., & Farzan, F. (2015). Microstates in resting-state EEG: Current status and future directions, Neuroscience & Biobehavioral Reviews, Volume 49, 2015, Pages 105-113, ISSN 0149-7634, https://doi.org/10.1016/j.neubiorev.2014.12.010.

Lehmann, D., Ozaki, H., & Pal, I. (1987). EEG alpha map series: brain micro-states by space-oriented adaptive segmentation, Electroencephalography and Clinical Neurophysiology, Volume 67, Issue 3, 1987, Pages 271-288, ISSN 0013-4694, https://doi.org/10.1016/0013-4694(87)90025-3.
Lopez-Calderon J, Luck SJ. ERPLAB: an open-source toolbox for the analysis of event-related potentials. Front Hum Neurosci. 2014 Apr 14;8:213. doi: 10.3389/fnhum.2014.00213. PMID: 24782741; PMCID: PMC3995046.

Poulsen, A. T., Pedroni, A., Langer, N., & Hansen, L. K. (2018). Microstate EEGlab toolbox: An introductory guide. bioRxiv.

