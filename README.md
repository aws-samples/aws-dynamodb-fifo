# Implement serverless FIFO queues with filtering capabilities using Amazon DynamoDB transactions


## Setup instructions
* `git clone git@github.com:aws-samples/aws-dynamodb-fifo.git`  Clone repository
* `cd aws-dynamodb-fifo`   change directory
* `pip install -r requirements.txt`   Install dependent packages

## Create DynamoDB Agent Queue
`python createTable.py`

## Initialize table with agents and queue metadata
`python initializeAgentPoolAndQueueMetaData.py`

## Assign available agents to queue (adding agents to Agent Queue)
`python addAvailAgentsToQueue.py`

## Assign agents to callers
To find the first agent who speaks French and has a male gender.
`python assignAgentToCallRequest.py Q#French#M`

## Cleanup
`python deleteTable.py`
