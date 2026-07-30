# Learn Python Roadmap

> A complete, step-by-step roadmap to learn Python from zero to job-ready. Each step links to free, in-depth tutorials from PyShine.

[![GitHub stars](https://img.shields.io/github/stars/pyshine-labs/learn-python-roadmap?style=social)](https://github.com/pyshine-labs/learn-python-roadmap/stargazers)
[![License: CC0](https://img.shields.io/badge/License-CC0-green.svg)](LICENSE)
[![Tutorials: 50+](https://img.shields.io/badge/Tutorials-50%2B-blue)](https://pyshine.com)
[![Time: 12 Weeks](https://img.shields.io/badge/Duration-12_Weeks-orange)](#timeline)

This roadmap takes you from absolute beginner to Python developer in 12 weeks. Every step includes links to free, hands-on tutorials.

Maintained by **[PyShine](https://pyshine.com)** -- 600+ free programming tutorials.

---

## Roadmap Overview

```
┌─────────────────────────────────────────────────────────────────┐
│                     LEARN PYTHON ROADMAP                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Week 1-2          Week 3-4          Week 5-6                   │
│  ┌─────────┐      ┌─────────┐      ┌─────────┐                 │
│  │  Python │ ───► │ Python  │ ───► │  OOP &  │                 │
│  │ Basics  │      │ Inter. │      │ Design  │                 │
│  └─────────┘      └─────────┘      └─────────┘                  │
│      │                │                │                        │
│      ▼                ▼                ▼                        │
│  Variables        Decorators      Classes                       │
│  Data Types       Generators      Inheritance                   │
│  Control Flow     Context Mgr     Polymorphism                  │
│  Functions        Async/Await     Design Patterns               │
│                                                                 │
│  Week 7-8          Week 9-10         Week 11-12                 │
│  ┌─────────┐      ┌─────────┐      ┌─────────┐                 │
│  │ Advanced│ ───► │   Web   │ ───► │  AI &   │                 │
│  │ Python  │      │ & APIs  │      │ Deploy  │                 │
│  └─────────┘      └─────────┘      └─────────┘                  │
│      │                │                │                        │
│      ▼                ▼                ▼                        │
│  Meta-classes      FastAPI        Machine Learning              │
│  Concurrency       REST APIs      AI Agents                     │
│  Testing           Databases      Docker & Deploy               │
│  Performance       Web Scraping   Production                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Timeline

| Week | Topic | Difficulty | Hours/Day |
|------|-------|------------|-----------|
| 1-2 | Python Basics | Beginner | 2-3 |
| 3-4 | Intermediate Python | Beginner-Intermediate | 2-3 |
| 5-6 | OOP & Design Patterns | Intermediate | 2-3 |
| 7-8 | Advanced Python | Intermediate-Advanced | 3-4 |
| 9-10 | Web & APIs | Intermediate | 3-4 |
| 11-12 | AI & Deployment | Advanced | 3-4 |

---

## Week 1-2: Python Basics

### What you'll learn
- Install Python and set up your environment
- Variables, data types, operators
- Control flow (if/else, loops)
- Functions
- Lists, tuples, dictionaries, sets
- String manipulation
- File I/O basics

### Tutorials

1. **[Python Installation and Setup](https://pyshine.com/Learn-Python-Part-01/)**
   - Install Python 3.12+
   - Set up VS Code
   - Create a virtual environment
   - Install packages with pip

2. **[Python Variables and Data Types](https://pyshine.com/Learn-Python-Part-01/)**
   ```python
   # Numbers
   age = 25              # int
   height = 5.9          # float
   complex_num = 3 + 4j  # complex

   # Strings
   name = "Alice"
   greeting = f"Hello, {name}!"

   # Booleans
   is_student = True

   # None
   address = None
   ```

3. **[Python Control Flow](https://pyshine.com/Learn-Python-Part-01/)**
   ```python
   # if/elif/else
   score = 85
   if score >= 90:
       grade = "A"
   elif score >= 80:
       grade = "B"
   else:
       grade = "C"

   # Loops
   for i in range(5):
       print(i)

   while True:
       user_input = input("Enter 'quit' to exit: ")
       if user_input == "quit":
           break
   ```

4. **[Python Functions](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   def greet(name, greeting="Hello"):
       """Greet someone with a custom message."""
       return f"{greeting}, {name}!"

   # Default arguments
   print(greet("Alice"))           # Hello, Alice!
   print(greet("Bob", "Hi"))      # Hi, Bob!

   # Lambda functions
   square = lambda x: x ** 2
   print(square(5))  # 25
   ```

5. **[Python Data Structures](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   # Lists (mutable, ordered)
   fruits = ["apple", "banana", "cherry"]
   fruits.append("date")
   fruits[0] = "apricot"

   # Tuples (immutable, ordered)
   coordinates = (40.7128, -74.0060)

   # Dictionaries (key-value pairs)
   person = {"name": "Alice", "age": 30, "city": "NYC"}

   # Sets (unique elements, unordered)
   unique_numbers = {1, 2, 3, 3, 2, 1}  # {1, 2, 3}
   ```

6. **[Python String Manipulation](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   # String methods
   text = "Hello, World!"
   print(text.upper())        # HELLO, WORLD!
   print(text.lower())        # hello, world!
   print(text.split(","))     # ['Hello', ' World!']
   print(text.replace("World", "Python"))  # Hello, Python!

   # f-strings (Python 3.6+)
   name = "Alice"
   age = 30
   print(f"{name} is {age} years old")

   # String slicing
   print(text[0:5])   # Hello
   print(text[-6:])   # World!
   print(text[::-1])  # !dlroW ,olleH
   ```

7. **[Python File I/O](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   # Reading files
   with open("input.txt", "r") as f:
       content = f.read()
       lines = f.readlines()

   # Writing files
   with open("output.txt", "w") as f:
       f.write("Hello, World!\n")
       f.writelines(["Line 1\n", "Line 2\n"])

   # Using pathlib (modern approach)
   from pathlib import Path
   p = Path("data.txt")
   text = p.read_text()
   p.write_text("New content")
   ```

### Projects to Build
- Calculator
- Number guessing game
- Todo list (CLI)
- File organizer script

### Checkpoint
- [ ] Can you write a function with default arguments?
- [ ] Can you iterate over a dictionary?
- [ ] Can you read and write files?
- [ ] Can you use list comprehensions?

---

## Week 3-4: Intermediate Python

### What you'll learn
- List/dict comprehensions
- Decorators
- Generators and iterators
- Context managers
- Error handling
- Working with modules and packages
- Regular expressions

### Tutorials

1. **[75+ Good Python Coding Examples](https://pyshine.com/Quick-Python-Tips/)** - Comprehensive tips and tricks

2. **[40 Essential Tips to Write Better Python](https://pyshine.com/Fourty-tips-to-write-better-python/)** - Best practices

3. **[Difference Between Yield and Return](https://pyshine.com/Difference-between-yield-and-return-in-python/)**
   ```python
   # return -- stops function, returns one value
   def get_squares_list(n):
       result = []
       for i in range(n):
           result.append(i ** 2)
       return result

   # yield -- pauses function, produces values lazily
   def get_squares_gen(n):
       for i in range(n):
           yield i ** 2

   # Generator is memory-efficient
   for sq in get_squares_gen(1000000):  # Uses ~0 bytes
       if sq > 100:
           break
   ```

4. **[Decorators Deep Dive](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   from functools import wraps
   import time

   def timing(func):
       @wraps(func)
       def wrapper(*args, **kwargs):
           start = time.perf_counter()
           result = func(*args, **kwargs)
           print(f"{func.__name__}: {time.perf_counter()-start:.4f}s")
           return result
       return wrapper

   @timing
   def slow_operation():
       import time
       time.sleep(1)
   ```

5. **[Python Cheatsheet Every Learner Must Know](https://pyshine.com/2026-02-17-Python-Cheatsheet/)**

### Projects to Build
- Web scraper (using requests + BeautifulSoup)
- Log file analyzer
- CSV data processor

---

## Week 5-6: OOP & Design Patterns

### What you'll learn
- Classes and objects
- Inheritance and MRO
- Polymorphism and duck typing
- Magic/dunder methods
- Abstract base classes
- Design patterns (Singleton, Factory, Observer, Strategy)
- SOLID principles

### Tutorials

1. **[Python OOP Tutorial](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   class Animal:
       def __init__(self, name, sound):
           self.name = name
           self.sound = sound

       def speak(self):
           return f"{self.name} says {self.sound}"

   class Dog(Animal):
       def __init__(self, name):
           super().__init__(name, "Woof")

       def fetch(self):
           return f"{self.name} fetches the ball!"

   dog = Dog("Buddy")
   print(dog.speak())   # Buddy says Woof
   print(dog.fetch())   # Buddy fetches the ball!
   ```

   ```python
   # Singleton
   class Database:
       _instance = None

       def __new__(cls):
           if cls._instance is None:
               cls._instance = super().__new__(cls)
               cls._instance.connection = "connected"
           return cls._instance

   # Factory
   class AnimalFactory:
       @staticmethod
       def create(animal_type):
           if animal_type == "dog":
               return Dog("Buddy")
           elif animal_type == "cat":
               return Cat("Whiskers")
   ```

### Projects to Build
- Bank account system (classes, inheritance)
- Library management system
- Shape calculator (polymorphism)

---

## Week 7-8: Advanced Python

### What you'll learn
- Async/await and asyncio
- Multiprocessing and threading
- Metaclasses
- Descriptors
- Type hints and mypy
- Testing (pytest)
- Performance optimization

### Tutorials

1. **[Python Performance Tips](https://pyshine.com/Tips-for-faster-python-code/)**
   ```python
   # Use built-in functions
   sum(range(1000))  # Faster than manual loop

   # Use generators for large data
   (x**2 for x in range(1000000))  # Memory-efficient

   # Use __slots__ for memory
   class Point:
       __slots__ = ['x', 'y']

   # Cache expensive calls
   from functools import lru_cache

   @lru_cache(maxsize=128)
   def fibonacci(n):
       if n < 2: return n
       return fibonacci(n-1) + fibonacci(n-2)
   ```

2. **[Async/Await Tutorial](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   import asyncio
   import aiohttp

   async def fetch_url(session, url):
       async with session.get(url) as response:
           return await response.text()

   async def fetch_all(urls):
       async with aiohttp.ClientSession() as session:
           tasks = [fetch_url(session, url) for url in urls]
           return await asyncio.gather(*tasks)

   # Run multiple requests concurrently
   urls = ["https://api.example.com/1", "https://api.example.com/2"]
   results = asyncio.run(fetch_all(urls))
   ```

3. **[Python Type Hints Tutorial](https://pyshine.com/Learn-Python-in-One-Post-Complete-Tutorial-Async-Type-Hints-Quick-Start/)**
   ```python
   from typing import List, Dict, Optional, Union

   def greet(name: str) -> str:
       return f"Hello, {name}"

   def process_items(items: List[int]) -> Dict[str, int]:
       return {"sum": sum(items), "count": len(items)}

   def find_user(user_id: int) -> Optional[Dict]:
       # Returns dict or None
       pass
   ```

### Projects to Build
- Async web scraper (1000+ pages concurrently)
- CLI tool with argparse
- Unit-tested library (100% coverage)

---

## Week 9-10: Web & APIs

### What you'll learn
- FastAPI / Flask
- REST API design
- Database integration (SQLAlchemy, SQLite)
- Authentication
- Web scraping
- WebSocket

### Tutorials

1. **[FastAPI Tutorial - Build REST APIs](https://pyshine.com/Learn-FastAPI-in-One-Post-Complete-Tutorial-Pydantic-Async-Dependency-Injection-Quick-Start/)**
   ```python
   from fastapi import FastAPI, HTTPException
   from pydantic import BaseModel

   app = FastAPI()

   class Item(BaseModel):
       name: str
       price: float
       description: Optional[str] = None

   items = {}

   @app.get("/items/{item_id}")
   def get_item(item_id: int):
       if item_id not in items:
           raise HTTPException(status_code=404, detail="Item not found")
       return items[item_id]

   @app.post("/items/")
   def create_item(item: Item):
       item_id = len(items) + 1
       items[item_id] = item
       return {"id": item_id, **item.dict()}
   ```

2. **[SQLAlchemy Tutorial](https://pyshine.com/Learn-SQL-in-One-Post-Complete-Tutorial-Joins-Window-Functions-Transactions-Quick-Start/)**
   ```python
   from sqlalchemy import create_engine, Column, Integer, String
   from sqlalchemy.orm import declarative_base, sessionmaker

   engine = create_engine("sqlite:///app.db")
   Base = declarative_base()

   class User(Base):
       __tablename__ = "users"
       id = Column(Integer, primary_key=True)
       name = Column(String)
       email = Column(String, unique=True)

   Base.metadata.create_all(engine)
   Session = sessionmaker(bind=engine)
   ```

3. **[Web Scraping with BeautifulSoup](https://pyshine.com/Scrapling-Adaptive-Web-Scraping-AI-Element-Tracking/)**

### Projects to Build
- REST API for a blog
- Web scraper that saves to database
- Real-time chat with WebSocket

---

## Week 11-12: AI & Deployment

### What you'll learn
- Machine learning basics
- AI agents and LLMs
- Docker
- CI/CD
- Cloud deployment

### Tutorials

1. **[Introduction to AI Agents](https://pyshine.com/12-Factor-Agents-Reliable-LLM-Powered-Software/)**
   ```python
   from openai import OpenAI

   client = OpenAI()

   def ai_agent(task):
       response = client.chat.completions.create(
           model="gpt-4",
           messages=[
               {"role": "system", "content": "You are a helpful assistant."},
               {"role": "user", "content": task}
           ]
       )
       return response.choices[0].message.content

   print(ai_agent("Write a Python function to sort a list"))
   ```

2. **[Build Your First AI Agent](https://pyshine.com/Build-Your-Own-X-Master-Programming-by-Recreating-Technologies/)**

3. **[Machine Learning with Python](https://pyshine.com/Learn-Machine-Learning-in-One-Post-Complete-Tutorial-Supervised-Unsupervised-Deep-Learning-Quick-Start/)**

4. **[Docker for Python Developers](https://pyshine.com/Learn-Docker-in-One-Post-Complete-Tutorial-Dockerfile-Volumes-Compose-Quick-Start/)**

### Projects to Build
- AI chatbot
- ML model deployed as API
- Full-stack app deployed to cloud

---

## Additional Resources

### Books (Free)
- [Think Python](https://greenteapress.com/wp/think-python-3rd-edition/) - Allen Downey
- [Automate the Boring Stuff](https://automatetheboringstuff.com/) - Al Sweigart
- [Python Documentation](https://docs.python.org/3/)

### Practice
- [LeetCode](https://leetcode.com/) - Coding interview practice
- [HackerRank](https://hackerrank.com/) - Python challenges
- [Exercism](https://exercism.org/tracks/python) - Python exercises

### Cheatsheets
- [Python Cheatsheet](https://pyshine.com/2026-02-17-Python-Cheatsheet/) - PyShine
- [75+ Python Tips](https://pyshine.com/Quick-Python-Tips/) - PyShine

### Interview Prep
- [Python Interview Questions](https://github.com/pyshine-labs/python-interview-questions) - 150+ Q&A
- [Python Interview Questions on PyShine](https://pyshine.com/Interview-questions-for-python-programming/)

### YouTube
- [PyShine YouTube Channel](https://youtube.com/@pyshine) - Video tutorials

---

## FAQ

### How long does it take to learn Python?
- **Basics:** 2-4 weeks
- **Intermediate:** 2-3 months
- **Job-ready:** 6-12 months (with projects)
- **Expert:** 2+ years

### Do I need a CS degree?
No. Many Python developers are self-taught. Build projects, contribute to open source, and create a portfolio.

### Which Python version should I use?
Always use the latest stable Python 3.x (currently Python 3.13). Python 2 is end-of-life.

### Should I learn Flask or FastAPI?
FastAPI is modern, faster, and has built-in type validation. Start with FastAPI unless you're maintaining legacy code.

### How do I stay motivated?
- Build projects you're passionate about
- Join communities (PyShine Discord, Reddit r/Python)
- Contribute to open source
- Teach what you learn

---

## Contributing

Found a great resource? Want to improve the roadmap?

1. Fork this repo
2. Edit README.md
3. Submit a pull request

## License

[CC0 1.0 (Public Domain)](LICENSE)

## About

Maintained by **[PyShine](https://pyshine.com)** -- 600+ free programming tutorials.

- Website: [https://pyshine.com](https://pyshine.com)
- GitHub: [pyshine-labs](https://github.com/pyshine-labs)
- YouTube: [@pyshine](https://youtube.com/@pyshine)

---

**Found this useful?** Star this repo and share with someone learning Python!

**Ready to start?** Visit [pyshine.com](https://pyshine.com) for 600+ free tutorials.
