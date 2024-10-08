
# ELIZA Gets a Facelift

## How to use Eliza to create immersive language tutorials using Wade Brainerd’s ELIZA Python program and Doctor input file

Listed below is a log of a session that shows how the Doctor input file and the ELIZA program can create a new language-learning functionality and also retain the original Rogerian therapist role.

The first part of the log introduces basic conversational phrases, while the second part reverts to the familiar therapist-style interaction.

For the language learning part of the session, **[brackets]** are used to offer the user different options, allowing them to select responses from a guided list. This makes the learning experience more interactive and immersive.

I also made a small change to the ELIZA Python program to capture the user’s name and include it in the response from ELIZA.

---

### Example: English Tutorial

This conversation highlights how ELIZA is used to set up an English tutorial, such as exchanging greetings and ordering food:

```
ELIZA: Nice to meet you. How should we start? Say [hello world] to begin.  
USER: hello world  
USER: my name is Mel  
ELIZA: Mel, nice to meet you. How are you today? [ok] or [not ok]  
USER: ok  
ELIZA: Mel, glad to hear that. Say [good morning].  
USER: good morning  
ELIZA: Mel, Ok. Say [good afternoon].  
USER: good afternoon  
ELIZA: Mel, Ok. Say [good evening].  
USER: good evening  
ELIZA: It is dinner time. Say [I am hungry].  
USER: I am hungry  
ELIZA: What would you like to eat? [chicken] or [meat]?  
USER: chicken  
ELIZA: What would you like to eat with your chicken? [salad] or [soup]?  
USER: salad  
ELIZA: What beverage? [water], [tea], or [coffee]?  
USER: tea  
ELIZA: Ok, you will be getting tea with your dinner. Tell me more about yourself: [I am married] or [I am not married].  

Rogerian Therapist .. because no key setup for this user input..

USER: I am married  
ELIZA: Is it because you are married that you came to me?  
USER: yes  
ELIZA: You seem to be quite positive.  
USER: I feel really sad  
ELIZA: You say you feel really sad?  
USER: yes  
ELIZA: You are sure?  
USER: Who are you?  
ELIZA: Why are you interested in whether I am or not?  
USER: I love you  
ELIZA: Perhaps in your fantasies we love each other.
```

The revised `doctor.txt` file (included in this repository) has been modified to provide an immersive experience for learning basic phrases in a language. This is not a full language course, but rather an introduction to conversational phrases. Importantly, the original table entries for the Rogerian therapist are still included, so users can either engage in language learning or use the program in its original form.

---

### Example: Spanish Tutorial

A slightly different version of the Doctor file was used using the Twilio platform with google translate to create a Spanish tutorial.
 

```
Welcome to the Hal9000 language tutor... Text me [Hello] in Spanish to continue in Spanish or select another language such as [French], [Hebrew], [German], etc.
USER: Hello world
ELIZA: Thank you for dropping by. How are you? [*good* or *not good*]  
USER: Hola Mundo  
ELIZA: Gracias por pasarte. ¿Cómo estás? [*bueno* o *no bueno*]  
USER: Bueno  
ELIZA: Ok. Say [good morning]  
USER: Buenos días  
ELIZA: Ok. Say [good afternoon]  
USER: Buenas tardes  
ELIZA: Ok. Say [good evening]  
USER: Buenas noches  
ELIZA: It is dinner time. Say [I am hungry]  
USER: Tengo hambre  
ELIZA: What would you like to eat? [chicken] or [meat]?  
USER: Pollo  
ELIZA: What would you like to eat with your chicken? [salad] or [soup]?  
USER: Ensalada  
ELIZA: What beverage? [water], [tea], or [coffee]?
```

