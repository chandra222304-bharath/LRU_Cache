# LRU_Cache
This is a console based project which in built in java

# 🧠 LRU Cache Management System in Java

## 📌 Project Overview

The **LRU (Least Recently Used) Cache Management System** is a Java-based console application that demonstrates how cache memory can be managed efficiently using a **HashMap and Doubly Linked List**.

The system stores key-value pairs and automatically removes the least recently used element when the cache reaches its maximum capacity.

It follows the LRU caching principle, where recently accessed or inserted elements are given higher priority, while elements that have not been accessed for the longest time are removed first.

## 🚀 Features

- **Dynamic Cache Capacity:** Allows users to specify the cache capacity at runtime.
- **Put Operation:** Inserts a new key-value pair into the cache.
- **Get Operation:** Retrieves a value using its key and updates its usage priority.
- **Automatic Eviction:** Removes the Least Recently Used (LRU) element when the cache is full.
- **Display Cache:** Displays all cache elements from Most Recently Used (MRU) to Least Recently Used (LRU).
- **Update Existing Keys:** Updates the value of an existing key and moves it to the MRU position.
- **Interactive Console:** Provides a simple command-based interface to interact with the cache.

## 🛠️ Technologies Used

- Java
- HashMap
- Doubly Linked List
- Object-Oriented Programming (OOP)
- Java Collections Framework

## ⚙️ Data Structures Used

### 1. HashMap

A HashMap stores key-node pairs and provides efficient lookup of cache elements.

**Time Complexity:** O(1) average for lookup.

### 2. Doubly Linked List

A doubly linked list maintains the usage order of cache elements.

- Head represents the MRU position.
- Tail represents the LRU position.
- Recently accessed elements are moved to the front.
- Least recently used elements are removed from the end.

## 📂 Project Structure

```text
LRU-Cache/
│
├── LRUApp.java
└── README.md
```

## ▶️ How to Run

**Step 1: Clone the repository**

```bash
git clone <your-repository-url>
```

**Step 2: Navigate to the project directory**

```bash
cd LRU-Cache
```

**Step 3: Compile the Java file**

```bash
javac LRUApp.java
```

**Step 4: Run the application**

```bash
java LRUApp
```

## 💻 Sample Execution

```text
Enter cache capacity:
3

🧠 LRU Cache Console

Commands:
  put <key> <value>
  get <key>
  display
  exit

> put 1 100
✅ Put done

> put 2 200
✅ Put done

> put 3 300
✅ Put done

> get 1
🔍 Value: 100

> display
📦 Cache Contents:
Most Recently Used -> [1:100] [3:300] [2:200] -> Least Recently Used

> put 4 400
✅ Put done

> display
📦 Cache Contents:
Most Recently Used -> [4:400] [1:100] [3:300] -> Least Recently Used

> exit
👋 Exiting...
```

**Explanation:**

When key `4` is inserted, the cache is already full. Since key `2` is the Least Recently Used element, it is automatically removed to make space for the new element.

## ⏱️ Time and Space Complexity

| Operation | Time Complexity |
|---|---|
| Get | O(1) average |
| Put | O(1) average |
| Remove LRU | O(1) |
| Display | O(n) |

**Space Complexity:** O(C), where C is the cache capacity.

## 🎯 Learning Outcomes

- Understanding the LRU caching algorithm.
- Implementing a HashMap and Doubly Linked List together.
- Applying efficient data structures to optimize time complexity.
- Understanding object references and pointer manipulation in Java.
- Implementing real-world cache management concepts.

## 🔮 Future Enhancements

- Develop a graphical user interface using HTML, CSS, and JavaScript.
- Add cache statistics such as hit count and miss count.
- Implement a web-based cache management dashboard.
- Add support for different cache replacement policies such as MRU and FIFO.

## 👨‍💻 Author

**Bharath Chandra**

