# 🔥 Improving Tinder match rates and reducing racial bias: An Exploratory Data Analysis of Speed Dating data using Python

An in-depth analysis of Tinder Speed Dating data, exploring factors that influence successful matches. This project demonstrates Exploratory Data Analysis (EDA) skills in Python, including data cleaning, visualisation, interpretation, and reporting.

---

# **Executive summary**

Tinder is experiencing a global decrease in user matches, potentially exacerbated by underlying social biases. This exploratory analysis, conducted on data from controlled speed dating experiments, explores whether match rates are negatively impacted by racial bias, and whether mitigating these biases can lead to improved user engagement, increased satisfaction among users, and ultimately, greater retention on the platform.

The analysis reveals clear evidence of significant racial disparities in attractiveness perceptions and match rates. Certain racial groups experience disproportionately lower match rates compared to others of the same gender, likely due to biases in selection. Racial groups with lower match rates also reported lower levels of satisfaction with the dating process, suggesting that these groups may be at risk of attrition without further action to counter racial biases.

However, race itself is only weakly correlated with match success, suggesting that other factors play a larger role. Notably, the factors most strongly correlated with match success were a sense of fun, attractiveness, and shared interests. Other personality attributes, such as intelligence, sincerity and ambition, all contributed considerably more to match success than demographic attributes such as race, age or income.

It was also observed that groups with higher match rates tended to report increased levels of confidence post-event.

These insights provide an opportunity for Tinder to increase overall match rates and platform satisfaction by counteracting racial biases and fostering inclusivity. To achieve this, we recommend:

1. Avoiding collection and use of sensitive demographic data such as race
2. Shifting user focus towards compatibility, personal qualities and shared interest through UX/UI design
3. Enforcing a ban on explicitly stating a preference for racial or racialised physical attributes on user profiles to minimise potential for discrimination and bias
4. Improving algorithmic transparency and user agency to allow users to understand how and why specific matches are recommended and foster trust in the product
5. Minimising bias from image recognition algorithms
6. Tracking long-term outcomes alongside shorter-term metrics to provide better-quality matches

Such steps will enhance user inclusivity, satisfaction, and engagement, directly addressing the core business challenge of declining matches - and, in turn, boosting user engagement and revenue.

---

# **1. Project**

## 1.1 Disclaimers

### 1. Fictional business case:

This project is based on a fictional business case designed to simulate a real-world analysis for Tinder. The dataset and analysis are adapted to provide a business-oriented context for educational purposes.

### 2. Context of analysis:

The analysis focuses on examining social biases in dating, including the influence of factors such as race, religion, and income on matches. This approach aligns with practices in contexts like the US and UK, where collecting and analysing data on race, religion, and ethnicity is permissible and often encouraged to monitor and improve Diversity, Equity, and Inclusion (DEI) initiatives.

However, this analysis would not be feasible in a French context due to legal restrictions prohibiting the collection of data related to race and religion. In France, a similar investigation into social biases would rely on other factors, such as income or education level.

The analysis presented in this project therefore assumes a UK/US legal and cultural context.

## 1.2 Case study context

Tinder, launched in 2012 by Sean Rad at a hackathon hosted by Hatch Labs in West Hollywood, is one of the world's leading online dating and geosocial networking platforms. As of 2025, Tinder has facilitated over 100 billion matches globally.

To better understand what drives interest and connections between users, Tinder has designed a speed dating experiment. Each participant in the experiment provides information that mimics their dating profile on the app, including demographics, self-perceptions, and lifestyle factors. Data from the experiment is used to investigate patterns and insights into what makes people agree to go on a second date.

## 1.3 Project goals

The marketing team at Tinder has observed a global decrease in the number of matches across the platform, raising concerns about user engagement and satisfaction, particularly among certain demographics. To address this issue, the marketing and Diversity, Equity, and Inclusion (DEI) teams propose the following hypotheses:

1. **Social Biases**: User preferences or prejudices—such as those based on race, religion, or income—may result in lower match rates for specific groups.
2. **Algorithmic Reinforcement of Biases**: The matching algorithm might inadvertently amplify these biases, exacerbating disparities and contributing to feelings of exclusion among users.

This project aims to:

- **Understand User Preferences**: Investigate how demographic and personal attributes influence decisions to go on a second date, using exploratory data analysis (EDA).
- **Identify Disparities**: Uncover patterns of unequal match rates or preferences across different demographic groups.
- **Provide Actionable Insights**: Recommend strategies for Tinder's marketing and DEI teams to address identified biases, enhance user experiences, improve match rates for underrepresented groups, and promote inclusivity on the platform.

These insights aim to help Tinder create a more equitable and engaging user experience while addressing the global decline in matches.

---

# **2. Dataset**

## 2.1 Source

The dataset used in this project originates from speed dating experiments conducted as part of an academic study by Columbia Business School professors Ray Fisman and Sheena Iyengar. The study aimed to explore decision-making in mate selection and the influence of various factors on dating outcomes.

Link to original dataset and data key: http://www.stat.columbia.edu/~gelman/arm/examples/speed.dating/

## 2.2 About the dataset

Data was gathered from participants in experimental speed dating events from 2002-2004. During the events, the attendees would have a four minute "first date" with every other participant of the opposite sex. At the end of their four minutes, participants were asked if they would like to see their date again. They were also asked to rate their date on six attributes: Attractiveness, Sincerity, Intelligence, Fun, Ambition, and Shared Interests.

The dataset contains detailed information about speed dating events, including:

- **Demographics**: Age, race, income, and education level of participants.
- **Ratings**: Participants evaluated their dates on attributes such as attractiveness, sincerity, intelligence, fun, ambition, and shared interests.
- **Match Decisions**: Indications of whether participants agreed to a second date with their partner.
- **Questionnaire Responses**: Data on participants’ self-perceptions, dating habits, and preferences.

## 2.3 Structure

The dataset contains 8378 rows and 195 columns.

- Each row represents one speed date between two individuals.
- A match is recorded when both participants agree to see each other again.

Key columns include:

- `gender`: Participant gender (1 = male, 0 = female).
- `age`: Age of the participant.
- `race`: Self-identified race of the participant.
- `goal`: Participant’s primary motivation for attending the event.
- `attr_o`: Rating of the partner’s attractiveness.
- `like_o`: Likelihood of liking the partner.
- `match`: Outcome of the date (1 = yes, 0 = no).

## 2.4 Ethics and compliance

The dataset has been checked to ensure it contains no personally identifiable information (PII), thus protecting participant privacy. This approach aligns with ethical research standards and complies with data protection regulations, including:

- The General Data Protection Regulation (GDPR) in the European Union.
- The UK General Data Protection Regulation (UK-GDPR) in the United Kingdom.
- The California Consumer Privacy Act (CCPA) in the United States.

By ensuring the absence of identifiable data, the dataset is exempt from these regulations, facilitating its ethical use for analysis in this project.

---
