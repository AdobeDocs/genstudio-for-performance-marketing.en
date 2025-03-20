---
title: Text features
description: Learn about the text feature of attribute categories used in GenStudio for Performance Marketing.
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
---
# Text features

Text features include counts for certain text elements, such as words, sentences, emojis, and classifications for semantics, emotion, and tone that are used for analysis with [!DNL Insights]. Text may also receive a readability score.

GenStudio for Performance Marketing uses Adobe's AI and machine learning capabilities to study text and apply [!UICONTROL Media attributes] based on the associated text tones and marketing narrative. The process validates the input text to ensure it contains alphanumeric characters, removing extra white spaces and non-printable characters, and truncating the text to the maximum allowed 1500 words. Before applying detected attribute tags, the AI predicts the prevalent tone.

## Tone of voice

Tone represents a general character, attitude, or atmosphere exhibited through language. A simple choice of words and punctuation, sentence structure, and style can alter the tone of your message. For example, consider the following urgent messages using the three basic levels of tone:

| Tone           | Description                         | Example                                                   |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| Formal         | Polished and professional language. | `Take advantage of this distinctive and exceptional opportunity!` |
| Conversational | Friendly and informal language.     | `Don't miss out on this great opportunity!`                 |
| Direct         | Straightforward and to the point.   | `Don't miss the chance!`                                    |

Other secondary values for tone provide a finer distinction of the character and attitude of your message. In keeping with the earlier example of an urgent message, the GenAI may detect a _poetic_ tone in this whimsical example: `Embrace the moment, without delay, for this occasion won't always stay.`

The following table lists the tonal values recognized by the GenStudio for Performance Marketing AI.

| Tone           | Description                                      | Example                                                   |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| Enthusiastic   | Showing intense and eager enjoyment, interest, or approval. | `This is an amazing opportunity you can't miss!` |
| Assertive      | Confident and forceful in expression.            | `You need to act now to secure this deal!`                |
| Humorous/Witty | Light-hearted and clever.                        | `Why wait? Grab this deal before it's gone!`              |
| Inspirational  | Encouraging and uplifting.                       | `Believe in yourself and seize this opportunity!`         |
| Empathetic     | Showing understanding and sensitivity.           | `We understand your needs, and this is perfect for you.`  |
| Sensory        | Engaging the senses.                             | `Feel the excitement with this incredible offer!`         |
| Storytelling   | Narrating a story to convey a message.           | `Once upon a time, there was an offer you couldn't refuse.`|
| Poetic         | Artistic and expressive.                         | `Embrace the dawn of a new opportunity.`                  |
| Quantitative   | Based on numerical data.                         | `99% of users loved this offer, and you will too.` |

## Emotional appeal

Marketers leverage the power of human emotions to create a strong connection between the audience and the brand. By tapping into the senses such as happiness, fear, excitement, or nostalgia, marketers can craft messages that resonate on a deeper level, driving engagement and influencing consumer behavior. Emotional appeal helps deliver more relatable and memorable content, ultimately fostering brand loyalty and encouraging desired actions.

Persuasion tactics, marketing emotions, and narrative styles work together to target customer segments.

- **Narrative styles**, such as authenticity, celebration, and community, help convey the values and identity that resonate with the target audience, creating a more compelling and relatable message.
- **Persuasion tactics**, such as scarcity, social proof, and reciprocity, are designed to influence consumer behavior by appealing to their emotions and preferences.
- **Marketing emotions** aim to stimulate feelings that enhance engagement and connection with the brand.

GenStudio for Performance Marketing AI detects and distinguishes these characteristics by analyzing the text for emotional cues, tone, and narrative style. The AI uses natural language processing (NLP) and machine learning algorithms to identify patterns and classify the text based on predefined emotional and persuasive attributes.

### Narrative style

The narrative, or appeal factor, attributes help identify media that communicates the values, purpose, or identity that resonates with your target audience. The following table lists the narrative styles recognized by the GenStudio for Performance Marketing AI.

| Appeal factors    | Description                                                           | Example                                    |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Authenticity      | Genuine and real, often highlighting transparency and honesty.        | `A behind-the-scenes look at how our products are made.` |
| Celebration       | Marking special occasions or achievements with joy and festivity.     | `Join us in celebrating our 10th anniversary with special offers!` |
| Community         | Fostering a sense of belonging and togetherness among a group.        | `Our brand is built on the strength of our community.` |
| Convenience       | Emphasizing ease of use and time-saving benefits.                     | `Get what you need with just one click.` |
| Empowerment       | Encouraging and enabling individuals to take control and make decisions. | `Empower yourself with our latest tools and resources.` |
| Exploration       | Inviting discovery and adventure, often associated with new experiences. | `Discover new horizons with our travel packages.` |
| Futuristic        | Highlighting innovation and forward-thinking ideas.                   | `Experience the future of technology today.` |
| Hype              | Generating excitement and anticipation around a product or event.     | `Don't miss out on the most anticipated event of the year!` |
| Indulgence        | Appealing to fantasies, desires, or pleasures.                        | `Treat yourself to the finest gourmet chocolates.` |
| Peace of mind     | Providing reassurance and a sense of security.                        | `Rest easy knowing your data is safe with us.` |
| Personalization   | Tailoring experiences or products to individual preferences.          | `Get a custom-fit solution just for you.` |
| Prestige          | Associating with high status and exclusivity.                         | `Join the elite with our premium membership.` |
| Timelessness      | Emphasizing enduring quality and classic appeal.                      | `Our designs are timeless and never go out of style.` |
| Versatility       | Highlighting adaptability and multiple uses.                          | `Our product fits seamlessly into any lifestyle.` |
| Well-being        | Promoting health, happiness, and overall wellness.                    | `Enhance your well-being with our holistic approach.` |

### Persuasion tactics

Persuasion techniques are used to influence consumer behavior and drive desired actions. These strategies target specific psychological triggers and customer segments to enhance the effectiveness of marketing messages. The following table lists the persuasion tactics recognized by the GenStudio for Performance Marketing AI.

| Tactic                | Description                                                                 | Example                                                   |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Anthropomorphism      | Attributing human characteristics to products or brands.                    | `Our friendly chatbot is here to help you.`               |
| Comparison            | Highlighting differences between options to influence choice.               | `See how we compare to the competition.`                  |
| Concreteness          | Providing specific details to make the message more tangible.               | `Save 20% on your next purchase.`                         |
| Endorsement           | Featuring approval from credible sources or influencers.                    | `Recommended by top industry experts.`                    |
| Foot in the door      | Starting with a small request to increase the likelihood of agreement to a larger request. | `Try our free trial today.`                               |
| Overcoming reactance  | Reducing resistance by acknowledging and addressing objections.             | `We understand your concerns, and here's how we address them.` |
| Reciprocity           | Offering something of value to encourage a return favor.                    | `Get a free gift with your purchase.`                     |
| Scarcity              | Creating a sense of urgency by highlighting limited availability.           | `Only a few items left in stock!`                         |
| Social identity       | Leveraging the consumer's sense of belonging to a group.                    | `Join our community of innovators.`                       |
| Social impact         | Emphasizing the positive impact on society or the environment.              | `Your purchase helps plant a tree.`                       |
| Social proof          | Using testimonials or user-generated content to build trust.                | `See why thousands of users love our product.`            |

### Marketing Emotions

Emotions are targeted in marketing messages to evoke specific feelings and responses from the audience, which may enhance engagement and connection with the brand. The following table lists the emotions recognized by the GenStudio for Performance Marketing AI.

| Emotion       | Description                                                                 | Example                                                   |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Aspiration    | Inspiring a desire to achieve or attain something greater.                  | `Imagine the possibilities with our premium service.`     |
| Challenge     | Encouraging the audience to overcome an obstacle or embrace a new task.        | `Are you ready to take the next step in your career?`     |
| Curiosity     | Arousing interest and a desire to learn more.                               | `Discover the secrets behind our success.`                |
| Exclusivity   | Creating a sense of being part of a select group.                           | `Join our exclusive club for members-only benefits.`      |
| Fascination   | Captivating the audience with intriguing or exciting content.               | `Be amazed by our latest innovations.`                    |
| Gratification | Providing satisfaction and pleasure from using the product or service.      | `Enjoy the ultimate comfort with our luxury bedding.`     |
| Recognition   | Acknowledging and valuing the audience's achievements or status.            | `Get the recognition you deserve with our award-winning service.` |
| Trust         | Building confidence and reliability in the brand.                           | `Trust us to deliver quality and excellence every time.`  |
| Urgency       | Prompting immediate action by emphasizing time-sensitive opportunities.     | `Act now before this limited-time offer expires!`         |

## Readability scoring

Readability scoring assesses how easy a piece of text is to read and understand. It helps ensure that your content is appropriate for your target audience. The scores are based on various factors, including sentence length and word complexity. The following table lists the readability levels recognized by the GenStudio for Performance Marketing AI.

| Readability level   | Description                                                        | Example                                                   |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5th grade           | Very simple language, suitable for young children.                 | `The cat sat on the mat.`                                 |
| 6th grade           | Simple and clear language, suitable for a general audience.        | `You can find great deals on our website.`                |
| 7th grade           | Easy to understand, with straightforward vocabulary and structure. | `Our new product is simple to use and very effective.`    |
| 8th and 9th grade   | Clear and concise language, suitable for teenagers.                | `This guide will help you understand the basics of our service.` |
| 10th to 12th grade  | More complex language, suitable for older teenagers and adults.    | `The comprehensive manual provides detailed instructions for setup.` |
| College             | Advanced language, suitable for a well-educated audience.          | `The study explores the multifaceted implications of the new policy.` |
| College graduate    | Highly advanced language, suitable for experts and specialists.    | `The dissertation delves into the intricacies of quantum mechanics.` |

## Counts

Understanding and leveraging count attributes like hashtag counts, word counts, sentence counts, and stop words ratios can significantly enhance your content strategy. These metrics offer valuable insights into the effectiveness and reach of your marketing efforts. The following table lists the count categories recognized by the GenStudio for Performance Marketing AI.

| Category              | Description                                                                 | Example               |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| Emojis Count          | The number of emoji present in the text. Emojis can enhance engagement and convey emotions quickly. | `😊`, `🚀`, `❤️`       |
| HashTags Count        | The number of hashtags used in the text. Hashtags help categorize content and increase discoverability on social media. | `#Marketing`, `#Sale` |
| Words count per sentence | The average number of words per sentence in the text. Shorter sentences are often easier to read and understand. | `10`                  |
| Words Count           | The total number of words in the text. A higher word count can provide more detailed information but may also require more effort to read. | `1500 words`          |
| Stop words ratio      | The ratio of stop words to meaningful words in the text. Stop words (such as "a" "an" "the") are often ignored in search queries and results. A high ratio of stop words can make content less engaging and harder to read. | `0.375`               |
| Sentences count       | The total number of sentences in the text. More sentences can indicate more detailed content, but overly long texts may lose the reader interest. | `75 sentences`        |
