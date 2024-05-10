# Requirements - 
- It should support multiple topics where message can be published
- Publisher should be able to publish a message to a particular topic
- Subscribers should be able to subscribe to a topic
- Whenever a message is published to a topic, all subscribers to that particular topic should receive messages
- Should be able to reset the offset for a subscriber . Subscribers should start receiving messages from that offset (Replaying the messages)
- Subscribers should be able to run in parallel


# Apis
- createTopic(topicName) -> topicId
- subscribe(topicId,subscriber) -> boolean
- publish(topicId,message) -> boolean
- readOffset(topicId, subscriber, offset) -> boolean
