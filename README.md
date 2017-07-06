###Input Data

Ideally, the input data would come from a real-time, streaming API, but we don't want this challenge to focus on the relatively uninteresting task of connecting to an API.

As a result, you may assume that the purchases and social network events have already been collected in two logs (in the log_input directory), which we can replay to mimic the data stream.

The first file, batch_log.json, contains past data that should be used to build the initial state of the entire user network, as well as the purchase history of the users.

Data in the second file, stream_log.json, should be used to determine whether a purchase is anomalous. If a purchase is flagged as anomalous, it should be logged in the flagged_purchases.json file. As events come in, both the social network and the purchase history of users should get updated.

The first line of batch_log.json contains a JSON object with the parameters: degree (D) and number of tracked purchases (T) to consider for the calculation.

###Optional Input Data
Minimum number of users (-N) - to be provided as a command line parameter in the following way
If 
