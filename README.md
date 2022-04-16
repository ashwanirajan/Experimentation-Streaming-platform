# Hypothetical-Experimentation-on-Streaming-platform-to-minimize-browsing-time

Netflix is one of the most popular streaming platforms which provides the user with a plethora of viewing options. While the high number of viewing options provide users with a wide variety of options, it also comes with the curse of Decision Paralysis. This may lead a user to spend more time browsing among the options, only to be fatigued and ultimately lose interest and return without watching anything. The primary goal of this online controlled experiment is to minimize the average browsing time a Netflix user spends at the home screen of the website. An increase in browsing time may be due to several factors like suitability of the recommended content, varying interests of a user, and so on. However, for the case of this experiment, we chose to focus on four major factors which are hypothesized to influence the browsing time, i.e. Tile Size, Match Score, Preview Length, and Preview Type.
We begin by experimenting with different levels of these four factors to test which factors make a statistically significant influence on browsing time. We performed controlled experiments with these factors, starting with a 24 factorial test to check for the significance of each factor. This helped us eliminate Tile Size as an insignificant factor. We then performed a series of sequential factorial experiments using different conditions within our reduced search space. As a result, we concluded that the following levels produced the most optimal browsing time:
- Preview Type: Teaser/Trailer, Match Score: 75, Preview Length: 75 seconds
A minimum average browsing time of 9.84 minutes with a 95% Confidence Interval of (9.62, 10.07) was obtained for this optimal condition.

In this project, we aim to reduce the time Netflix users spend browsing the suggested content. This helps improve user engagement with the platform and addresses the issue of decision paralysis. We define the average browsing time as the Metric of Interest (MoI). The goal is to minimize our MOI through controlled experimentation on selected design factors.

The experiments were performed in a controlled environment with 100 responses for each experimental condition. Our initial goal was to check the importance of each factor. We performed a 24 factorial test with two levels for each factor sufficiently spaced apart. As part of the first step, we plotted the main effects and interaction effects of each factor. We performed partial F-tests to check for the significance of terms and pairwise t-tests to find the condition which minimizes the browsing time.
Then iterative experiments were performed to refine our search as we go along to find the optimum value of these factors for the MoI. Since we are comparing the mean browsing time, we deployed the appropriate t-tests (Student’s or Welch’s) based on the result of the F-test for variances. We used Bonferroni adjusted p-values to address the multiple comparison problem. We stopped this process once we could not improve the MoI further.
The next section provides a detailed description of each round of experiments and documents our reasoning for our experimental design for each round. We start by explaining the 2k factorial experiment and its conclusion. This is followed by the algorithmic workflow of the consequent rounds. Later we list down the results of each experiment round and our conclusion on the optimal condition.
