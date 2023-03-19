# Guidelines

## Consider designing applications that are loosely coupled

Compute, network, storage, and many other technology components are delivered as services by AWS.

Think of your applicationas a consumer and provider of services. Design and develop your applicationas granular components (microservices) that can be delivered and scaled independently.

## Architect for resilience

Architect your application so that it can react gracefully and quickly to spikes in volume or unexpected failures.

Examples:
- You might set up your servers to scale automatically based on the number of users concurrently visiting your application. Automatic scaling would enable your application to handle a surge in volume during a sale or promotion and go back to normal operating levels when the sale is over.
- You could set up a cluster of nodes so that when one node fails, another node automatically picksup all the traffic.
- You might consider setting up read replicas for your database. This will shift read-heavy workloads away from your main database instance and provide better throughput for write operations.

## Design for failure

Services might become completely unavailable or might show increased latency if there is an unexpected surge in activity. Design applications to handle and survive failures.

In case of service failure, your application could log the failure and retry at a later time. If the service is slow to respond, your application could retry by using an exponential backoff algorithm: it will retry after increasing amounts of time between attempts. For example: it would retry after two seconds, then retry after four seconds and so on.

## Log metrics and monitor performance

Incorporate instrumentation in all your services, log usage metrics and failures, and monitor performance. Measuring, recording, and monitoring performance is critical to building a high-performance application.

## Implement a strong DevOps model

Develop a modular, automated, and continuous build process. Ensure consistency in the development, staging, and production environments. Set up scripts or use robust tools to consistently configure your environments.

## Be aware of security and regulatory restrictions

These restrictions can impact the design and implementation of your application and restrict where sensitive data can be stored. You might not be able to use certain services if they are not available in a specific Region. Regulatory restrictions might prevent you from using the service in a different Region.

Examples of security and regulatory restrictions:
- The Federal Information Processing Standard (FIPS) specifies the security requirements for cryptographic modules that protect sensitive information.
- The Health Insurance Portability and Accountability Act (HIPPA) includes provisions to protect the security and privacy of Protected Health Information (PHI). PHI includes a very wide set of personally identifiable health-related data like insurance and billing information, diagnosis data, clinical care data, and lab results such as images and test results.
- The EU Data Protection Directive refers to the directive on the protection of individuals with regard to the processing of personal data and on the free movement of this data.

## Implement security in every layer

Make sure that you implement security in the infrastructure, in the application, for data in transit and at rest, and for user authentication and authorization.
