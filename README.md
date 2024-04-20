# WESAD
###  A Multimodal Dataset for Wearable Stress and Affect Detection
##### Group 3: Tongxin Shi, Talia Zhuang, Shijia Ren, Yuqing Liu, Junjie Wu

----------

### Dataset Information [1]:
Data Set Information:

"WESAD is a publicly available dataset for wearable stress and affect detection. This multimodal dataset features physiological and motion data, recorded from both a wrist- and a chest-worn device, of 15 subjects during a lab study. The following sensor modalities are included: blood volume pulse, electrocardiogram, electrodermal activity, electromyogram, respiration, body temperature, and three-axis acceleration. Moreover, the dataset bridges the gap between previous lab studies on stress and emotions, by containing three different affective states (neutral, stress, amusement). In addition, self-reports of the subjects, which were obtained using several established questionnaires, are contained in the dataset. Details can be found in the dataset's readme-file, as well as in [1].


Data Collection: Collected from physiological and motion sensors.
Devices used: Empatica E4 (wrist-worn) and RespiBAN (chest-worn)
Study Context: Included 15 subjects during a stress-affect lab study
Datasets: https://archive.ics.uci.edu/ml/datasets/WESAD+%28Wearable+Stress+and+Affect+Detection%29



### Classes

**Baseline condition**: 20 minute period of standing/sitting reading magazines.<br>
**Amusement condition**: During the amusement condition, the
subjects watched a set of eleven funny video clips.<br>
**Stress condition**: Trier Social Stress Test (TSST), consisting of public speaking and mental arithmetic.

### Documents
** API.ipynb: Web development by using Python Flask
** pickle_to_csv.ipynb: The raw datasets are pickle file which is not east to processed, so we transfer the pickle file to csv file.
** combine_table&csv_to_DB.ipynb: Each raw csv file contain only one attribute for one participant, so we combine attributes(tables) for each participant (10 participants in total) and store them into database by using PostgreSQL.
** PI_readme_final.ipynb: Store the personal information into MongoDB database. 
** quest to mongodb.ipynb: Store the quest result into MongoDB database.
** Data_Wrangling.ipynb: Data wrangling process was inspired by [3], which follow by the idea from the original research [1].
** Training_model.ipynb: Use the processed database to train models and predict the classes (Baseline, Amusement, and Stress)
** readme_parser.py: Aimimg for merge personal information data with feature data. Code adapted from: https://github.com/WJMatthew/WESAD.git

  


------------
   
#### References

[1] Schmidt, Philip & Reiss, Attila & Duerichen, Robert & Marberger, Claus & Van Laerhoven, Kristof. (2018). Introducing WESAD, a Multimodal Dataset for Wearable Stress and Affect Detection. 400-408. 10.1145/3242969.3242985.  https://dl.acm.org/citation.cfm?doid=3242969.3242985

[2] A Greco, G Valenza, A Lanata, EP Scilingo, and L Citi
"cvxEDA: a Convex Optimization Approach to Electrodermal Activity Processing"
IEEE Transactions on Biomedical Engineering, 2015
DOI: 10.1109/TBME.2015.2474131
https://github.com/lciti/cvxEDA

[3] Schmidt, P., Reiss, A., Duerichen, R., Marberger, C., Van Laerhoven, K., & WJMatthew. (Year). WESAD: A publicly available dataset for wearable stress and affect detection. GitHub. https://github.com/WJMatthew/WESAD


#### Useful Resources:
- https://github.com/jaganjag/stress_affect_detection
- https://github.com/arsen-movsesyan/springboard_WESAD
- https://www.birmingham.ac.uk/Documents/college-les/psych/saal/guide-electrodermal-activity.pdf
- http://research.cs.tamu.edu/prism/publications/choi2011ambulatoryStressMonitor.pdf
