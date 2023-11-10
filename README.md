# Toxicity Assessment API Evaluation

## Hypothesis
The hypothesis of this project is that the Perspective API, specifically designed for assessing the toxicity of comments, will be ineffective at evaluating comments in which users have intentionally circumvented language filters through word substitution.

## Method
The methodology involves testing the API with sets of toxic and non-toxic statements, both in their original form and with substitutions replaced with the intended words. The goal is to analyze the API's accuracy in identifying toxicity in different linguistic contexts.

## Code Overview
The code utilizes the Google Perspective API (commentanalyzer) to assess toxicity scores for a set of statements. The statements include both direct and indirect toxic language, as well as non-toxic statements. The results are then analyzed to evaluate the accuracy of the API in different scenarios.

## Results
The evaluation indicates that the API's assessments for toxic statements are less accurate when circumventive language is used, while assessments for non-toxic statements are more accurate. The API seems to indiscriminately perceive indirect statements as less toxic overall, rather than accurately classifying them as toxic or non-toxic.

## Reflection
The findings suggest that the API may lack the ability to consider context effectively, relying more on individual words to determine toxicity. The API's focus on specific words without considering their context could lead to false positives and negatives. The low accuracy in assessing direct non-toxic statements indicates a potential limitation in the API's contextual understanding.

## Future Considerations
The project raises questions about the feasibility of training machine learning algorithms to better understand human context and subtleties in language. Further exploration could involve investigating methods to enhance the API's ability to interpret context accurately.

---

**API Used:** Perspective API (commentanalyzer) by Google Jigsaw

**Python Libraries:** googleapiclient

**API Key:** Replace 'API_KEY' in the code with your valid API key for authentication.

---

Feel free to explore the code and contribute to further discussions on the effectiveness of toxicity assessment in natural language processing.

