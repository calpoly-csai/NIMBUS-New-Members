# NIMBUS-New-Members

As new members are introduced to the project, the scripts used to develop the wake word solution will be made available here. 

## Audio Data Collection

First, we need data. To obtain audio data for the wake word, please view the audio recording script ```Audio_Data_Recording.py```
To run this program, you must ensure that you have the following:

1. Python 3.x
2. Pyaudio (python -m pip install pyaudio)
3. Wave (pip install wave)

Also, modifications to the script need to be made. 

1. At line 16 of ```Audio_Data_Recording.py```, you must replace None with a string of your last name. 
   Ex: Replace None with "ewenike"
   
2. At line 18 of ```Audio_Data_Recording.py```, you must replace None with a string of the path to this repository in your local machine. 
   Ex: Replace None with "C:\\Users\\Skywalker\\Documents\\NIMBUS-New-Members"
   Note that Windows users need a double backslash as one backslash serves as the escape character and the second serves as the actual        backslash character
   
3. If you are not using Windows, you must change the double backslashs in line 118 to single forward slashes.
   Ex: wf = wave.open("%s\\Data\\%s\\%s" % (PATH...... to wf = wave.open("%s/Data/%s/%s" % (PATH......



After these modifications, your program should run. Label the audio recording with the appropriate name for organization. Format is as follows: 
Wake Word:
      “<ww>_<gender>_<description> _<location>_<noise-level>_<last name>_<first name>_<date>_<your last name>.wav”
Ex: Correct Wake Word Label Example:
	  “ww_m_curious_classroom_q_skywalker_luke_04212019120040_ewenike.wav”
   Incorrect Wake Word Label Example:
  “recording1.wav”

     Not Wake Word:
      “<notww>_<description>_<location>_<noise-level>_<date>_<your last name>.wav”
Ex: Correct Wake Word Label Example:
	  “notww_background_classroom_l_04212019120040_ewenike.wav”
   Incorrect Wake Word Label Example:
  “reco.wav”

Be sure to follow the spec description guidelines in the Data directory for correct description labeling. 

Happy collecting!
