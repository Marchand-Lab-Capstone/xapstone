# Components

## Big Idea/Script Components 

### Command Line 
This would be the main UI for users. A user would call ```python xenofind.py [method] [fast5/pod5 directory] [reference fasta]``` with required inputs. Progress and errors would show up here.

### xenofind_pipe.py 
This will be the other 'UI' for users. Users would input where they want the working directory to be, as well as the directories for inputted fast5/pod5 and the reference fasta for basecalling. In addition, you would set which detection method you would want to use on this script. This is essenetially pretty much the same as running the command line as mentioned above except it those inputs would be stored and easy to see. 

### xenofind.py
This is the primary script. This will call the desired detection method in the ```lib``` directory regard if it is called using the command line or xenofind_pipe.py. 

### xf_params
This will contain the parameters used in any of the detection methods such as the path for the basecaller. It also contains toggleable variables to only run certain parts of the script (e.g., initial basecall). This is imported into most of the scripts in this program. 

### xf_tools 
This script contains all the reusable, general functions that can be called as needed (e.g., fast5 to pod5 conversion). This script is imported to most of the scripts in this program. 

### xf_low_qual.py
This script outlines the first approach for identifying potential positions of XNA bases with limited accuracy and precision. In this method, the raw datasets will be merged and basecalled into a ```.bam``` file, and the features of the reads in the bam file will be generated. Then it conducts a statistical test to identify low-quality scores on a per-read basis. Following this assessment, the reads are recentered and grouped to the reference sequence. Finally, positions with low-quality scores indicative of XNA presence are extracted.

### extract_read_info function
This function takes in the merged bam file and extracts the readID, basecalled sequence, start of reference sequence, the quality socre per base and the average quality score of each read.

### xna_guess function
This function performs a statistical test on a per base read to indentify low-quality scores, recenters and groups the reads to the reference sequence, and extracts the positions indicative of the XNA presence.