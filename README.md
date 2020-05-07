# tail2kafka 

## Overview
tail2kafka is a linux tool for sending log lines into a kafka topic.

It supports local and remote kafka servers, log rotation and batching messages to kafka.

Great thanks to Daniel Sully's pykafka (https://github.com/dsully/pykafka).

## Contact
Any feedback/suggestions/complaints regarding this tool would be much appreciated. Contributions are most welcome as well, of course.

Harel Ben-Attia, harelba@gmail.com, @harelba on Twitter


## Fork
use Kafka library ... https://towardsdatascience.com/kafka-python-explained-in-10-lines-of-code-800e3e07dad1

pip install kafka-python

To run

python ./tail2kafka/tail2kafka -l /Users/mminns/projects/stash.atlassian.com/jiraserver/jira-wt/atlassian_jira_8_8_branch/jirahome-clustered/**/log/audit/ -t atlassian-jira-audit -s localhost -p 9092

NB.
./tail2kafka/tail2kafka -l /Users/mminns/projects/stash.atlassian.com/jiraserver/jira-wt/atlassian_jira_8_8_branch/jirahome-clustered/**/log/audit/ -t atlassian-jira-audit -s localhost -p 9092

throws 
Traceback (most recent call last):
  File "./tail2kafka/tail2kafka", line 5, in <module>
    from kafka import KafkaProducer
ImportError: No module named kafka

but 

python ./tail2kafka/tail2kafka -l ....

works ??????
