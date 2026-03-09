---
title: Video Features
description: Learn about the video feature of attribute categories used in GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
TQID: https://experienceleague.adobe.com/s-8h3ODnNuRyebiDTLZGQORJzPnPOcPzQjIhWBmpk-c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
    internal-label: Generative AI
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
---
# Video features

Video features represent distinct and informative elements, sounds, or patterns within a video for analysis with [!DNL Insights]. These features help in categorizing and understanding the video content, enabling more accurate and detailed insights. By identifying various attributes such as audio mood, music genre, and objects, the AI can provide a comprehensive analysis of the video, aiding in better decision-making and strategy formulation.

## Audio detection

Audio detection in GenStudio for Performance Marketing involves analyzing the audio track of a video to identify various attributes. This detection process determines the overall mood of the audio by identifying the types of audio present, tagging specific genres or categories of music, and extracting keywords from speech. By understanding these audio elements, the AI can provide deeper insights into the video's content and context, enhancing the overall analysis and categorization process.

## Search video features

**To preview a video and hear a sample of the audio**:

1. In _[!DNL Insights]_, select the **[!UICONTROL Attributes]** view.

1. Change the table view by selecting **[!UICONTROL Video]**.

1. Select a feature from the **[!UICONTROL Attribute category]** list. For an audio example, select **Music genre**.

1. Select an attribute for a detailed view of videos that share that category.

   As an example, the `Music genre` category may have `electronic` as an attribute.

1. The _Attribute details_ page lists all the videos with this attribute. Hold your mouse pointer over any video in the list to start a video preview.

1. Toggle the **unmute** (located in the lower-left corner of a video preview) button and listen to the audio of the video preview.

The following table lists the video feature categories recognized by the GenStudio for Performance Marketing AI. The detected attributes list for an media content is not exhaustive. Media that contains a rich set of features may be limited to the three most dominant features identified by the AI.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Category            | Description                                                                                                  | Example                                                                                 |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Audio Mood          | Determines the overall emotional tone or atmosphere of the audio track, such as `calm`, `upbeat`, or `tense`. | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| Audio Types         | Tags the video with one or more audio content types present, such as `music` or `speech`.                         | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| Categories          | Classifies the video into one or more broad content categories.                                              | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| Music Category      | Broad classification of music genre when music is present in the video. Genre helps in identifying the general type of music, such as `contemporary` or `traditional` styles. | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| Music Genre         | Specific classification of music style when music is present in the video, which provides a more detailed identification of the music, such as `electronic` or `jazz`. | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| Objects             | Identifies one or more items, entities, and elements that appear in the video.                               | Values are too numerous, but some examples include: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap` |
| Orientation         | The alignment of the video in relation to its width and height. Detects whether it is wider than it is tall (landscape), taller than it is wide (portrait), or equal in width and height (square). | `landscape`, `portrait`, `square` |
| People              | When at least one person is present, one or more attributes may describe the person, or persons present in the video. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| Scenes              | Identifies the setting or environment within a video, providing context about where the video was made or the type of location depicted. | Values are too numerous, but some examples include: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`      |
| Styles              | Detects visual treatments applied to video elements, such as those used in After Effects or Lightroom.       | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| Tags                | Detects other video characteristics that do not fall under a specific classification. Tags provide additional context and metadata about the video.  | Values are too numerous, but some examples include: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`       |
