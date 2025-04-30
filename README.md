# Gilbert Kristian - 2306274951 - Adpro A
### Publisher Questions

a. How many data will your publisher program send to the message broker in one run?

   In reference to the program, the publisher will send 5 pieces of data in a single execution. These data represent user IDs ranging from 1 to 5, each with a unique name.

b. The URL of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

   This indicates that the RabbitMQ server, which is connected using the AMQP protocol in the subscriber program, is also being used by the publisher program (the same server). As a result, the interaction between these two programs can be observed as a unified system.

## Running RabbitMQ as message broker
![RabbitMQ](ss/1.png)

### Console Screenshot when running `cargo run` Publisher 
![Console screenshot](ss/2.png)

When the publisher is executed, it sends 5 pieces of data to the RabbitMQ server. Since the subscriber is actively listening for activity on the RabbitMQ server, it detects the incoming data from the publisher. As a result, the subscriber displays the received data in the specified format.

### Message Rate Spike Photo

![Message ss](ss/3.png)

The graph represents the message rate. This graph calculates the rate of messages received per second. In the displayed example, the publisher program sends multiple messages over a short period, which results in a series of spikes on the graph. The higher spikes indicate periods with more messages being sent within a shorter time frame, while the lower ones represent quieter intervals. The varying message rate is visualized through these fluctuations in the graph.
