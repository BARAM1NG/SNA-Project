# SNA-Project

## Introduction

The expansion of KBO League’s digital platforms, particularly through YouTube, has strengthened interactions and a sense of belonging among fan communities. In 2024, the KBO League surpassed 9 million spectators and demonstrated vibrant fan activities online. The Korean Series between the KIA Tigers and SAMSUNG Lions offers an ideal case for exploring fandom interactions and digital network structures. This study analyzes YouTube comment networks from the two teams to examine the impact of sports fandom digitalization and the phenomenon of filter bubbles.

## Main Body

### 1. Research Methods and Data

- Subjects of Analysis
  - The study focuses on videos and comments uploaded to the official YouTube channels of the Kia Tigers and Samsung Lions during the 2024 KBO League Korean Series.

- Data Collection
  - Comments were collected using the YouTube V3 API. Relationships between commenters and videos were defined as nodes and edges to construct a commenter-video network.
    - OpenAI's model was employed for sentiment analysis to identify fan affiliations based on comment content.
    - To quantify interactions between fandoms, commenters' activities were aggregated to determine their primary team affiliation.

- Analysis Methods
  - Homophily Analysis: Network density and homophily metrics were examined to assess intra-fandom cohesion.
  - Modularity Analysis: The modularity of the network was analyzed to measure community structure and segmentation.
  - Temporal Network Analysis: The data was divided into the Korean Series period and the post-series period to observe network changes over time.

### 2. Analysis Results

- Fandom Network Characteristics
  - Both fandoms exhibited strong internal cohesion, with limited direct interaction between fans of opposing teams.
  - Filter bubble phenomena were evident, with minimal cross-fandom exchanges.

- Homophily Changes
  - During the Korean Series, inter-fandom interactions showed low homophily (0.0005), indicating restricted exchanges between fanbases.
  - Post-series, internal cohesion within each fandom increased (KIA: 0.285, SAMSUNG: 0.470), while inter-fandom homophily declined further (0.0003).

| Period           | Among Kia Fans | Among Samsung Fans | Between Kia and Samsung Fans |
|------------------|----------------|--------------------|------------------------------|
| Before Korean Series End | 0.163         | 0.304             | 0.0005                       |
| After Korean Series End  | **0.285**     | **0.470**         | **0.0003**                   |



- Community Analysis
  - Communities were primarily centered on individual team fandoms, forming distinct, independent groups.
  - Using the Louvain method, modularity scores ranged between 0.5 and 0.6, reflecting strongly cohesive internal communities.
  - Echo chamber effects were prominent within each fandom, with negligible interactions across teams.
 
| Period                              | Modularity |
|-------------------------------------|------------|
| Game 1: 2024.10.19~2024.10.21 | 0.5439     |
| Game 1 & Game 2: 2024.10.19~2024.10.23 | 0.5614     |
| Game 3: 2024.10.19~2024.10.25       | 0.5656     |
| Game 4: 2024.10.19~2024.10.26       | 0.5647     |
| Game 5: 2024.10.19~2024.10.28       | 0.5493     |
| Post-Series Period 1: 2024.10.29~2024.10.31 | 0.4998     |
| Post-Series Period 2: 2024.10.29~2024.11.01 | 0.5621     |
| Post-Series Period 3: 2024.10.29~2024.11.02 | 0.5500     |
| Post-Series Period 4: 2024.10.29~2024.11.03 | 0.5560     |
| Post-Series Period 5: 2024.10.29~2024.11.04 | 0.5530     |

- Temporal Network Changes:
  - During the Korean Series (October 19–28), comment activity intensified as the series progressed, with a dramatic spike in Kia’s channel activity following their championship win.
  - Post-series, activity declined, and network density gradually decreased.
  - Korean Series Period (2024.10.19~2024.10.28)
    ![image](https://github.com/user-attachments/assets/59a4392a-1176-4cf3-9f53-9b3412dc8e09)
  - Post-Korean Series Period (2024.10.29~2024.11.04)
    ![image](https://github.com/user-attachments/assets/25d8b3ba-53c3-458e-9ff6-5c656b164f55)


### 3. Discussion
- This study highlights the dual nature of YouTube comment networks, where filter bubble structures enhance intra-fandom cohesion while limiting cross-fandom interactions.
- Even after the Korean Series, both Kia and Samsung fanbases maintained independent communities, emphasizing how team-centric identities shape fandom culture on digital platforms.

## Conclusion

This research demonstrates how digital platforms reinforce fandom culture through filter bubbles. The independent communities formed by Kia and Samsung fans indicate that the digitalization of sports fandom fosters cohesion within groups while reducing opportunities for cross-fandom interaction. Future studies should explore strategies to encourage positive interactions between fandoms across various platforms.
