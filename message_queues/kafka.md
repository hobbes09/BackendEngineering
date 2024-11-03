# Kafka



Originally developed in LinkedIn during 2011, Apache Kafka is one of the most popular open-source Apache projects out there. So far it has had a total of 24 notable releases and most intriguingly, its code base has grown at an average rate of 24% throughout each of those releases.

Kafka is a distributed streaming platform serving as the internet’s de-facto standard for real-time data streaming.

Its development is path-dependent on the problems LinkedIn hit at the time. As they were one of the first companies to hit large scale distributed systems problems, they noticed the common problem of uncontrolled microservice proliferation:

![](https://lh7-us.googleusercontent.com/Zfsoz8lj4ftWa8N7t_0Zntof1skFW7l2jE2fejY3PixDz905PVwJvAmQ98mYvdA1xiWfm9XY5Yc5B0Gh0y-d8xiDCV4mEegvyrDXVKsxfJvrkbjM4u1nqlFTfT4xRLxLW9apTsbwWdTbUOFl9OicTRI)

To fix the growing complexity of service-to-service and persistence store permutations, they opted to develop a single platform which can serve as the source of truth.

![](https://lh7-us.googleusercontent.com/rmJNLP33hKiT7VX_J66qxdDJxFkjF9lmRT19t1calefx1c5yr2LX9YHCEYQe4b-HSvOL2GbRDRwrjhENC5AhppIex_ADIgWVBmY5123OUeZadE4DLcxPNZr5wgSXhmEdNuwXB4UA5TwEJ8EWXKTqrgo)

Apache Kafka is a distributed system that was meant to solve the service coordination problem. Its vision is to be used as the central nervous system inside a company - somewhere where data goes, is processed/transformed and is consumed by other downstream systems (data warehouses, indices, microservices, etc.).

Therefore, it is optimized for accommodating large throughput (millions of messages a second) while storing a lot of data (terabytes)
