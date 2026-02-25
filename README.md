Objective:
<br>
Online Gaming Behavior dataset consists of 40K+ records and this project aims to understand player engagement patterns, monetization gaps and genre based retention. A custom Engagement Score was calculated to segment players into tiers to identify metrics that determines player loyalty.

Data characteristics:
<br>
Upon analysis, this dataset exhibits synthetic characteristics including non-zero feature correlations and uniform distribution across genres. This report critiques these anomalies while extracting the logic of the engagement model.

Important attributes:
<br>
Gender: Male(60%), Female(40%)
Location: USA(40%), Europe(30%), Asia(20%), Other(10%)
Game Difficulty: Easy(50%), Medium(30%), Hard(20%)
Engagement Distribution: Medium(48%), High(26%), Low(26%)
Genres: near equal distribution (~20% each) across all genres (sports, action, strategy, simulation, RPG)

Insights & Tasks:
<br>
Task 1: Player Segmentation
Players were segmented into Low, Medium, and High groups. We found that engagement is primarily driven by session depth rather than session frequency.
High Engagement: ~162 mins/session
Medium Engagement: ~104 mins/session
Low Engagement: ~35 mins/session

Task 2: Feature Importance
<br>
By correlation analysis, it is identified that Average Session Duration is the dominant driver of engagement. Interestingly, in this dataset, In-Game Purchases and Player Level show near-zero correlation with engagement scores, contradicting real-world esports telemetry (where level and spending usually scale with playtime).

Task 3: Market Analysis (Monetization)
<br>
Analysis revealed a Monetization Paradox: Average purchases remain flat at ~20% across all segments. High-engagement players provide massive value in "time on screen" but are currently under-monetized relative to their commitment.

Task 4: Product Analysis
<br>
Retention rates increase from 55% (Low) to 63% (High).
High-engagement players prefer Strategy and Sports, suggesting a preference for skill-intensive loops.
Low-engagement players prefer Simulation, indicating a casual, low-commitment user base.

Task 5: Gaming KPI Analysis
<br>
The most striking metric is Average Session Duration, which surges from 34.69 minutes (Low) to 161.85 minutes (High), a +366% increase in time-on-screen per session. This immersion directly bolsters the Retention Rate, which climbs from 55.34% to 63.27%. While a +7.93% lift in retention may seem incremental, in gaming telemetry, this represents a critical reduction in churn and a significant boost to long-term player Lifetime Value (LTV).
Ultimately, moving a player from a casual to a hardcore profile results in a Total Engagement Lift of 143.47%. This proves that high-engagement users are fundamentally more invested in the ecosystem.

Recommendation:
<br>
Genre Graduation: Introduce "Hybrid" game designs (e.g., Simulation → Strategy elements) to migrate casual players into deeper engagement loops.

Monetization Pivot: Move away from flat "pay-to-win" models. High-engagement segments should be targeted with progression-based purchases (Cosmetics/Expansions), similar to the successful models used by Riot Games and Activision Blizzard.

Game Design: Since "Session Duration" is the strongest engagement anchor, focus on progression systems and challenges that encourage "extended play" rather than just "daily login" rewards.

Tools:
<br>
Python (Pandas, NumPy)
Visualization: Matplotlib, Seaborn
Statistics: Correlation Matrices, Quantile binning, segmentation

Conclusion:
<br>
This project demonstrates how behavioral analytics can guide player segmentation, monetization strategy, and game design decisions. Even with synthetic-like data, the engagement model reveals that immersive gameplay depth—not just play frequency drives retention and long-term player value. These insights can inform the development of recommendation engines that enhance both player satisfaction and business revenue in competitive gaming ecosystems.
