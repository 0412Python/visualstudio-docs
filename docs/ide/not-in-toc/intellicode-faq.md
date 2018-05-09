---
title: IntelliCode FAQ
ms.date: 05/07/2018
ms.prod: visual-studio-dev15
ms.technology: vs-ide-general
ms.topic: conceptual
manager: douge
author: markw-t
ms.author: mwthomas
---
# Visual Studio IntelliCode FAQ

Thanks for your interest in Visual Studio IntelliCode! We've provided this short FAQ to hopefully answer some of the questions you may have.

## Q. What is Visual Studio IntelliCode?

At Build 2018, we announced Visual Studio IntelliCode, a new capability that enhances software development using AI. IntelliCode helps developers and teams code with confidence, find issues faster, and focus code reviews.

We showed an early view of how IntelliCode enhances the software development process in the following ways:

- Delivers context-aware code completions
- Guides developers to adhere to the patterns and styles of their team
- Finds difficult-to-catch code issues
- Focuses code reviews by drawing attention to areas that really matter

Developers can find more information and sign up for news and future private previews at [https://aka.ms/intellicode](https://aka.ms/intellicode).

## Q. What does Visual Studio IntelliCode enable customers to do?

Visual Studio IntelliCode is a range of capabilities that offers new productivity enhancements through artificial intelligence (AI).

Developers can [download an experimental extension](https://go.microsoft.com/fwlink/?linkid=872707) for Visual Studio 2017 version 15.7 and later. The extension provides enhanced IntelliSense that predicts the most likely correct API for the developer to use, rather than just presenting an alphabetical list of members. It uses the developer's current code context and patterns to provide this dynamic list. We'll update the extension with more capabilities in the coming months.

## Q: What makes “AI-assisted IntelliSense” powered by IntelliCode better than regular IntelliSense?

With IntelliCode, the completion list suggests the most likely correct API for a developer to use, rather than presenting a simple alphabetical list of members. It uses the developer's current code context, and patterns based on 2000 high quality, open-source projects on GitHub each with over 100 stars, to provide this dynamic list. The results form a model that predicts the most likely and most relevant API calls.

## Q: How good are the IntelliCode completion suggestions?

We’ve been using IntelliCode’s recommendations internally at Microsoft for some time, and believe the suggestions are useful. Ultimately, though, the proof will be in how useful these recommendations are to you as you code. We would love you to give the Visual Studio [IntelliCode extension](https://go.microsoft.com/fwlink/?linkid=872707) a try. Let us know how it works out for you and send us your feedback. We’ll also train our model based on what you pick in our recommendations, and we'll update the extension as the model improves.

> [!NOTE]
> None of your user-defined code is collected. See the question on [privacy](#privacy).

## Q. What's the future of IntelliCode?

We're exploring a wide range of ways to improve developer productivity using AI and other advanced techniques. At Build 2018, we showed an early view of some of the scenarios where we think AI could assist developers, but there are so many more! We're interested in learning from developers that experiment with what we've shown, so sign up for news and updates at [https://aka.ms/intellicode](https://aka.ms/intellicode).

## Q. How much does it cost?

We have no announcements regarding pricing at present.

## Q. When will IntelliCode be released?

IntelliCode's AI-assisted IntelliSense is currently in its first experimental preview. We'll continue to update the experimental extension, and we'll add further capabilities in the future. We have no schedule for a final release, but we welcome feedback from developers so we can deliver the best possible experiences. You can sign up for news and updates at [https://aka.ms/intellicode](https://aka.ms/intellicode).

## Q. Is this experience only available in Visual Studio and for C#?

The experience was shown at Build 2018 in Visual Studio 2017 on a C# codebase. However, we look forward to expanding IntelliCode to more languages and tools in the Visual Studio family in the future.

## Q. Is this experience only available in English?

IntelliCode is a preview extension today, and we are eager to understand how useful these capabilities are for a broad set of customers. When we take IntelliCode out of preview, we'll certainly consider which locale or language to support first, and how it is packaged, based on your feedback. 

## <a name="privacy"/> Q: What about privacy? Are you sending my code to the cloud? What customer data is being sent to Microsoft?

Developers are invited to experience Visual Studio IntelliCode today as an experimental preview extension. The purpose of the extension is to enable developers to test IntelliCode's capabilities and to provide feedback to the product team.

We capture some anonymized usage and error-reporting data from the extension to help improve the product. No user-defined code is sent to Microsoft, but we collect information about your use of the IntelliCode results. The data only includes open-source and .NET types and members that you selected from IntelliCode's suggested list. Developers can opt out of Visual Studio data collection, which turns off data collection for the IntelliCode extension too. From the menu bar, select **Help** > **Send Feedback** > **Settings**. In the **Visual Studio Experience Improvement Program** dialog, select **No, I would not like to participate** and then select **OK**.

The IntelliCode extension may periodically ask the developer to complete a survey, which again is anonymized. Users can sign up for news and a future private preview, but are not currently required to do so to use the experimental extension.

Future features may require access to a service, which will require sign-up. We'll publish more details when those features are ready for private preview.
