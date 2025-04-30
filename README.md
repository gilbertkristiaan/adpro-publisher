# Gilbert Kristian - 2306274951 - Adpro A
### Publisher Questions

a. How many data will your publisher program send to the message broker in one run?

   In reference to the program, the publisher will send 5 pieces of data in a single execution. These data represent user IDs ranging from 1 to 5, each with a unique name.

b. The URL of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

   This indicates that the RabbitMQ server, which is connected using the AMQP protocol in the subscriber program, is also being used by the publisher program (the same server). As a result, the interaction between these two programs can be observed as a unified system.
