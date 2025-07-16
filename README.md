🔧 Cache Simulator in C
This project simulates different types of CPU caches using the C programming language. It helps users understand how memory addresses are handled in various caching techniques like Direct Mapped, Fully Associative, and Set Associative caches, and how replacement policies like FIFO, LRU, and RANDOM affect performance.

📌 Features
✅ Simulates:

Direct Mapped Cache

Fully Associative Cache

Set Associative Cache

🔁 Supports Replacement Policies:

FIFO (First-In First-Out)

LRU (Least Recently Used)

RANDOM

📊 Reports:

Cache Hits

Cache Misses

Hit/Miss Rate

🧠 Cache Types Explained with Diagrams
1️⃣ Direct Mapped Cache
Each memory block maps to exactly one cache line.
2️⃣ Fully Associative Cache
Any block can be placed anywhere in the cache. Needs a search on every access.
3️⃣ Set Associative Cache
The cache is divided into sets, and each set has multiple blocks (ways).
🔁 Replacement Policies
🔸 FIFO (First-In-First-Out)
Replace the oldest cache line in the set.

🔸 LRU (Least Recently Used)
Replace the line that was least recently accessed.

🔸 RANDOM
Replace a randomly chosen line in the set.

📥 Sample Input
txt
Copy
Edit
Cache Type: Set Associative (4-way)
Replacement Policy: LRU
Cache Size: 16 blocks
Memory Access Sequence: 0x1A3, 0x1B4, 0x1A3, 0x2C4, 0x1B4
📤 Sample Output
txt
Copy
Edit
Accessing 0x1A3: MISS
Accessing 0x1B4: MISS
Accessing 0x1A3: HIT
Accessing 0x2C4: MISS
Accessing 0x1B4: HIT

Total Hits: 2
Total Misses: 3
Hit Rate: 40%
