# Toxicity Assessment API Evaluation

## Overview
This project aims to evaluate the effectiveness of Google Jigsaw's Perspective API in assessing the toxicity of comments, especially when users purposefully circumvent language filters through word substitution. The evaluation includes both direct and indirect toxic statements, comparing the API's accuracy in different contexts.

## Hypothesis
The hypothesis suggests that the API will be ineffective at assessing the toxicity of comments in which users have purposely circumvented language filters through word substitution.

## Method
To test the hypothesis, the following steps were taken:
1. Creation of 10 toxic and 10 non-toxic statements with circumventive language.
2. Replacement of circumventive language with the intended words to create a parallel set of statements.
3. Utilization of Google Jigsaw's Perspective API to assess the toxicity of both sets of statements.
4. Calculation of accuracy for direct toxic, direct non-toxic, indirect toxic, and indirect non-toxic statements.

## Results
The obtained results indicate:
- Indirect Toxic Accuracy: 70%
- Indirect Non-Toxic Accuracy: 90%
- Direct Toxic Accuracy: 100%
- Direct Non-Toxic Accuracy: 60%

## Conclusion
The results support the hypothesis, showing that the API's assessments were 30% less accurate for toxic statements when circumventive language was used. However, non-toxic statements were assessed 30% more accurately with circumventive language. The API seemed to indiscriminately perceive indirect statements as less toxic overall, lacking the ability to accurately flag them as toxic or non-toxic.

The surprising finding was the API's lower accuracy (60%) in assessing direct non-toxic statements, possibly indicating a reliance on specific words rather than considering contextual nuances. The theory suggests that the API may struggle with context and might be easily fooled when users employ circumventive language that obscures profanity.

## Future Considerations
A key question for future exploration is whether it's possible to enhance the API's understanding of human context and subtle language nuances. Further research could investigate methods to teach the algorithm to recognize context, improving its accuracy in assessing the true toxicity of statements.

## Files
- `toxicity_assessment.py`: Python script for conducting the evaluation.
- `api_data_results.csv`: CSV file containing the results of the API assessments.
- `README.md`: This file providing an overview of the project, the hypothesis, method, results, conclusion, and future considerations.
