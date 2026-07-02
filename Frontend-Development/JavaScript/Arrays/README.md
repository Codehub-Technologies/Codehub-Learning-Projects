

---

## Task 1: The "Top Tracks" Playlist (Indexing & Length)

**Objective:** Practice reading specific items from an array using zero-based indexing and calculating the total size of the collection.

### Instructions:

You are building the dashboard for a music streaming application. Your database has returned a list of a user's favorite tracks in order of preference.

1. Write a console log statement that prints out the **first** song in the playlist array.
2. Write a console log statement that prints out the **third** song in the playlist array.
3. Use the `.length` property to calculate the total number of songs currently in the playlist. Log this number with a clear string descriptive message like: `"Total songs in your queue: X"`.

### Starter Code:

```javascript
const userPlaylist = ["Midnight City", "Electric Feel", "Starlight", "Bohemian Rhapsody"];

// Write your extraction and length inspection code below:

```

---

## Task 2: The Roster Swap (Array Mutation)

**Objective:** Learn how to target and overwrite specific items inside an array collection using assignment syntax.

### Instructions:

You are managing the team lineup for a multiplayer tournament match. Right before the game kicks off, player `"Sarah"` needs to be substituted out, and a bench player named `"David"` needs to take her exact place in the squad list.

1. Look closely at the `teamRoster` array to determine the correct **zero-based index position** of `"Sarah"`.
2. Write an assignment statement that targets her specific index position and replaces her value with the string `"David"`.
3. Log out the updated `teamRoster` array to the console to confirm that the swap was successful and the other teammates remained unchanged.

### Starter Code:

```javascript
const teamRoster = ["Alex", "Blessing", "Sarah", "John"];

// 2. Perform your roster substitution swap below:


// 3. Print the final roster array configuration:

```

---

## Task 3: The Queue and Inventory Stack (Modifications, Splice, Slice & Concat)

**Objective:** Master the mutator methods (`push`, `pop`, `shift`, `unshift`), absolute index engineering (`splice`), section extractions (`slice`), and array structural merges (`concat`).

### Instructions:

You are coding an automated task pipeline system for a server. Run the following actions sequentially on the starter arrays:

1. **Queue Management:** An incoming urgent task needs to be processed first. Use `unshift()` to add `"Urgent-Task"` to the *beginning* of the `activeQueue` array.
2. A lagging background process needs to be discarded. Use `pop()` to remove the *very last* element from `activeQueue`.
3. The oldest running item at the front is completed. Use `shift()` to remove the *very first* item from `activeQueue`.
4. **Splice & Insertion:** A high-priority item named `"Priority-X"` needs to be injected exactly between `"Task-2"` and `"Task-3"`. Use `splice()` on `activeQueue` to start at index `2`, delete `0` items, and insert `"Priority-X"`.
5. **Extraction:** Create a new array named `subQueue` by slicing out a subset of `activeQueue` containing *only* `"Task-2"` and `"Priority-X"`. (Hint: Use `slice()` with proper start/end indices).
6. **Merging:** Combine your newly created `subQueue` with the separate `backupQueue` array into a single final array called `unifiedPipeline` using `concat()`.

### Starter Code:

```javascript
const activeQueue = ["Task-1", "Task-2", "Task-3", "Task-4"];
const backupQueue = ["Fallback-Alpha", "Fallback-Beta"];

// Write your multi-step array engineering below:

```

---

## Task 4: The Data Transformations Lab (ForEach, Map, Filter & Reduce)

**Objective:** Master functional array loops to iterate, isolate targeted information, map dataset variations, and compress data rows to singular totals.

### Instructions:

You are analyzing a data matrix stream of sensor reading numbers. Write separate functional operations using the `sensorReadings` array:

1. **forEach:** Print each raw sensor reading value directly to the console one by one using a `forEach` block loop.
2. **map:** The physical sensors report their metrics in a custom scale, but you need to convert them to a double scale baseline. Use `map()` to generate a completely new array named `doubledReadings` where every element is multiplied by $2$.
3. **filter:** You need to weed out cold zones. Use `filter()` on `sensorReadings` to produce a new array named `warmReadings` that contains *only* values that are strictly greater than $15$.
4. **reduce:** Calculate the sum total of all values inside the `sensorReadings` array. Distill it down to a single numeric value stored in a variable named `totalSum`.

### Starter Code:

```javascript
const sensorReadings = [12, 25, 8, 19, 30, 15];

// Write your functional transformation pipelines below:

```

---

## Task 5: The Security Audit Search Engine (Searching & Logic Assertions)

**Objective:** Harness advanced conditional lookup helpers (`indexOf`, `includes`, `find`, `findIndex`, `findLast`) and structural assertion conditions (`some`, `every`).

### Instructions:

You are auditing user log data arrays to determine if the active session matches compliance standard indicators. Write expressions to test the `logins` array structure:

1. **indexOf:** Locate the index number where the string `"Admin"` first appears. Save it to a variable named `adminIndex`.
2. **includes:** Run a quick boolean inspection check to see if the element `"Guest"` is contained anywhere inside the list. Save it to `hasGuest`.
3. **find:** Search through the array to extract the **first** element that has a string character count strictly greater than 5 characters long (i.e., `item.length > 5`). Save it to `firstLongWord`.
4. **findIndex:** Locate the zero-based index of the **first** word that ends with the character `"r"`. Save it to `endsWithRIndex`.
5. **findLast:** Scan the array backwards from right to left to locate the **last** word that starts with the character `"M"`. Save it to `lastMWord`.
6. **some:** Check if **at least one** word in the collection is exactly equal to `"Superuser"`. Save the boolean result to `isSuperuserPresent`.
7. **every:** Verify if **absolutely every** username entry inside the collection is a valid string type (i.e., `typeof item === "string"`). Save the result to `allAreStrings`.

### Starter Code:

```javascript
const logins = ["Manager", "Admin", "Moderator", "User", "Member", "Guest"];

// Write your search queries and logic assessments below:

```

Here are three exercises designed to help students master ES6 array features: array destructuring (including skipping elements and setting default values), the Rest parameter, and the Spread operator.

---

## Task 6: The Olympics Podiums (Destructuring & Skipping)

**Objective:** Master array destructuring mechanics, including positional unpacking, skipping unneeded indices, and establishing default fallbacks.

### Instructions:

You are parsing the official final standings array for an athletic racing tournament. Write a single destructuring assignment statement to extract the matching data values:

1. Unpack the first two items into distinct variables named `gold` and `silver`.
2. Skip the third element entirely using an empty comma space placeholder.
3. Unpack the fourth element into a variable named `fourthPlace`.
4. Create a fifth variable named `wildcard` that falls back to the default string value `"Disqualified"` if no fifth element exists in the incoming array.
5. Print out all four variables using a `console.log` statement to confirm successful extraction.

### Starter Code:

```javascript
const finalStandings = ["Marathon-Runner-A", "Marathon-Runner-B", "Marathon-Runner-C", "Marathon-Runner-D"];

// Write your destructuring pattern on a single line below:


// Add your verification log below:

```

---

## Task 7: The VIP Guestlist (Rest Parameter Architecture)

**Objective:** Use the Rest parameter (`...`) to isolate primary leading entries while capturing variable remaining data elements into independent subset arrays.

### Instructions:

An event planner has a list of attendees checking into a venue. The first two names are elite corporate VIP sponsors who get premium seats, while the rest of the guests go into a standard ticketing buffer pool.

1. Use array destructuring along with the **Rest Parameter (`...`)** syntax to capture the first attendee into a variable named `vip1`, the second attendee into `vip2`, and all subsequent attendees into a brand new array called `generalAdmission`.
2. Write a separate standalone function named `multiplyAll(...factors)` that uses the Rest parameter to accept an infinite length list of number arguments and multiplies them together using `.reduce()`.
3. Test `multiplyAll(2, 3, 4)` in your console to verify it outputs `24`.

### Starter Code:

```javascript
const eventAttendees = ["Dr. Smith", "CEO Jones", "Alice", "Bob", "Charlie", "David"];

// 1. Unpack the VIPs and collect the remaining guests into a new array below:


// 2. Write your standalone multiplyAll function here:

```

---

## Task 8: The Content Feed Merge (Spread Operator & Safe Copies)

**Objective:** Harness the Spread operator (`...`) to flat-merge multiple separate data collections into a unified stream, and create reference-free data copies.

### Instructions:

You are building an administrative content dashboard that pulls structural arrays from different system feeds.

1. Create a brand new array named `completeFeed`. Use the **Spread Operator** to merge all items from `breakingNews` followed immediately by all items from `sportsFeed` inside a single layout context.
2. A junior developer wants to clone the `completeFeed` array to run some modifications, but they are worried about accidentally breaking the original array data. Create an independent shallow copy of `completeFeed` named `safeCopy` using the Spread operator.
3. Push the string `"New-Ad-Tag"` to the end of `safeCopy`.
4. Console log both `completeFeed` and `safeCopy` to verify that the original array remains safely untouched by the modification.

### Starter Code:

```javascript
const breakingNews = ["Headline-1", "Headline-2"];
const sportsFeed = ["Score-Update-A", "Score-Update-B"];

// 1. Merge the feeds using spread below:


// 2 & 3. Create a safe copy and push your new value to it:


// 4. Verify original array integrity below:

```

