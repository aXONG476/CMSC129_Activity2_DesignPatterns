# Dateboxd: A UPV Dating App

## App Summary
**Dateboxd** is a dating app tailored for UPV students. While most dating app only allows the users to get to know their match through profile summaries and chats, Dateboxd allows you to check your match's vibe score from their previous matches. 

Before you even decide to meet at the lover's lane or commute to the city campus, you can check a match’s **Vibe Score**. This score is built from peer reviews of their **online-only interactions**. It’s basically a community-led "Vibe Check" to ensure you’re not wasting your time on low-effort matches, ghosters, or "catfishes."

### The Twist
This dating app is inspired by letterboxd, where instead of a movie, you can rate and review your previous matches. 
After you and your match chatted for a certain period, you can choose to vibe check or rate your match based on different optional categories, or you can leave a review about your experience with your match.

### The 5 Digital Vibe Categories:
1.  **Response Time (Ghost-Meter):** Does it take them 3-5 business days to reply, or is the energy consistent?
2.  **Quality of Conversation:** Is it just "kamusta?" and "hi," or do they actually know how to carry a conversation?
3.  **Profile Accuracy:** Does their digital persona match their actual vibe (and program/acad org)?
4.  **Digital Respect:** Do they stay respectful in the DMs, or are they sending unsolicited vibes?
5.  **Vibe Consistency:** Is the energy they give off in their bio the same energy you get in the chat?

### Leaving a Review
Other than rating them based on the given categories, users can also leave a review or anything they wanted other users to know about their match.

## Design Pattern Implementation
### 1. Creational Design Pattern
* **Name of Pattern:** Creational - Factory
* **Concept in Conyo:**
* **Visual Diagram:**
* **Why it Works Nga:**
* **Pseudocode:**

### 2. Behavioral Design Pattern
* **Name of Pattern:** Behavioral - Strategy
* **Concept in Conyo:**
* **Visual Diagram:**
* **Why it Works Nga:**
* **Pseudocode:**

### 3. Structural Design Pattern
* **Name of Pattern:** Structural - Decorator
* **Concept in Conyo:**

  Kasi nga optional only ang categorical ratings in Dateboxd, it is bagay talaga to make gamit Decorator Pattern to implement our feature. We start with the Base Review and wrap it layer by layer gamit ang decorators. It's like similar to making halo-halo where you can make pili the toppings you want to add. Like, you can make lagay sago if you want it in your halo halo or you not make lagay beans if it you don't like it. So in our Dateboxd, the user can just pili if gusto nila irate ang quality conversation, we can just make wrap our base review with qualityConversationDecorator. If they want to leave a review, the program will just wrap it with a review decorator. They are not made pilit to rate all categories or to bigay a review.

The base review ay foundation lang siya, and we just make wrap it with a specific decorator that the user wanted to implement.
* **Visual Diagram:**
* **Why it Works Nga:**

  Without our pinakamamahal na decorator, we need to make iba't ibang classes for the categories pati narin ang kanilang combinations na magmemake result on class explosion which is so hirap talaga to maintain sa isang dating app. Yung ating decorator makes our system to be very flexible talaga kasi we only need to wrap our base review to make dagdag the categories na want ng users irate, or if gusto nila magbigay ng review. This also adheres to the isa sa SOLID principles, yung Single Responsibility Principle kung saan each decorator only make focus sa kaniyang implementation, like yung profileAccuracyDecorator only make focus sa pagmanage ng pag-implement ng profile accuracy category, and so on, like gets ba? This will also make our buhay easier kung may idadagdag tayo na categories or ways to vibe check our matches like if magdagdag tayo ng tags na functionality other than the categories or reviews.
* **Pseudocode:**





