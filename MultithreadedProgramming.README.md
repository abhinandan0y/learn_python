#Multithreaded Programming:<br /> 

Example 1: Basic Multithreading

```python
import threading
import time

def print_numbers():
    for i in range(5):
        time.sleep(1)
        print(i)

def print_letters():
    for letter in 'ABCDE':
        time.sleep(1)
        print(letter)

thread1 = threading.Thread(target=print_numbers)
thread2 = threading.Thread(target=print_letters)

thread1.start()
thread2.start()

thread1.join()
thread2.join()
```
Example 2: Thread Synchronization

```python
import threading

counter = 0
lock = threading.Lock()

def increment():
    global counter
    for _ in range(100000):
        with lock:
            counter += 1

thread1 = threading.Thread(target=increment)
thread2 = threading.Thread(target=increment)

thread1.start()
thread2.start()

thread1.join()
thread2.join()

print("Counter:", counter)
```
Example 3: Producer-Consumer Problem

```python
import threading
import queue
import time

def producer(q):
    for i in range(5):
        time.sleep(1)
        q.put(i)
        print(f"Produced: {i}")

def consumer(q):
    while True:
        item = q.get()
        if item is None:
            break
        print(f"Consumed: {item}")

my_queue = queue.Queue()
thread_producer = threading.Thread(target=producer, args=(my_queue,))
thread_consumer = threading.Thread(target=consumer, args=(my_queue,))

thread_producer.start()
thread_consumer.start()

thread_producer.join()
my_queue.put(None)
thread_consumer.join()
```
Example 4: Thread Pooling

```python
from concurrent.futures import ThreadPoolExecutor

def square(number):
    return number ** 2

numbers = [1, 2, 3, 4, 5]

with ThreadPoolExecutor(max_workers=2) as executor:
    results = executor.map(square, numbers)

print(list(results))
```
Example 5: Asynchronous Programming

```python
import asyncio

async def count_up_to_5():
    for i in range(1, 6):
        print(i)
        await asyncio.sleep(1)

async def main():
    task1 = asyncio.create_task(count_up_to_5())
    task2 = asyncio.create_task(count_up_to_5())

    await asyncio.gather(task1, task2)

asyncio.run(main())
```
Advanced Application:
```python
#Developing a real-time chat application where multithreading is used to handle multiple user connections concurrently.
```
