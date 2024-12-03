# Dependency Injection (DI) 📦

**Dependency Injection (DI)** is a design pattern commonly used in software development. It aims to provide a class with its required dependencies from external sources rather than creating them within the class. This method promotes modularity, testability, and flexibility in software.

---

## ✨ Advantages
- **Loose Coupling:** Reduces the dependencies between classes.
- **Testability:** Enables the use of mocks and stubs for isolated testing.
- **Reusability:** Dependencies can be reused in different scenarios.
- **Maintainability:** Promotes cleaner and more sustainable code.

---

## 🚀 Why Use Dependency Injection?

In traditional approaches, classes often create their own dependencies, leading to tightly coupled designs. Dependency Injection addresses this by providing dependencies externally, offering the following benefits:
- More flexible code structures.
- Easier modification and updates.
- Reduced code complexity.

---

## 🔧 Implementation Methods

### 1️⃣ Constructor Injection
Dependencies are provided through the class constructor:
```java
class Service {
    private final Dependency dependency;

    public Service(Dependency dependency) {
        this.dependency = dependency;
    }
}
