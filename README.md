# Amazon-Alexa-Tutorial
A brief overview on how to make a basic Alexa skill using Java on AWS Lambda!

#### Things you'll need
- [amazon developer account](https://developer.amazon.com/)
- [amazon web services account](https://aws.amazon.com/)
- [some java proficiency](https://github.com/alexa/alexa-skills-kit-sdk-for-java)
- [a dash of maven](https://mvnrepository.com/artifact/com.amazon.alexa/alexa-skills-kit)
- [maybe an IDE](https://www.jetbrains.com/idea/)

#### Other great resources / reading
- [Alexa Developer Docs](https://developer.amazon.com/alexa-skills-kit)
- [The Geekette Speaketh](http://thegeekettespeaketh.com/2017/02/build-an-alexa-skill-java-1/)

### How to get Started
1. Decide on an idea. >[Maybe watch this](https://www.youtube.com/watch?v=QxgdPI1B7rg)<.
  1. [Think about what KIND of skill you want to make ...this doc is going to describe a custom skill!](https://developer.amazon.com/docs/ask-overviews/build-skills-with-the-alexa-skills-kit.html)
2. Log into your Amazon Dev Account, and describe your new Skill.
  1. Navigate to the alexa subsection >[Click here for direct link as of 8/13/18](https://developer.amazon.com/alexa)<.
  2. Find the 'Create a Skill' >[Click here for direct link as of 8/13/18](https://developer.amazon.com/alexa/console/ask/create-new-skill)<.
  3. Decide on a skill name! 
    * It should be at least 2 characters.
    *  Generally, make it something descriptive. Makes sense, eh?
  4. Start configuring your skill.
      * Your Invocation Name
        * ex: "Llama Dice"
        * This is basically the word phrase you'll use when interacting with an Alexa device to start up or trigger your program.
        * It should be 2-3 words, not using the reserved words like (Amazon/Alexa/Echo etc) and shouldn't break trademark law.
      * Your Intents w/ Slots
        * ex: "RollDiceIntent"
        * You can think of Intents kind of like the endpoints of your skill service, or like the different methods that could be executed within your program.
        * It should be a single phrase, PascalCased that describes the 'idea' behind the intent.
      * Slots
        * These are basically the parameter variables for your Intents described above.
        * They can either be custom defined, or one of the many [Amazon slots](https://developer.amazon.com/docs/custom-skills/slot-type-reference.html) defined.
      * Sample Utterances
        * ex: "roll a random die"
        * This is basically the word phrase that can trigger and of the described Intents above.
  5. Write a AWS webservice to provide for your Skill!
        * clone this repo!
        * Update to match for your services
          * Match for intents
          * parse for slots
          * return response & card
