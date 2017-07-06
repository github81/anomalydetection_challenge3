

###Optional Input Data
Minimum number of users (-N) - to be provided as a command line parameter in the following way:

python ./src/process_log.py ./log_input/batch_log.json ./log_input/stream_log.json ./log_output/flagged_purchases.json -N 50

If provided the program will consider at least N (minimum number of) users in the User's network to find out if the purchase in question is anomalous or not. The script will first scan for the users (friends) in the provided degree of network of a particular user. If the number of users scanned is less than the minimum number of users provided then the script will consider the next degree in the network until minimum number of users are scanned.


