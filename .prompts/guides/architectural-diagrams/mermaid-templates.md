# 🔧 Mermaid Diagram Templates

Ready-to-use **Mermaid templates** for common architectural scenarios. Copy,
customize, and use these as starting points for your system diagrams.

## 🎯 **How to Use Templates**

1. **Choose the appropriate template** based on your use case
2. **Copy the Mermaid code** to your editor or Mermaid Live Editor
3. **Replace placeholder text** with your actual components/flows
4. **Customize styling** and add/remove components as needed
5. **Validate syntax** using Mermaid preview or online editor

---

## 📊 **Template Collection**

### **1. API Request Flow (Sequence Diagram)**

**Use for:** API interactions, user authentication flows, microservice
communication

```mermaid
sequenceDiagram
    participant User as 👤 User
    participant Frontend as 🌐 Frontend App
    participant API as 🔌 API Gateway
    participant Auth as 🔐 Auth Service
    participant DB as 🗄️ Database

    User->>Frontend: Click Login
    Frontend->>Frontend: Validate Form
    Frontend->>API: POST /auth/login
    API->>Auth: Validate Credentials
    Auth->>DB: Query User Table
    DB-->>Auth: User Data
    Auth-->>API: JWT Token
    API-->>Frontend: 200 + Token
    Frontend-->>User: Redirect to Dashboard

    Note over Auth,DB: Error handling paths
    Auth->>Frontend: 401 Invalid Credentials
    DB->>Auth: Connection Error
```

**Customization:**

- Replace participant names with your actual services
- Add/remove steps based on your flow
- Include error handling paths specific to your system

---

### **2. Business Logic Flow (Flowchart)**

**Use for:** Decision trees, business process flows, algorithm visualization

```mermaid
flowchart TD
    Start([User Action]) --> Input[Receive Input]
    Input --> Validate{Input Valid?}

    Validate -->|No| Error[Show Error Message]
    Error --> Start

    Validate -->|Yes| Process[Process Business Logic]
    Process --> Check{Check Conditions}

    Check -->|Condition A| PathA[Execute Path A]
    Check -->|Condition B| PathB[Execute Path B]
    Check -->|Default| PathC[Execute Default Path]

    PathA --> Save[(Save to Database)]
    PathB --> Save
    PathC --> Save

    Save --> Success[Return Success Response]
    Success --> End([Complete])

    %% Error handling
    Save -->|Database Error| Rollback[Rollback Transaction]
    Rollback --> Error
```

**Customization:**

- Replace decision points with your business rules
- Add parallel processing paths if needed
- Include specific error handling for your domain

---

### **3. System Architecture (Component Diagram)**

**Use for:** High-level system overview, microservices architecture, service
interactions

```mermaid
flowchart TB
    subgraph "Frontend Layer"
        Web[Web App]
        Mobile[Mobile App]
        Admin[Admin Panel]
    end

    subgraph "API Gateway"
        Gateway[Load Balancer/API Gateway]
    end

    subgraph "Services Layer"
        UserService[User Service]
        OrderService[Order Service]
        PaymentService[Payment Service]
        NotificationService[Notification Service]
    end

    subgraph "Data Layer"
        UserDB[(User Database)]
        OrderDB[(Order Database)]
        Cache[(Redis Cache)]
    end

    subgraph "External"
        PaymentAPI[Payment Provider]
        EmailService[Email Service]
    end

    Web --> Gateway
    Mobile --> Gateway
    Admin --> Gateway

    Gateway --> UserService
    Gateway --> OrderService
    Gateway --> PaymentService

    UserService --> UserDB
    UserService --> Cache
    OrderService --> OrderDB
    OrderService --> Cache
    PaymentService --> PaymentAPI
    NotificationService --> EmailService

    OrderService -.-> UserService
    OrderService -.-> PaymentService
    OrderService -.-> NotificationService
```

**Customization:**

- Replace services with your actual microservices
- Add/remove data stores based on your architecture
- Include message queues, caches, or other infrastructure

---

### **4. Data Model Relationships (Class Diagram)**

**Use for:** Database schemas, object relationships, inheritance structures

```mermaid
classDiagram
    class User {
        +String id
        +String email
        +String name
        +DateTime createdAt
        +login()
        +logout()
        +updateProfile()
    }

    class Order {
        +String id
        +String userId
        +Decimal total
        +String status
        +DateTime createdAt
        +addItem()
        +removeItem()
        +calculateTotal()
    }

    class OrderItem {
        +String id
        +String orderId
        +String productId
        +Integer quantity
        +Decimal price
        +updateQuantity()
    }

    class Product {
        +String id
        +String name
        +String description
        +Decimal price
        +Integer stock
        +updateStock()
        +getDetails()
    }

    User ||--o{ Order : "places"
    Order ||--o{ OrderItem : "contains"
    Product ||--o{ OrderItem : "includes"

    class PaymentMethod {
        <<interface>>
        +processPayment()
        +refund()
    }

    class CreditCard {
        +String cardNumber
        +String expiryDate
        +processPayment()
        +refund()
    }

    class PayPal {
        +String accountEmail
        +processPayment()
        +refund()
    }

    PaymentMethod <|-- CreditCard
    PaymentMethod <|-- PayPal
    Order --> PaymentMethod : "uses"
```

**Customization:**

- Replace classes with your actual data models
- Add specific methods and properties for your domain
- Include inheritance relationships if applicable

---

### **5. Simple Data Flow (Graph)**

**Use for:** Simple directional relationships, basic system connections

```mermaid
graph TD
    Input[User Input] --> Validation[Input Validation]
    Validation --> Transform[Data Transformation]
    Transform --> Business[Business Logic]
    Business --> Storage[(Data Storage)]
    Storage --> Response[Generate Response]
    Response --> Output[User Output]

    Business --> Audit[Audit Log]
    Business --> Notify[Notifications]

    Validation --> Error[Error Handler]
    Transform --> Error
    Business --> Error
    Storage --> Error
```

**Customization:**

- Replace nodes with your actual processing steps
- Add parallel flows or alternative paths
- Include monitoring and logging components

---

## 🎨 **Styling and Customization**

### **Adding Colors and Styles**

```mermaid
flowchart TD
    A[Normal] --> B[Success]
    A --> C[Warning]
    A --> D[Error]

    classDef success fill:#d4edda,stroke:#155724,color:#155724
    classDef warning fill:#fff3cd,stroke:#856404,color:#856404
    classDef error fill:#f8d7da,stroke:#721c24,color:#721c24

    class B success
    class C warning
    class D error
```

### **Using Subgraphs for Organization**

```mermaid
flowchart TB
    subgraph "Frontend"
        A[Component A]
        B[Component B]
    end

    subgraph "Backend"
        C[Service C]
        D[Service D]
    end

    A --> C
    B --> D
```

## 💡 **Best Practices**

1. **Start simple** → Begin with basic structure, add complexity gradually
2. **Use clear labels** → Descriptive names over technical variable names
3. **Group related items** → Use subgraphs for logical organization
4. **Show data flow** → Make direction of information clear
5. **Include error paths** → Don't forget edge cases and failures
6. **Validate syntax** → Test in Mermaid Live Editor before sharing

## 🔗 **Helpful Resources**

- **Mermaid Live Editor**: [https://mermaid.live/](https://mermaid.live/)
- **Mermaid Documentation**: [https://mermaid.js.org/](https://mermaid.js.org/)
- **Syntax Reference**:
  [https://mermaid.js.org/syntax/](https://mermaid.js.org/syntax/)

---

**Choose a template that matches your use case, customize it with your specific
components, and validate the syntax before using!**
