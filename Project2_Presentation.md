# Project 2: Predicting Injury Risk in University Football Players
## A Data-Driven Approach to Athlete Health

**Tarun Vigneswaran**  
**DSC 101 | Dr. Rimal | April 1, 2026**

---

## Slide 1: Dataset Background

### University Football Injury Prediction Dataset

- **Source**: Kaggle dataset from Scientific Reports (2025)
- **Population**: 800 Chinese university football players
- **Data Collection**: Systematic monitoring across multiple institutions
- **Purpose**: Identify factors associated with injury risk in competitive athletes

### Why This Matters
- Sports injuries affect player health, team performance, and athletic careers
- Understanding risk factors enables targeted prevention strategies
- Data-driven approaches can optimize training and improve athlete welfare

---

## Slide 2: Project Goal

### Research Question
**Which training, fitness, and lifestyle factors are most strongly associated with injury risk in university football players?**

### Supporting Questions
- Do injured players show different stress and sleep patterns?
- Does previous injury history increase future injury risk?
- Which playing positions have the highest injury rates?
- Can modifiable factors be identified for prevention programs?

---

## Slide 3: Data Overview

### Dataset Characteristics
- **800 observations** (individual players)
- **19 variables** across four domains
- **Binary target**: Injury in next season (0 = no, 1 = yes)
- **No missing values** - high quality dataset

### Variable Categories
1. **Basic Information**: Age, height, weight, BMI, position
2. **Training Factors**: Training hours, matches played, previous injuries
3. **Physical Fitness**: Knee strength, flexibility, reaction time, balance, sprint speed, agility
4. **Lifestyle Habits**: Sleep hours, stress level, nutrition quality, warmup adherence

---

## Slide 4: Data Cleaning & Preprocessing

### Cleaning Process
- ✅ **No duplicate records** found (800 unique players)
- ✅ **Zero missing values** across all variables
- ✅ **Data types standardized** (numeric and categorical)
- ✅ **Categorical encoding**: Playing position converted to numeric codes

### Outlier Handling
- **IQR method** applied to detect extreme values
- Outliers **capped at boundaries** (Q1 - 1.5×IQR to Q3 + 1.5×IQR)
- Preserved all observations while reducing extreme value influence
- Final dataset: **800 clean observations ready for analysis**

---

## Slide 5: Key Finding 1 - Balanced Injury Distribution

### Injury Outcome Distribution
- **~50% injury rate** across the cohort
- Balanced dataset ideal for identifying risk factors
- Confirms injury is a common concern in this population

### Injury Rates by Playing Position
- **Forwards & Midfielders**: Higher injury rates
- **Defenders & Goalkeepers**: Lower injury rates
- Pattern reflects higher intensity and contact in offensive positions
- **Implication**: Position-specific prevention strategies needed

---

## Slide 6: Key Finding 2 - Lifestyle Factors Matter

### Stress and Sleep Patterns
- **Injured players** show:
  - Higher stress levels (median ~50 vs. 45)
  - Fewer sleep hours (median ~7.5 vs. 8 hours)
  - Negative correlation between stress and sleep

### Key Insight
- High stress disrupts sleep quality
- Inadequate sleep reduces stress resilience
- **Synergistic effect** increases injury vulnerability
- Both factors are **modifiable** through interventions

---

## Slide 7: Key Finding 3 - Previous Injury History

### Strong Predictor of Future Risk
- Injured players: **Median 2 prior injuries**
- Non-injured players: **Median 1 prior injury**
- Clear dose-response relationship

### Possible Explanations
- Incomplete recovery from previous injuries
- Biomechanical compensations during rehabilitation
- Underlying individual susceptibility factors
- **Implication**: Enhanced monitoring for players with injury history

---

## Slide 8: Physical Fitness & Training Patterns

### Balance and Proprioception
- **Lower balance scores** in injured players
- Neuromuscular control plays protective role
- Balance training may reduce injury risk

### Training Load Variability
- Similar median training hours between groups
- **Greater variability** in injured players
- Inconsistent training patterns more problematic than absolute volume
- Warmup adherence shows **clear protective effect**

---

## Slide 9: Correlation Analysis

### Strongest Associations with Injury Risk

**Positive Correlations** (increase risk):
- Previous injury count
- Stress level score
- Training hours variability

**Negative Correlations** (protective):
- Sleep hours per night
- Balance test scores
- Warmup routine adherence

### Multi-Factor Interactions
- High stress + Low sleep = Elevated risk
- High training load + Previous injuries = Compounded risk

---

## Slide 10: Main Insights Summary

### Critical Risk Factors Identified
1. **Lifestyle**: High stress and inadequate sleep
2. **History**: Previous injury count strongly predictive
3. **Physical**: Lower balance and proprioceptive ability
4. **Behavioral**: Inconsistent training and poor warmup adherence
5. **Positional**: Forwards and midfielders at higher risk

### Why These Findings Matter
- Most factors are **modifiable** through targeted interventions
- Evidence-based prevention strategies can be developed
- Holistic approach needed addressing multiple risk domains
- Early identification enables proactive athlete support

---

## Slide 11: Value to Stakeholders

### Athletic Programs
- Reduce injury rates and healthcare costs
- Maintain team performance and competitive success
- Improve athlete retention and satisfaction

### Coaches & Trainers
- Implement position-specific training protocols
- Monitor player stress and recovery patterns
- Identify high-risk athletes for targeted support

### Athletes
- Empowerment through modifiable risk factors
- Better understanding of injury prevention
- Long-term health and career protection

### Society
- Reduced healthcare costs
- Promotion of evidence-based sports medicine
- Culture of athlete welfare and health awareness

---

## Slide 12: Ethical Considerations

### Privacy & Data Security
- Athlete health data is highly sensitive
- Robust security measures required
- Strict access controls essential

### Fairness & Equity
- Avoid stigmatization of "high-risk" players
- Ensure equitable access to prevention resources
- Predictions should inform support, not punishment

### Responsible Implementation
- Avoid over-reliance on predictive models
- Maintain human judgment in medical decisions
- Transparent communication with athletes
- Informed consent for data use

---

## Slide 13: Limitations

### Dataset Constraints
- **Population**: Chinese university players only
- **Generalizability**: May not apply to other contexts
- **Sample size**: 800 players (may miss rare patterns)
- **Timeframe**: Single season (cross-sectional)

### Measurement Limitations
- Self-reported data (stress, sleep) subject to bias
- Binary injury outcome (no severity information)
- No injury type or mechanism details
- Limited causal inference from observational data

### Need for Validation
- Longitudinal studies required
- Intervention trials needed
- Diverse populations should be studied

---

## Slide 14: Next Steps & Future Research

### Immediate Actions
1. **Intervention programs**: Test stress management and sleep optimization
2. **Enhanced monitoring**: Track high-risk players more closely
3. **Warmup protocols**: Standardize and enforce proper preparation
4. **Balance training**: Incorporate proprioceptive exercises

### Future Research Directions
- **Longitudinal studies** across multiple seasons
- **Intervention trials** to establish causality
- **Diverse populations** for generalizability
- **Machine learning models** for personalized risk assessment
- **Implementation research** on translating findings to practice

### Collaborative Approach
- Data scientists + Sports medicine professionals
- Coaches + Athletes + Researchers
- Evidence-based, athlete-centered prevention programs

---

## Slide 15: Conclusion

### Project Achievements
✅ Identified key modifiable risk factors  
✅ Demonstrated multifactorial nature of injury risk  
✅ Provided evidence-based insights for prevention  
✅ Highlighted ethical considerations for implementation

### Take-Home Message
**Injury prevention requires a holistic approach addressing training, physical fitness, and lifestyle factors. By focusing on modifiable risk factors—particularly stress management, sleep optimization, and consistent training patterns—sports programs can protect athlete health while supporting performance excellence.**

### Questions?

---

## References

1. Kaggle dataset: https://www.kaggle.com/datasets/yuanchunhong/university-football-injury-prediction-dataset

2. Ma, J., Liu, S., & Pei, Y. (2025). *SHAP-based interpretable machine learning for injury risk prediction in university football players: a multi-dimensional data analysis approach.* Scientific Reports. https://www.nature.com/articles/s41598-025-24144-y

---

## Presentation Tips

### Delivery Guidelines
- **Time**: 5-7 minutes for full presentation
- **Pace**: ~30 seconds per slide
- **Focus**: Emphasize strongest findings (slides 5-9)
- **Visuals**: Reference charts from notebook during presentation

### Key Points to Emphasize
1. Modifiable nature of key risk factors
2. Synergistic effects (stress + sleep)
3. Previous injury as strongest predictor
4. Practical applications for coaches and trainers
5. Ethical implementation considerations

### Backup Slides Available
- Detailed correlation heatmap
- Distribution histograms for all variables
- Scatterplot analyses
- Group comparison statistics
