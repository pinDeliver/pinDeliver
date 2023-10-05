# Terminology
This terminology list provides an overview of common terms that are essential to understand when learning about pinDeliver.

**Customer order**
A term used to refer to a delivery or a pickup. It is used for the sake of brevity instead of explicitly mentioning "Delivery" or "Pickup" every time.

**Dynamic pickups and deliveries**
This term is used when planning a route that involves picking up items from one or more locations and then delivering them to one or more destinations. The pickups are scheduled based on the optimal route calculated by the system.

**Open end**
When a vehicle does not have a specified end address, the route is considered to have an "open end". In this case, the time required to travel from the last stop to the location where the vehicle needs to be parked is not included in the route optimization process.

**Pickup identifier**  
A unique value used to establish a connection between a pickup and one or more deliveries, or vice versa. It helps to ensure the proper association and tracking of related orders.

**Stop time**  
The estimated duration, in minutes, for a stop at a customer's location to perform a delivery and/or pickup. It helps in calculating the overall time required for a route and optimizing the scheduling process.

**Stop type**  
This attribute specifies whether a customer order is a delivery or a pickup. In the case of connected pickups and deliveries, they must have corresponding pickup identifiers.

**Time window**  
An interval between two specific times during which a delivery is allowed to be made. It helps in managing the scheduling of deliveries within specific time constraints.

**Vehicle tag**  
A value often used as a property or definition for a vehicle. Customer orders can only be planned on a vehicle that has a matching tag. Common examples of vehicle tags include "cold", "freeze", etc.
