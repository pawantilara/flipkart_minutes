# flipkart_minutes

### Flipkart Minutes — Real-Time Order & Delivery Assignment System

Built a **production-style backend simulation of Flipkart Minutes** using **Golang**, focusing on real-time order processing, delivery-partner assignment, concurrency, and failure handling.

The system models the complete order lifecycle — from order creation and partner assignment to delivery completion and automatic cancellation. It uses a modular **repository–service architecture** with dedicated components for **Order/Notification handling, Partner Management, Assignment, and Auto-Cancellation scheduling**.

Key engineering challenges addressed include:

* Designed a **concurrent partner-assignment workflow** to efficiently match delivery partners with incoming orders.
* Implemented **thread-safe state management** using Go concurrency primitives and synchronization mechanisms.
* Built an **Auto-Cancel Scheduler** to automatically cancel orders that remain unassigned beyond a configured timeout.
* Added **failure handling and state transitions** to prevent inconsistent order/partner states during concurrent operations.
* Designed the system with clear separation between **business logic, repositories, and background workers**, making components independently testable and extensible.
* Handled concurrent requests and synchronization carefully to avoid **race conditions, deadlocks, and inconsistent partner allocation**.
* Explored production-level concerns such as **timeouts, cancellation, failure propagation, scheduler reliability, and scalability**.

**Tech Stack:** Golang, Goroutines, Channels, Mutex/RWMutex, Concurrent Data Structures, REST APIs, Repository–Service Architecture, Background Workers, Scheduling.
