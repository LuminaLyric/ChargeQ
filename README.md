ChargeQ: Fair Power for Disaster Charging Hubs
Built for MOVE-A-THON 2026 (IEEE MOVE India). Focus: the first 72 hours after a disaster.
The problem
After a flood, cyclone or earthquake, a mobile phone is a lifeline. People use it to tell their family they are safe, call for rescue, reach a doctor, and receive official alerts. But the power is usually gone, so relief camps set up charging hubs with a battery bank and a few charging ports.
These hubs quickly become chaotic:
• Hundreds of people want to charge, but only a few can at a time.
• There is no fair order, so people push and argue.
• Rescue workers and medical staff wait in the same line as everyone else.
• Nobody knows how long the battery will last, so it dies without warning.
Our solution
ChargeQ is a simple app that runs on one phone or laptop at the hub. It manages the queue and the battery. It needs no special equipment and no training beyond a short demonstration.
How it works
1. Setup. The hub operator enters the battery size, the number of ports, and how long one phone takes to charge.
2. Priority tokens. Each person gets a token. Rescue and medical workers go first, then elderly people and families with children, then everyone else. Each person sees an estimated waiting time.
3. Power at a glance. The main screen shows the battery as blocks, where every block is one phone charge. Colored blocks show the people waiting. If more people are waiting than the battery can serve, the app shows a clear warning so the operator can act early.
4. Port management. The operator assigns the next person to a free port and marks when they are done. The remaining battery updates automatically.
5. Safe-Ping. While waiting, each person leaves a short message such as "I'm safe at the school shelter." These messages are exported as a batch that can be sent by SMS or radio as soon as any signal returns, so families hear from their loved ones.
6. Records. A log of who was served and how much power was used can be copied out for relief coordinators.
Why it matters
• Relevance: It addresses the first 72 hours, and it strengthens two of MOVE's own capabilities, power and communications.
• Innovation: Most disaster tools detect, predict or map. ChargeQ manages the scarce resource itself, fairly.
• Feasibility: The prototype already works as a web app.
• Cost: Near zero. It runs on a phone or laptop already at the hub.
• Scalability: It works with any existing charging setup, and any camp can use it.
Built to grow into hardware
Today the operator types in the battery level. The app talks to its power source through one simple interface, so real hardware can be added later without rebuilding the app:
• A current and voltage sensor reads the real battery level.
• Port relays switch each charging port on or off under the queue's control.
• A small ESP32 or Raspberry Pi creates a local Wi-Fi network, so people can join the queue from their own phones with no internet.
• An optional LoRa or SMS module sends Safe-Ping batches automatically.
The prototype includes a simulated sensor mode that demonstrates this roadmap. The hardware itself is planned work, not yet built.
Current status
A working software prototype exists. The sensor feed is simulated, and the hardware integration is the next stage, to be supported by the implementation grant.
