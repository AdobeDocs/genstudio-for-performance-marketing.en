---
title: Text features
description: Learn about the text feature of attribute categories used in GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
hide: yes
hidefromtoc: no
recommendations: noDisplay, noCatalog
---
# Text features

Text features include counts for certain text elements, such as words, sentences, emojis, and classifications for semantics, emotion, and tone that are used for analysis with [!DNL Insights]. Text may also receive a readability score.

GenStudio for Performance Marketing uses Adobe's AI and machine learning capabilities to study text and apply [!UICONTROL Asset attributes] based on the associated text tones and marketing narrative. The process validates the input text to ensure it contains alphanumeric characters, removing extra white spaces and non-printable characters, and truncating the text to the maximum allowed 1500 words. Before applying detected attribute tags, the AI predicts the prevalent tone.

## Tone of voice

Tone represents a general character, attitude, or atmosphere exhibited through language. A simple choice of words and punctuation, sentence structure, and style can alter the tone of your message. For example, consider the following urgent messages using the three basic levels of tone:

- `Formal`

   ```
   Take advantage of this distinctive and exceptional opportunity!
   ```

- `Conversational`

   ```
   Don't miss out on this great opportunity!
   ```

- `Direct`

   ```
   Don't miss the chance!
   ```

The AI further detects a more nuanced tone. Using the same urgent statement from the earlier example, the following version uses a whimsical `poetic` tone:

- `Poetic`

   ```
   Embrace the moment, without delay, for this occasion won't always stay.
   ```

Other secondary values for tone include: `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Narrative

The narrative attributes help you to identify assets that communicate the values, purpose, or identity that resonates with your target audience.

| Narrative         | Description | Example |
| ----------------- | ----------- | ------- |
| `Authenticity`    |             |         |
| `Celebration`     |             |         |
| `Community`       |             |         |
| `Convenience`     |             |         |
| `Empowerment`     |             |         |
| `Exploration`     |             |         |
| `Futuristic`      |             |         |
| `Hype`            |             |         |
| `Indulgence`      |             |         |
| `Peace of mind`   |             |         |
| `Personalization` |             |         |
| `Prestige`        |             |         |
| `Timelessness`    |             |         |
| `Versatility`     |             |         |
| `Well-being`      |             |         |

## Readability scoring

Readability scoring assesses how easy a piece of text is to read and understand. It helps ensure that your content is appropriate for your target audience. The scores are based on various factors, including sentence length and word complexity.

| Score       | School level       | Notes                                                                     |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100.00-90.00| 5th grade          | Very easy to read. Easily understood by an average 11-year-old student.   |
| 90.0–80.0   | 6th grade          | Easy to read. Conversational English for consumers.                       |
| 80.0–70.0   | 7th grade          | Fairly easy to read.                                                      |
| 70.0–60.0   | 8th and 9th grade  | Plain English. Easily understood by 13- to 15-year-old students.          |
| 60.0–50.0   | 10th to 12th grade | Fairly hard to read.                                                      |
| 50.0–30.0   | College            | Hard to read.                                                             |
| 30.0–0.0    | College graduate   | Very hard to read. Best understood by university graduates.               |

## Word counts

TBD

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description   | Example               |
| -------------------- | ------------- | --------------------- |
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   | Emotions are targeted in marketing messages to evoke specific feelings and responses from the audience, which may enhance engagement and connection with the brand. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Persuasion Strategies | Techniques used to influence consumer behavior and drive desired actions. These strategies target specific psychological triggers and customer segments to enhance the effectiveness of marketing messages. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Tone of voice   | The general character, attitude, or atmosphere that is conveyed in a marketing message through word choice, punctuation, sentence structure, and style. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
