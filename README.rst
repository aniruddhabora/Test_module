### **Code Setup**
 
1. Encoder Decoder output
	
	To see the encoder decoder outputs for a particular Field Variable:
			
			* open the job_sbatch file.
			
			* Enter the datapath in which the data is in  *DATAPATH=''*. For example if you have the data in the path *'/Users/abora/NEW_AE_DATA/', then enter DATAPATH='/Users/abora/NEW_AE_DATA/'.
			
			* We have three kinds of data in three different folders:
						* 	 'NDG_TEND/' : for the nudging tendency data
						*    'BF_NDG/': for the before nudged data
						*    'REF/' : for the reference data
			    Based on whichver data we want type the folder name in FOLDER_NAME=''. For example if we want the data for nudging tendency enter FOLDER_NAME='NDG_TEND/'.
			    
			* Enter the state variable name in the FIELD="" . For example if you want to see the results for U type FIELD="U".
			
			* Enter the time for which you want to see the plots in PLOT_TIME= . For example you want to see the plot for t=100, then enter PLOT_TIME=100.
			
			* Make an empty folder Figs in same directy as where the code is to save all the figures. 
			
			* Now type sbatch job.sbatch in your terminal.
