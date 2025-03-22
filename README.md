# 🔥 How to uncover hidden bias in dating apps: Using Data Analysis in Python to improve inclusivity (A Tinder-inspired case study)

This project investigates how implicit biases and personality traits influence dating decisions, using real-world speed dating data in a fictional case study inspired by Tinder. Through Exploratory Data Analysis (EDA) and statistical hypothesis testing in Python, it demonstrates skills in data cleaning, visualisation, statistical interpretation, and delivering actionable, business-focused insights.

---

## 🚩 Context: Falling matches and hidden biases

Online dating apps like Tinder thrive on connecting people, but globally declining match rates have raised concerns about user satisfaction. Are hidden social biases - such as those related to race, religion, or income - quietly affecting user engagement?

To explore this critical question, I conducted a data analysis inspired by Tinder's matchmaking process, using a real-world speed dating dataset from an academic study by Columbia Business School professors Ray Fisman and Sheena Iyengar.

---

## 🎯 Project objectives:

This project aims to:

- Detect hidden social biases influencing dating decisions.
- Understand what really drives successful matches: personality, demographics, or deeper compatibility.
- Provide clear, actionable insights for dating apps seeking to improve fairness, inclusivity, and overall user satisfaction.

---

## 🔍 Data and methods

I analysed a robust dataset gathered from speed dating events involving **8,378 interactions**. Participants provided demographic details, rated their partners across attributes such as attractiveness, fun, ambition, and shared interests, and indicated whether they wanted a second date.

### Dataset overview:

- **Demographics:** Age, race, income, education level
- **Ratings:** Attractiveness, sincerity, intelligence, fun, ambition, shared interests
- **Match decisions:** Mutual decisions to pursue a second date

The analysis included **exploratory data analysis (EDA)**, **statistical hypothesis testing** (Kruskal-Wallis tests), and clear **visualisations** using Python libraries like **Pandas, NumPy, Seaborn, Plotly,** and **SciPy**.

[🔗 Original Dataset and Documentation](http://www.stat.columbia.edu/~gelman/arm/examples/speed.dating/)

---

## 💡 Key insights: What drives matches, and what holds them back?

This analysis uncovered three important insights into modern dating dynamics:

1. **Hidden biases subtly shape dating outcomes**  
   Statistical analysis (Kruskal-Wallis, p < 0.0001) revealed significant racial disparities in match rates, highlighting how implicit biases quietly influence romantic choices.

   ![Match rates by racial group and gender](placeholder_path)

2. **Meaningful connections are driven by personality and compatibility**  
   Despite biases, the strongest predictors of match success were genuine personal attributes: being perceived as **fun**, physically attractive, and sharing common interests.

   ![Factors correlating with match success](placeholder_path)

3. **Successful matches positively reinforce confidence**  
   Participants receiving more matches showed notably increased confidence, highlighting the deeper psychological benefits of inclusive, compatibility-driven matchmaking.

   ![Confidence levels before and after speed dating](placeholder_path)

---

## 🚀 Actionable recommendations for dating apps

To tackle biases and improve user experiences, I propose clear, actionable steps inspired by this analysis:

- **Minimise collection of sensitive demographic data** to reduce potential algorithmic bias.
- **Encourage users to explicitly focus on compatibility and personality** through UX/UI nudges.
- **Enforce strict anti-discrimination guidelines** for user profiles.
- **Increase algorithmic transparency** and give users more control over their matchmaking preferences.
- **Continuously monitor long-term outcomes** to address hidden biases and ensure genuinely meaningful connections.

---

## 🔮 Suggestions for future improvement

To deepen the analysis and better tackle biases, future studies could:

- Conduct **qualitative research** (interviews/focus groups) to explore user dissatisfaction.
- Obtain more **representative data** inclusive of LGBTQIA+ participants and individuals from more diverse backgrounds beyond the university context.
- Track **long-term relationship outcomes** beyond initial matches.
- Test **UX interventions aimed at improving confidence and satisfaction** among users impacted by biases.

---

## ⚠️ Disclaimer & ethics

This analysis is a fictional, educational business scenario inspired by Tinder but uses a real dataset from academic research. It operates under ethical standards ensuring participant anonymity and compliance with GDPR, UK-GDPR, and CCPA regulations.

Note: Such analysis would be suitable in contexts like the US or UK, where collecting demographic data on race and religion is permissible to improve Diversity, Equity, and Inclusion (DEI). In contexts like France, where such data collection is restricted, analysis would rely on non-sensitive attributes.

---

## 🛠️ Technology stack

- **Python**: Pandas, NumPy, Seaborn, Plotly, SciPy
- **Statistical Testing**: Kruskal-Wallis non-parametric tests
- **Visualisation**: Seaborn, Plotly

---

## 🎓 About the Analyst

- **Ned Chambers**
- Data Analyst  
- [LinkedIn](https://www.linkedin.com/in/nedchambers/) | [GitHub](https://github.com/ned-chambers)
