# Mercator Prototype

Mercator is a benchmark prototype that I will use as a proof-of-concept for my technical abilities.  The design is to make an MVC architecture with two interfaces: a provisioning interface and a real-time interface as gateways to access a data model.  

This prototype has several broad objectives, showcasing: 
Phase 1 
 * Test-Driven-Design (TDD)
 * SOLID architecture and design principles
 * Enabling a synchronous API 
Phase 2
 * Real-time-stream via Apache Kafka or RabbitMQ
 * Demonstrating security RBAC controls and Cross Site Scripting hardeningand
 * Showing plugin encryption of data in transit and data at rest, as well as binary bytestream
Phase 3
 * An example of a "cloud hosted app"
 * App finally implemented not as a "lab test bench" but as a full app
 * A basic Android mobile app that can act as the "view" that interacts with the API
 
This will be implemented in Python first, then in GO and benchmark tested.  
