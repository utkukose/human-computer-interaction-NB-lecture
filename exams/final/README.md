<div align="center">

# Final project: An interface with an artificial intelligence (AI) feature, designed and evaluated

**Human-Computer Interaction (BIL-429 İnsan-Bilgisayar Etkileşimi)**  
Prof. Dr. Utku Kose, Süleyman Demirel University

</div>

## Overview

The final project takes an interface with an artificial intelligence (AI) feature of the student's choice along the stages of the clinic app. These are a baseline, an evaluation, a redesign, a test and an AI feature measured for reliance [1]. It combines the methods of the whole course, with the weight on Weeks 9 to 14. Choose one of the three options below, and extend its starter Colab notebook with the data of your own interface. Timing: Released in Week 12, due at the end of Week 14. The final project counts 60 percent of the course grade.

## Learning outcomes assessed

Course learning outcomes 1, 5, 6, 7 and 8 (see the [course README](../../README.md)).

## Options

### Final option 1: An assistant that suggests

Take an interface in which an AI suggests something that the user accepts or changes, such as a category, a reply, a tag or a route. Log at least 200 suggestions with their confidence and their right answers. Check whether the confidence is honest with a reliability table, the expected calibration error and the Brier score (Week 13) [2, 3]. Choose a threshold below which the interface lets the user decide alone, and estimate the accuracy of the team [4, 5]. Test the current design against the redesign with participants. Measure completion, time on task, the System Usability Scale (SUS) and the share of wrong suggestions that they accepted (Week 9) [6, 7]. Close with an accessibility audit of the AI feature (Week 10) [8].

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/utkukose/human-computer-interaction-NB-lecture/blob/main/exams/final/FIN1_assistant_that_suggests.ipynb) Starter Colab notebook: [`FIN1_assistant_that_suggests.ipynb`](FIN1_assistant_that_suggests.ipynb). Its example case: An expense app whose assistant suggests the category of a receipt.

### Final option 2: A conversational interface

Design a chatbot or a voice assistant for a task with a few slots, such as booking a court, ordering a meal or reporting a fault. Write its dialogue manager as a state machine with tests, and choose when it asks back from the error rate and the confidence measured in a test (Week 14) [9]. Test it with participants, and explain their satisfaction by task success and the costs of the dialogue with PARADISE (PARAdigm for DIalogue System Evaluation) [10]. Review the paths of consent and cancellation for dark patterns, and evaluate a rule that hands conversations over to a person [11, 12]. Check that the prompts use plain words (Week 10) [13].

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/utkukose/human-computer-interaction-NB-lecture/blob/main/exams/final/FIN2_conversational_interface.ipynb) Starter Colab notebook: [`FIN2_conversational_interface.ipynb`](FIN2_conversational_interface.ipynb). Its example case: A chatbot that books a court at the sports centre of a university.

### Final option 3: A mobile assistant with voice and suggestions

Take a mobile app with voice input and an assistant that makes suggestions, such as a to-do app, a calendar or a navigation app. Measure the word error rate of its voice commands and the effect of a read-back (Week 11) [14]. Estimate how often its notifications interrupt focused work, and how a batched delivery would change it (Week 11) [15]. Model how the trust of its users follows the reliability of the suggestions, also after an update, and compare a display of the recent reliability (Week 13) [4, 16]. Close with a usability test of voice against touch input (Week 9) [7].

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/utkukose/human-computer-interaction-NB-lecture/blob/main/exams/final/FIN3_mobile_voice_and_suggestions.ipynb) Starter Colab notebook: [`FIN3_mobile_voice_and_suggestions.ipynb`](FIN3_mobile_voice_and_suggestions.ipynb). Its example case: A to-do app with voice commands and an assistant that suggests when to remind its user.

## Proposal

The final project starts with a proposal of about 500 words, written in Week 12. It names the interface and its AI feature, the users and their main task, and the option with its methods. It plans the test with the number of participants and the measures, and it states how consent is asked and how the data are kept anonymous. During active semesters, the proposal can be sent to utkukose@sdu.edu.tr or utkukose@gmail.com for early feedback.

## Example proposals

Two example proposals show the expected scope and level of detail. Each follows the parts of the proposal above. Students write their own proposals in the same way for the interface of their choice.

### Category suggestions at the help desk of a computer centre (Option 1)

**The interface and its AI feature.** Students report problems with the services of a university computer centre in a web form. An assistant suggests the category of each request from its text: Network, e-mail, printing, accounts or software. The staff of the help desk accept the suggestion or change it, and a wrong category sends the request to the wrong team. The assistant is a text classifier with scikit-learn, trained on 1,500 past requests that the centre anonymised. It shows the suggestion with its confidence.

**The users and their task.** The users are the five staff members and eight student assistants of the help desk. Their task is to file a request in the right category within a few seconds. The assistants change every semester, so the interface must also suit people in their first week.

**The methods.** A log of 300 new requests with their right categories gives the reliability table, the expected calibration error and the Brier score of the confidence. The threshold of the redesign maximises the accuracy of the team, with the accuracy of a member of staff who decides alone measured on 40 requests. A heuristic evaluation by three classmates checks the screen of the suggestion before the test.

**The test plan.** Twelve participants file 20 requests each, four of them with a wrong suggestion. Half of them start with design A, the suggestion alone, and half with design B, which adds the confidence and leaves uncertain requests to the user. The measures are completion, the time per request, the System Usability Scale and the share of wrong suggestions accepted. An audit of the contrast, the target sizes and the plain words of design B closes the evaluation.

**Consent and data.** The participants read a short information sheet and agree in writing. The requests come from the centre without names, e-mail addresses or student numbers, and the Colab notebook keeps only a code for each participant.

### A chatbot for the practice rooms of a music department (Option 2)

**The interface and its AI feature.** Students book the practice rooms of a music department by e-mail today, and double bookings are common. A chatbot on the website of the department takes the booking in a conversation with three slots: The room, the day and the hour. A simple classifier recognises the intent of each message, and a matcher fills the slots with a confidence.

**The users and their task.** The users are about 200 students of the department, many of whom book on their phone between lessons. Their task is to book, move or cancel a room in less than a minute. The secretary of the department handles complaints and broken instruments.

**The methods.** The dialogue manager is a state machine with a test for every path. A test of 60 values gives the error rate and the ranges of the confidence, and these decide whether the chatbot asks back below a threshold. A review checks the newsletter of the department and the cancellation for dark patterns, and a rule hands complaints and urgent messages over to the secretary.

**The test plan.** Fifteen students do four tasks each and rate their satisfaction from 1 to 7. PARADISE explains the ratings by task success and the number of turns. The rule for the handover is evaluated on 40 labelled conversations of the test, and the grade level of every prompt is checked.

**Consent and data.** The students agree to take part after a short explanation and may stop at any time. The conversations are stored without names, and the Colab notebook keeps only the codes of the participants.

## Deliverables

An executed Colab notebook with all outputs, the report as a PDF, the interactive prototype as a link or as files, and the anonymised data of the test. The report has 1500 to 2500 words and follows the sections of the Word template [REPORT_TEMPLATE.docx](../REPORT_TEMPLATE.docx). File names start with the student number.

## Evaluation

| Criterion | Weight |
|---|---|
| Problem, users and the AI feature | 10 % |
| Prototype and implementation in the Colab notebook | 20 % |
| Design of the evaluation: participants, measures and comparisons | 20 % |
| Measures of the AI feature: calibration, reliance, trust or conversation | 20 % |
| Accessibility, ethics and honest discussion of the limitations | 15 % |
| Report quality, figures and references | 10 % |
| Statement on tools and responsible use | 5 % |

## Studies with people

Surveys, first-click tests, card sorts and usability tests with real people make a project stronger. Ask every participant for consent, explain the purpose, let people stop at any time and keep the data anonymous, as the syllabus asks. No names, e-mail addresses or other personal data enter the Colab notebook or the report. Simulated data are acceptable where real data cannot be collected, if the report says so clearly and explains how they were simulated.

## Submission

During active semesters, the deadline and the submission channel are announced by the instructor. Reports and Colab notebooks can be sent to utkukose@sdu.edu.tr or utkukose@gmail.com. Self-learners are welcome to complete the projects for their own portfolios. The policy on generative artificial intelligence tools in the [syllabus](../../SYLLABUS.md) applies.

## References

[1] Amershi, S., Weld, D., Vorvoreanu, M., Fourney, A., Nushi, B., Collisson, P., Suh, J., Iqbal, S., Bennett, P. N., Inkpen, K., Teevan, J., Kikin-Gil, R., & Horvitz, E. (2019). Guidelines for human-AI interaction. In *Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems* (pp. 1-13). ACM. <https://doi.org/10.1145/3290605.3300233>

[2] Guo, C., Pleiss, G., Sun, Y., & Weinberger, K. Q. (2017). On calibration of modern neural networks. In *Proceedings of the 34th International Conference on Machine Learning* (Proceedings of Machine Learning Research, Vol. 70, pp. 1321-1330). PMLR. <https://proceedings.mlr.press/v70/guo17a.html>

[3] Brier, G. W. (1950). Verification of forecasts expressed in terms of probability. *Monthly Weather Review*, *78*(1), 1-3. <https://doi.org/10.1175/1520-0493(1950)078<0001:VOFEIT>2.0.CO;2>

[4] Lee, J. D., & See, K. A. (2004). Trust in automation: Designing for appropriate reliance. *Human Factors*, *46*(1), 50-80. <https://doi.org/10.1518/hfes.46.1.50_30392>

[5] Bansal, G., Wu, T., Zhou, J., Fok, R., Nushi, B., Kamar, E., Ribeiro, M. T., & Weld, D. (2021). Does the whole exceed its parts? The effect of AI explanations on complementary team performance. In *Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems* (pp. 1-16). ACM. <https://doi.org/10.1145/3411764.3445717>

[6] Brooke, J. (1996). SUS: A 'quick and dirty' usability scale. In P. W. Jordan, B. Thomas, B. A. Weerdmeester, & I. L. McClelland (Eds.), *Usability Evaluation in Industry* (pp. 189-194). Taylor & Francis. <https://doi.org/10.1201/9781498710411-35>

[7] Sauro, J., & Lewis, J. R. (2016). *Quantifying the User Experience: Practical Statistics for User Research* (2nd ed.). Morgan Kaufmann. <https://shop.elsevier.com/books/catalog/isbn/9780128023082>

[8] Campbell, A., Adams, C., Bradley Montgomery, R., Cooper, M., & Kirkpatrick, A. (Eds.). (2023). *Web Content Accessibility Guidelines (WCAG) 2.2* (W3C Recommendation). World Wide Web Consortium. <https://www.w3.org/TR/WCAG22/>

[9] Clark, H. H., & Brennan, S. E. (1991). Grounding in communication. In L. B. Resnick, J. M. Levine, & S. D. Teasley (Eds.), *Perspectives on socially shared cognition* (pp. 127-149). American Psychological Association. <https://doi.org/10.1037/10096-006>

[10] Walker, M. A., Litman, D. J., Kamm, C. A., & Abella, A. (1997). PARADISE: A framework for evaluating spoken dialogue agents. In *Proceedings of the 35th Annual Meeting of the Association for Computational Linguistics and 8th Conference of the European Chapter of the Association for Computational Linguistics* (pp. 271-280). Association for Computational Linguistics. <https://doi.org/10.3115/976909.979652>

[11] Gray, C. M., Kou, Y., Battles, B., Hoggatt, J., & Toombs, A. L. (2018). The dark (patterns) side of UX design. In *Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems* (pp. 1-14). ACM. <https://doi.org/10.1145/3173574.3174108>

[12] European Parliament and Council of the European Union. (2024). Regulation (EU) 2024/1689 of the European Parliament and of the Council of 13 June 2024 laying down harmonised rules on artificial intelligence and amending Regulations (EC) No 300/2008, (EU) No 167/2013, (EU) No 168/2013, (EU) 2018/858, (EU) 2018/1139 and (EU) 2019/2144 and Directives 2014/90/EU, (EU) 2016/797 and (EU) 2020/1828 (Artificial Intelligence Act). *Official Journal of the European Union*, L, 2024/1689. <https://eur-lex.europa.eu/eli/reg/2024/1689/oj>

[13] Kincaid, J. P., Fishburne, R. P., Jr., Rogers, R. L., & Chissom, B. S. (1975). *Derivation of new readability formulas (Automated Readability Index, Fog Count and Flesch Reading Ease Formula) for Navy enlisted personnel* (Research Branch Report 8-75). Naval Technical Training Command. <https://doi.org/10.21236/ADA006655>

[14] Koenecke, A., Nam, A., Lake, E., Nudell, J., Quartey, M., Mengesha, Z., Toups, C., Rickford, J. R., Jurafsky, D., & Goel, S. (2020). Racial disparities in automated speech recognition. *Proceedings of the National Academy of Sciences*, *117*(14), 7684-7689. <https://doi.org/10.1073/pnas.1915768117>

[15] Pielot, M., Church, K., & de Oliveira, R. (2014). An in-situ study of mobile phone notifications. In *Proceedings of the 16th International Conference on Human-Computer Interaction with Mobile Devices and Services* (pp. 233-242). ACM. <https://doi.org/10.1145/2628363.2628364>

[16] Dietvorst, B. J., Simmons, J. P., & Massey, C. (2015). Algorithm aversion: People erroneously avoid algorithms after seeing them err. *Journal of Experimental Psychology: General*, *144*(1), 114-126. <https://doi.org/10.1037/xge0000033>
