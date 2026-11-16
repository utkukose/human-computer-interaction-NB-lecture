<div align="center">

# Midterm project: A usability study of an interface

**Human-Computer Interaction (BIL-429 İnsan-Bilgisayar Etkileşimi)**  
Prof. Dr. Utku Kose, Süleyman Demirel University

</div>

## Overview

The midterm project applies the methods of Weeks 1 to 7 to an interface that the student uses in daily life [1]. Examples are an app of a university, a bank or a delivery service, and a public terminal. It studies one important task. The task is modelled, the screens and the users are evaluated, and a redesign is proposed as an interactive prototype with its predicted improvement. Choose one of the three options below, and extend its starter Colab notebook with the data of your own interface. Timing: Released in Week 6, due at the end of Week 7. The midterm project counts 40 percent of the course grade. The optional weekly tasks and research assignments carry no separate weight. They are combined with the midterm component, and the instructor may take them into account as a discretionary adjustment.

## Learning outcomes assessed

Course learning outcomes 1, 2, 3, 4 and 8 (see the [course README](../../README.md)).

## Options

### Midterm option 1: A task in a mobile app

Choose a task that you do often in an app on your phone, such as renewing a book, sending money or ordering a meal. Model the task as a chain of steps with the slips and repairs that you observe (Week 1). Evaluate the screens with at least three evaluators against the ten heuristics, and rank the merged problems by severity (Week 5) [2, 3]. Build personas from a short survey of at least 20 users with k-means, and predict the task time of each persona with the keystroke-level model (Week 6) [4, 5]. Finally, prototype the redesign as a state machine, check that no screen traps its users, and compare the expected taps and times of both designs (Week 7) [6].

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/utkukose/human-computer-interaction-NB-lecture/blob/main/exams/midterm/MID1_mobile_task.ipynb) Starter Colab notebook: [`MID1_mobile_task.ipynb`](MID1_mobile_task.ipynb). Its example case: Renewing a borrowed book in the app of a university library.

### Midterm option 2: A self-service terminal

Choose a self-service terminal in a public place, such as a ticket machine, a parcel locker, a library kiosk or a self-checkout. Measure the size and the colours of its texts. Check them against the critical print size and the contrast ratios of the Web Content Accessibility Guidelines (WCAG) 2.2 (Week 2) [7, 8]. Model the choice in its main menu with search, the Hick-Hyman law and a split menu (Week 3) [9, 10]. Measure its buttons and predict the hit rates of users with steady and with shaking hands (Week 4) [11, 12]. Close with the keystroke-level model of the whole task before and after the redesign (Week 6) [5].

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/utkukose/human-computer-interaction-NB-lecture/blob/main/exams/midterm/MID2_self_service_terminal.ipynb) Starter Colab notebook: [`MID2_self_service_terminal.ipynb`](MID2_self_service_terminal.ipynb). Its example case: Buying a ticket at the ticket machine of a railway station.

### Midterm option 3: Navigation and a form of a website

Choose a website with many pages and an important form, such as the course registration of a university or the booking of a public service. Model its menus by breadth, depth and the scent of the labels, measured with a first-click test (Week 7) [13, 14]. Run an open card sort with at least 12 participants, and cluster the cards into a new menu (Week 7). Check the form for codes that must be recalled and for defaults that decide for the users (Week 3) [15, 16]. Evaluate the registration with at least three evaluators against the heuristics (Week 5) [2].

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/utkukose/human-computer-interaction-NB-lecture/blob/main/exams/midterm/MID3_website_navigation_and_form.ipynb) Starter Colab notebook: [`MID3_website_navigation_and_form.ipynb`](MID3_website_navigation_and_form.ipynb). Its example case: Registering for a course on the website of a university.

## Deliverables

An executed Colab notebook with all outputs, the report as a PDF and the interactive prototype, as a link or as files. The report has 1500 to 2500 words and follows the sections of the Word template [REPORT_TEMPLATE.docx](../REPORT_TEMPLATE.docx). File names start with the student number.

## Evaluation

| Criterion | Weight |
|---|---|
| The interface, the task and its model | 15 % |
| Correctness of the measures and of the code | 25 % |
| The users: survey, personas or measurements | 15 % |
| The redesign and its predicted improvement | 20 % |
| Interpretation and honest discussion of the limitations | 10 % |
| Report quality, figures and references | 10 % |
| Statement on tools and responsible use | 5 % |

## Studies with people

Surveys, first-click tests, card sorts and usability tests with real people make a project stronger. Ask every participant for consent, explain the purpose, let people stop at any time and keep the data anonymous, as the syllabus asks. No names, e-mail addresses or other personal data enter the Colab notebook or the report. Simulated data are acceptable where real data cannot be collected, if the report says so clearly and explains how they were simulated.

## Submission

During active semesters, the deadline and the submission channel are announced by the instructor. Reports and Colab notebooks can be sent to utkukose@sdu.edu.tr or utkukose@gmail.com. Self-learners are welcome to complete the projects for their own portfolios. The policy on generative artificial intelligence tools in the [syllabus](../../SYLLABUS.md) applies.

## References

[1] International Organization for Standardization. (2019). *Ergonomics of human-system interaction - Part 210: Human-centred design for interactive systems* (ISO Standard No. 9241-210:2019). ISO. <https://www.iso.org/standard/77520.html>

[2] Nielsen, J., & Molich, R. (1990). Heuristic evaluation of user interfaces. In *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems* (pp. 249-256). ACM. <https://doi.org/10.1145/97243.97281>

[3] Lewis, J. R. (2001). Evaluation of procedures for adjusting problem-discovery rates estimated from small samples. *International Journal of Human-Computer Interaction*, *13*(4), 445-479. <https://doi.org/10.1207/S15327590IJHC1304_06>

[4] Pruitt, J., & Grudin, J. (2003). Personas: Practice and theory. In *Proceedings of the 2003 Conference on Designing for User Experiences* (pp. 1-15). ACM. <https://doi.org/10.1145/997078.997089>

[5] Card, S. K., Moran, T. P., & Newell, A. (1980). The keystroke-level model for user performance time with interactive systems. *Communications of the ACM*, *23*(7), 396-410. <https://doi.org/10.1145/358886.358895>

[6] Houde, S., & Hill, C. (1997). What do prototypes prototype? In M. G. Helander, T. K. Landauer, & P. V. Prabhu (Eds.), *Handbook of Human-Computer Interaction* (2nd ed., pp. 367-381). Elsevier. <https://doi.org/10.1016/B978-044481862-1.50082-0>

[7] Legge, G. E., & Bigelow, C. A. (2011). Does print size matter for reading? A review of findings from vision science and typography. *Journal of Vision*, *11*(5), 8. <https://doi.org/10.1167/11.5.8>

[8] Campbell, A., Adams, C., Bradley Montgomery, R., Cooper, M., & Kirkpatrick, A. (Eds.). (2023). *Web Content Accessibility Guidelines (WCAG) 2.2* (W3C Recommendation). World Wide Web Consortium. <https://www.w3.org/TR/WCAG22/>

[9] Hick, W. E. (1952). On the rate of gain of information. *Quarterly Journal of Experimental Psychology*, *4*(1), 11-26. <https://doi.org/10.1080/17470215208416600>

[10] Cockburn, A., Gutwin, C., & Greenberg, S. (2007). A predictive model of menu performance. In *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems* (pp. 627-636). ACM. <https://doi.org/10.1145/1240624.1240723>

[11] Fitts, P. M. (1954). The information capacity of the human motor system in controlling the amplitude of movement. *Journal of Experimental Psychology*, *47*(6), 381-391. <https://doi.org/10.1037/h0055392>

[12] MacKenzie, I. S. (1992). Fitts' law as a research and design tool in human-computer interaction. *Human-Computer Interaction*, *7*(1), 91-139. <https://doi.org/10.1207/s15327051hci0701_3>

[13] Larson, K., & Czerwinski, M. (1998). Web page design: Implications of memory, structure and scent for information retrieval. In *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems* (pp. 25-32). ACM. <https://doi.org/10.1145/274644.274649>

[14] Pirolli, P., & Card, S. (1999). Information foraging. *Psychological Review*, *106*(4), 643-675. <https://doi.org/10.1037/0033-295X.106.4.643>

[15] Miller, G. A. (1956). The magical number seven, plus or minus two: Some limits on our capacity for processing information. *Psychological Review*, *63*(2), 81-97. <https://doi.org/10.1037/h0043158>

[16] Johnson, E. J., & Goldstein, D. (2003). Do defaults save lives? *Science*, *302*(5649), 1338-1339. <https://doi.org/10.1126/science.1091721>
