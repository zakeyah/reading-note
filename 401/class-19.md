# AWS: Events

SQS (Simple Queue Service)

SQS is mainly used to decouple applications or integrate applications. Messages can be stored in SQS for short duration of time (max 14 days).

![](https://miro.medium.com/max/723/1*DRrTtdyah9NHwR0VCm6MWA.png)


## SNS (Simple Notification Service)

SNS distributes several copies of message to several subscribers. 

![](https://miro.medium.com/max/1004/1*mdUPKzrfJFuXa4d43KhKUQ.png)




## Key Differences:
### Entity Type
- SQS : Queue (Similar to JMS).
- SNS : Topic (Pub/Sub system).
### Message consumption
- SQS : Pull Mechanism — Consumers poll and pull messages from SQS.
- SNS : Push Mechanism — SNS Pushes messages to consumers.
### Persistence
- SQS : Messages are persisted for some (configurable) duration is no consumer available.
- SNS : No persistence. Whichever consumer is present at the time of message arrival, get the message and the message is deleted. If no consumers available then the message is lost.
In SQS the message delivery is guaranteed but in SNS it is not.
### Consumer Type
- SQS : All the consumers are supposed to be identical and hence process the messages in exact same way.
- SNS : All the consumers are (supposed to be) processing the messages in different ways.
### Sample applications
- SQS : Jobs framework. Where the Jobs are submitted to SQS and the consumers at the other end can process the jobs asynchronously. And if the job frequency increases then the number of consumers can be increased for parallel processing.
- SNS : Image processing. If someone uploads an image to S3 then watermark that image, create a thumbnail and also send a ThankYou email. In that case S3 can send notification to SNS Topic and 3 consumers can be attached to SNS topic. 1st one watermarks the image, 2nd one creates a thumbnail and the 3rd one send a ThankYou email. All of them receiving the same message (image URL) and doing their corresponding processing in parallel.