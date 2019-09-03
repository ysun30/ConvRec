# ConvRec

### A Conversational Recommendation Dialogue Dataset

Have dialogues between a user and a dialogue agent discussing facets of a target item rated by this user. The rating information is from the MovieLens1M dataset and the Yelp Challenge dataset. Dialogues are randomly simulated based on templates collected from crowdsourcing tasks. The dataset is used to train Natural Language Understanding models and models for making recommendations in dialogues.

- The movie dataset contains 999,458 dialogues, 6040 users, 3412 items, and 15 facets.
- The restaurant dataset contains 875,721 dialogues, 62047 users, 21350 items, and 23 facets.
- A facet is an attribute-value pair of an item, e.g., "genre=Drama"

### Dialogue Example:

    <ID>    834     2633    3.0
    <User>  i would like a Romance movie with a rating between 7.0 to 8.0.  ["genre__Romance", "rating__7.0-8.0"]
    <Agent> who are you favourite director? []
    <User>  it is from any director.        ["director__-1"]
    <Agent> which year range would you like to watch        []
    <User>  a movie before 80s      ["year__before 80s"]
    <Agent> how many reviews would you like the movie to have       []
    <User>  i like review of movie less than 50000  ["num_review__0-50000"]
    <Agent> which language would you like?  []
    <User>  in the English language ["language__English"]
    <Agent> how long would you like the movie to be?        []
    <User>  I want the duration to be less than 60 minutes  ["duration__0-60"]
    <Agent> which actor do you like?        []
    <User>  I'm not sure    ["actor__-1"]

- The user id is 834, the item id is 2633, and the rating is 3.0 (in a 1 to 5 scale)
- Labels are given in a json string following each utterance


### Reference:

*Please cite one or both of the following if you use the data in any way*

Sun, Yueming. Recommendation in Dialogue Systems. Diss. UC Santa Cruz, 2019.

Sun, Y. and Zhang, Y., 2018, June. Conversational recommender system. In The 41st International ACM SIGIR Conference on Research & Development in Information Retrieval (pp. 235-244). ACM.
