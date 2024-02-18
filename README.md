# Wildre-Shared-task-baselines and coda lab

The [Code-mixed Less-Resourced Sentiment analysis (Code-mixed) for Indo-Aryan languages Shared Task](https://github.com/wildre-workshop/wildre-7_code-mixed-sentiment-analysis/) is a part of the 7th Workshop on Indian Language Data: Resources and Evaluation (WILDRE-7).

## Introduction: 
<p align="justify"> Code-mixing, the dynamic interplay of multiple languages within a single discourse, is a widespread linguistic phenomenon observed in multilingual societies. Code-mixing is particularly intriguing when observed in closely related languages. In such linguistic scenarios, where language boundaries are blurred, code-mixing becomes a dynamic expression of linguistic fluidity. Closely related languages share lexical and syntactic similarities, allowing for seamless transitions between them in communication. This phenomenon reflects the intertwined linguistic histories and presents a rich tapestry of expression. The nuances of code-mixing in closely related languages highlight the intricate ways in which linguistic diversity is woven into everyday discourse, showcasing the versatility and adaptability of language in diverse linguistic landscapes. The pervasive use of the Internet and social media platforms has led to the digital availability of most languages. This digital accessibility has paved the way for a myriad of artificial intelligence (AI) applications. Among these applications, sentiment analysis, machine translation, and hateful content detection stand out. Despite the increasing digital availability of languages due to the Internet and social media, the need for curated datasets for developing AI applications in many languages remains a significant challenge. Notably, numerous Indo-Aryan languages have been underrepresented in terms of linguistic resources. In recent years, demand has increased to create code-mixed and under-resourced Indo-Aryan languages. However, the effectiveness of existing natural language processing (NLP) techniques in utilizing these datasets and the need for novel techniques present key research areas. Understanding the applicability of current NLP methods and innovating new approaches will be crucial in maximizing the potential impact of these datasets across a spectrum of AI applications. 

<p align="justify"> Sentiment analysis stands as a classic challenge in computational linguistics, demonstrating a profound impact on various real-world applications.  While sentiment analysis as a field has been expanding, and numerous shared tasks have been organised from time to time, some of them are (Patra et al., 2016) ( Patwa et al., 2020), (Chakravarthi et al., 2021), (Debasis et al., 2022),  (Chakravarthi et al., 2022), (Premjith et al., 2023) (Hedge et al., 2023) and so on. However, none of these shared tasks focused on code-mixed closely related low-resource Indo-Aryan languages. Systems have made remarkable progress in setting new performance standards, but the effectiveness of sentiment prediction in the context of code-mixed data still needs to be improved. This limitation is primarily attributed to the variability in language availability and the quality of training data, which directly impacts the precision of sentiment analysis. </p>

## Task Description

<p align="justify">  This shared task addresses the complexities of code-mixed data from less-resourced similar languages and focuses on sentiment analysis. The task builds on code-mixed sentiment analysis but introduces language pairs and triplets of less-resourced closely related languages, Magahi-Hindi-English, Maithili-Hindi, Bangla-English-Hindi, and Hindi-English. These four languages come from the Indo-Aryan language family and are spoken in eastern India. Considering the challenges of processing closely related languages in code-mixed and low-resourced settings, we urge the participants to explore different Machine learning and Deep learning approaches to train the model on the given training and validation dataset. In this context, we will provide Hindi-English, Bangla-English and Magahi-Hindi-English datasets for training and validation. This task will allow the participants to use any approach to train their model that is robust enough to perform well on a closely related code-mixed language dataset. This would also allow us to understand the language representation in various code-mixed settings and the speakers' preference of language to express their emotions in each language pair. </p>

## Data
 We will provide annotated data for code-mixed languages (Magahi-Hindi-English, Bangla-English-Hindi, Hindi-English). Each code-mixed comment/sentence in Magahi-Hindi-English and Hindi-English is labeled with four sentiment labels (Positive, Negative, Neutral or Mixed). However, the Bangla-English-Hindi is labelled with only three sentiment labels (positive, negative or neutral). The data for Magahi-Hindi-English and Hindi English is collected from various YouTube channels and were annotated with the help of native speakers of the language. For Bangla-English code-mixed data set we are using [**SentMix-3L**](https://github.com/LanguageTechnologyLab/SentMix-3L) dataset (Raihan, et al., 2023). 

**NB !** In addition to this, the shared task allows participants to use external resources as long as they are openly available and can be, in theory, used by other participants for research purposes. In case participants decide to use external resources they should use proper citation and provide the details of the dataset in the system description paper.

#### Data Format
|sentence|sentiment|
|:------|:----|
|We support khan sir, jinko problem hai khan sir ke video se vo Pakistan ja Sakta hai.|MIX|
|साहेब का नया ऐलान"गोली खाइबा कपार में, तबे परिवार के  नौकरी मिलहै बिहार में"🙁|Negative|
|khub sundar Magahi geet hkai|Positive|
|জাস্ট হোইপেড উপ আ সিম্পল মেল ফর মাইসেলফ/ময় ফ্যামিলি এন্ড ফিলিং প্রেটি প্রাউড অফ ইট! টেকআউটের order দেওয়া থেকে বিরতি নেওয়া এবং scratch থেকে খাবার রান্না করা সবসময়ই ভালো। Plus, it's usually স্বাস্থ্যকর and saves money in the long run.  आज रात का मेनू: स्पेगेटी और मीटबॉल एक साइड सलाद के साथ। yam! #homaichooking #spaghaittinight #simlanddailichious #haialthyaiating #chivilmonaiy|Neutral|
|2022 Mai vhi kon kon iss song ko Sunna Raha hai|Positive|

## Evaluation 
<p align="justify"> The shared task is hosted on CodaLab. The standard evaluation metrics for evaluating and ranking the teams will be the average F1 score. However, we will release the F1 score, precision and recall across the four classes for a detailed discussion and error analysis. Each participating team will initially have access to the training and validation data only. Later, test data will be released along with the Maithili test set for zero-shot evaluation. We will make no distinction between constrained and unconstrained systems, but the participants are instructed to report the additional resources used for each submission.</p>

The evaluation will be in two different Tracks:

**A. Track 1:** Given training and validation data to determine the polarity (positive, negative , neutra or mixed) of the comment in the same code-mixed setting.
  1. Hindi-English
  2. Magahi-Hindi-English
  3. Bangla-English
  4. Combined all the language pairs (1+2+3)

**B. Track 2:** Given unlabelled test data for the code-mixed Maithili language (Maithi-Hindi-English) leverage any or all of the available training datasets in Track 1 to determine the sentiment of a comment in the target language. 

<p align="justify"> **NB!** The dataset are divided into the train, validation and test sets with the ratio of 70:15:15. However, for the fourth part of Track 1 (Combined all the language pairs), combine the provided training and validation dataset of each code-mixed language to train the model. </p>

## System Submission Format
The participants are requested to submit their predictions on [CodaLab](https://codalab.lisn.upsaclay.fr/). 



## Paper submission 
<p align="justify"> Participants will be invited to describe their system in a paper for the WILDRE7 workshop proceedings. The task organisers will write an overview paper describing the task, summarising the approaches taken, and analyse their results. 

Paper submission instructions will be the same as for the [workshop](http://sanskrit.jnu.ac.in/conf/wildre7/index.jsp). Each team participating in the shared task is expected to submit a system description paper of 4 to 5 pages, plus additional pages for references, formatted according to the workshop guidelines. The paper should describe the system and the resources used along with the libraries. The methodology/strategy should be documented in such a way that the readers and other researchers are able to replicate the work from the system description in the paper. </p>

# Shard Task Dates
```
Dec 22, 2023: Registration- https://forms.gle/HVRK1W1hHqBwtgpu6
Jan 10, 2024: Train and Validation Data set Release [to get the data please register]
Feb 15, 2024: Test Set Release
Feb 23, 2024: System Submission Due
Feb 29, 2024: System Results
March 15, 2024: System Description Paper Due
March 28, 2024: Paper notification of acceptance
```

## Important Links
[**Registration**](https://forms.gle/HVRK1W1hHqBwtgpu6) <br>
[**Worshop Page**](http://sanskrit.jnu.ac.in/conf/wildre7/index.jsp)<br>

## Task Organizers 

* **Priya Rani**, SFI Centre for Research and Training in AI, Data Science Institute, University of Galway 
* **Gaurav Negi**, Insight SFI Research Centre for Data Analytics, Data Science Institute, University of Galway 
* **Saroj Jha**, Indian Institute of Technology, Patna, India
* **Shardul Suryawanshi**, Insight SFI Research Centre for Data Analytics, Data Science Institute, University of Galway 
* **John P. McCrae**, Insight SFI Research Centre for Data Analytics, Data Science Institute, University of Galway
* **Paul Buitelaar**, Insight SFI Research Centre for Data Analytics, Data Science Institute, University of Galway

**Overview**
* **Atul Kr. Ojha**, Insight SFI Research Centre for Data Analytics, Data Science Institute, University of Galway
* **Girish Nath Jha**, Chairman, Commission for Scientific and Technical Terminology, MoE, GOI (on deputation from Jawaharlal Nehru University, India)
* **Sobha L.**, AU-KBC, Anna University
* **Kalika Bali**, Microsoft Reseach, India

## References 

1. Patra, Braja Gopal, Dipankar Das, Amitava Das and R. Rajendra Prasath. 2015. Shared Task on Sentiment Analysis in Indian Languages (SAIL) Tweets - An Overview. In: Prasath, R., Vuppala, A., Kathirvalavakumar, T. (eds) Mining Intelligence and Knowledge Exploration. MIKE 2015. Lecture Notes in Computer Science(), vol 9468. Springer, Cham. https://doi.org/10.1007/978-3-319-26832-3_61

2. Parth Patwa, Gustavo Aguilar, Sudipta Kar, Suraj Pandey, Srinivas PYKL, Björn Gambäck, Tanmoy Chakraborty, Thamar Solorio, and Amitava Das. 2020. SemEval-2020 Task 9: Overview of Sentiment Analysis of Code-Mixed Tweets. In Proceedings of the Fourteenth Workshop on Semantic Evaluation, pages 774–790, Barcelona (online). International Committee for Computational Linguistics.

3. Koustava Goswami, Priya Rani, Bharathi Raja Chakravarthi, Theodorus Fransen, and John P. McCrae. 2020. ULD@NUIG at SemEval-2020 Task 9: Generative Morphemes with an Attention Model for Sentiment Analysis in Code-Mixed Text. In Proceedings of the Fourteenth Workshop on Semantic Evaluation, pages 968–974, Barcelona (online). International Committee for Computational Linguistics.
  
5. Bharathi Raja Chakravarthi, Ruba Priyadharshini, Sajeetha Thavareesan, Dhivya Chinnappa, Durairaj Thenmozhi, Elizabeth Sherly, John P. McCrae, Adeep Hande, Rahul Ponnusamy, Shubhanker Banerjee, Charangan Vasantharajan. 2021. Findings of the Sentiment Analysis on Dravidian Languages in Code-Mixed Text. In Proceedings of the 13th Forum for Information Retrieval Evaluation, Gandhinagar, India.

6. Subalalitha Chinnaudayar Navaneethakrishnan, Bharathi Raja Chakravarthi, Kogilavani Shanmugavadivel, Malliga Subramanian, Prasanna Kumar Kumaresan, Bharathi, Lavanya Sambath Kumar, and Rahul Ponnusamy. 2023. Findings of shared task on Sentiment Analysis and Homophobia Detection of YouTube Comments in Code-Mixed Dravidian Languages. In Proceedings of the 14th Annual Meeting of the Forum for Information Retrieval Evaluation (FIRE '22). Association for Computing Machinery, New York, NY, USA, 18–21. https://doi.org/10.1145/3574318.3574347

7. Premjith B, Jyothish Lal G, Sowmya V, Bharathi Raja Chakravarthi, Rajeswari Natarajan, Nandhini K, Abirami Murugappan, Bharathi B, Kaushik M, Prasanth Sn, Aswin Raj R, and Vijai Simmon S. 2023. Findings of the Shared Task on Multimodal Abusive Language Detection and Sentiment Analysis in Tamil and Malayalam. In Proceedings of the Third Workshop on Speech and Language Technologies for Dravidian Languages, pages 72–79, Varna, Bulgaria. INCOMA Ltd., Shoumen, Bulgaria.

8. Asha Hegde, Bharathi Raja Chakravarthi, Hosahalli Lakshmaiah Shashirekha, Rahul Ponnusamy, Subalalitha Cn, Lavanya S K, Thenmozhi D., Martha Karunakar, Shreya Shreeram, and Sarah Aymen. 2023. Findings of the Shared Task on Sentiment Analysis in Tamil and Tulu Code-Mixed Text. In Proceedings of the Third Workshop on Speech and Language Technologies for Dravidian Languages, pages 64–71, Varna, Bulgaria. INCOMA Ltd., Shoumen, Bulgaria.

9. Md Nishat Raihan, Dhiman Goswami, Antara Mahmud, Antonios Anastasopoulos, Marcos Zampieri.2023.SentiMix-3L: A bangls-English-Hindi code-mixed Dataset for Sentiment Analysis. In Proceedings of The First Workshop in South East Asian Language Processing. Nusa Dua, Bali.


# License
Please see the [LICENSE](https://github.com/wildre-workshop/wildre-7_code-mixed-sentiment-analysis/blob/main/LICENSE) file.

# Acknowledgments

We would like to thank [Science Foundation Ireland (SFI)](https://www.sfi.ie/) grant number [SFI/12/RC/2289_ P2 Insight _ 2](https://www.insight-centre.org/) and [SFI/18/CRT/6223](https://www.crt-ai.ie/).
