---
title: Attribute categories
description: Learn about attribute categories used in GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
---
# Attribute categories

An attribute category is a classification group that organizes related attributes that share a common characteristic. These categories help streamline the discovery, identification, and understanding of specific attributes by providing greater context and facilitating their application and use.

GenStudio for Performance Marketing uses Adobe's AI and machine learning capabilities to study images, videos, and text and apply [!UICONTROL Asset attributes] based on the level of confidence. _Confidence_ refers to the probability that the AI assigns to a prediction or classification. In the context of machine learning, it is a kind of scoring that measures how "confident" the AI is that the classification is correct. The higher the confidence scoring, the greater the certainty. For example, when analyzing an image, the AI may identify several features and assign a score to each signifying how confident it is that the feature is correct. The attributes list of an asset is not exhaustive. Assets that contain a rich set of features may be limited to a confidence threshold, such as the three most dominant features identified.

## Image features

Image features represent distinct and informative elements or patterns within an image that are used for analysis with [!DNL Insights]. The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Category                | Description                                                                                           | Example                                                                                                                                                                        |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Camera angle            | The location and angle of the camera relative to the subject.                                         |                                                                                                                                                                                |
| Subject distance        | The distance between the camera and the subject of an image.                                          | `close up`, `mid shot`, `long shot`                                                                                                                                            |
| Camera setting          | The configuration of the camera's controls to produce the image.                                      |                                                                                                                                                                                |
| Color and tone          | Evaluates colors used in image elements. Identifies one to three colors from a set of 40 pre-determined colors in the following image layers:<br>**[!UICONTROL Foreground colors]**—elements in the front layer of the image<br>**[!UICONTROL Background colors]**—elements in the back layer of an image<p>**[!UICONTROL Color temperature]** describes the general warmth or coolness of colors in the image.<br>Tone or temperature values: `warm`, `cool`, `neutral` | ![colors and cool tones](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Image style             | The visual treatment of an image.                                                                     |                                                                                                                                                                                |
| Lighting condition      | The type of light in an image.                                                                        |                                                                                                                                                                                |
| Objects                 | Identifies one or more items, entities, and elements that make up the image.                          | ![sunflower, plane, flower object](../../assets/category/image-objects.png){width="200" zoomable="yes"}                                                                        |
| Orientation             | The position of the image relative to the aspect ratio.                                               | `landscape`, `portrait`, `square`                                                                                                                                              |
| People                  | When at least one person is present, one or more attributes may describe the person or persons in the image. | ![woman person dancing](../../assets/category/image-people.png){width="200" zoomable="yes"}                                                                             |
| Photography genres      | Detects the subject and technique used to capture an image, such as `abstract` or `landscape` (not the same as landscape orientation). |           |
| Scenes                  | Detects the setting or environment depicted in an image.                                              |                                             |
| Tags                    | Detects objects, elements, and other image characteristics that do not fall under a specific classification. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Video features

Image features represent distinct and informative elements, sounds, or patterns within a video for analysis with [!DNL Insights]. The following table lists the video feature categories recognized by the GenStudio for Performance Marketing AI.

| Category            | Description                                                                                                  | Example                                                                                 |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Audio Genre         | When music is present, the video may receive one classification of music style, such as `electronic` or `classical`.       |          |
| Audio Genre Category| When music is present, the video may receive one broad classification of music genre, such as `acoustic` or `traditional`. |          |
| Audio Mood          | Describes the general atmosphere or tone of the audio, such as `relaxing` or `energetic`.                    |          |
| Audio Types         | When audio is present, the video may receive a tag for one or more audio types, such as `music` or `speech`. |          |
| Objects             | Identifies one or more items, entities, and elements that appear throughout the video.                       | ![objects in video](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Orientation         | The position of the video relative to the aspect ratio of the frame.            | `landscape`, `portrait`, `square`        |
| People              | When at least one person is present, one or more attributes may describe the person or persons in the video. |        |
| Scenes              | The setting or environment depicted in the video.                                                            |        |
| Styles              | Detects visual treatments applied to elements in the video, such as `matte` or `neon`.                       |        |
| Tags                | Detects objects, elements, and other video characteristics that do not fall under a specific classification. |        |

## Text features

Text features include counts for certain text elements, such as words, sentences, emojis, and classifications for semantics, emotion, and tone that are used for analysis with [!DNL Insights]. Text may also receive a readability score. Coming soon.

<!-- Not yet approved by legal

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description | Example |
|----------------------|-------------|--------|
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   |             |        |
| Narratives           | Text that represents an overarching situation, theme, or a story. Narratives can communicate values, purpose, or identity that resonates with consumers on many levels.   |        |
| Persuasion Strategies|             |        |
| Readability          |             |        |
| Tone of voice        | | |
-->
