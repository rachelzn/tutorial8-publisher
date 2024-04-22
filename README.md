*REFLECTION*

a. How many data your publisher program will send to the message broker in one run?

    The publisher program's is going to toss five bits of data (messages) to the message hub in a single run. We can see it from the five times it shouts out "publish_event" inside the main function, but each one's got different data.

b. The url of: `amqp://guest:guest@localhost:5672` is the same as in the subscriber program, what does it mean?

    It means both the publisher and subscriber programs are using the same setup to connect to the AMQP server.

    - amqp:// tells us the protocol being used, which is AMQP.
    - guest:guest is the default login info being used. In this context, "guest" is the username, and "guest" is the password.
    - localhost:5672 is the host address and port being used to connect to the AMQP server. In this case, it's connecting to the same machine  (localhost) on the standard AMQP port (5672).