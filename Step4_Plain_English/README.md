# Step 4: Plain English Logic (Implementation Plan)

This step describes how the system should behave using plain English.

---

##  Sequence of Tasks (Logic Steps)

1. Start the system.
2. Check if a train is approaching.
3. If a train is approaching → **Lower the gate immediately**.
4. If no train is approaching → Check if a vehicle is on the tracks.
5. If a vehicle is on the tracks → **Keep the gate lowered**.
6. If there is **no train** and **no vehicle**:
   - Wait for a short delay (e.g., 5 seconds) to confirm the track is still clear.
   - After the delay, check again.
   - If it’s still clear → **Raise the gate**.
   - If a train or vehicle appears → **Keep the gate lowered**.
7. Repeat the process continuously.

---

 This logic ensures the gate only raises when it’s completely safe.
