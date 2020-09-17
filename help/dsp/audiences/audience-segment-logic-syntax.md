# Syntax for Audience Segment Logic {#audience-segment-logic-syntax}

When you create reusable audiences, you can manually define segment logic using alphanumeric segment IDs and the following syntax:

* () to indicate a group
* || for OR
* && for AND
* ! for NOT (exclude)

>[!NOTE]
>
>* All specified segment groups are included unless they're preceded by ! (which excludes them).

For example, the following logic:

```
(X5vUk1cNvZxvBJ3jMjTt) || (sfvXrmQkk77PL5OtHpLH) && !(SMWSjTZFiy9hR1bKm1vw || x08UReA0IcP9HAJdcGVe)
```

means (in plain English)

```
INCLUDE Segment ID X5vUk1cNvZxvBJ3jMjTt OR INCLUDE Segment ID sfvXrmQkk77PL5OtHpLH AND EXCLUDE (Segment ID SMWSjTZFiy9hR1bKm1vw AND Segment ID x08UReA0IcP9HAJdcGVe)
```

>[!NOTE]
>
>In placement settings, you can use saved audiences either as audiences to explicitly target or as separate audiences to exclude from targeting. Make sure your segment logic reflects the purpose for which you will be using the audience.

>[!MORELIKETHIS]
>
>* [About Audience Management](audience-about.md)
>* [Create a Reusable Audience](audience-create-reusable-audience.md)
>* [Audience Settings](audience-settings.md)
>* [Available Third-party Data Providers](audience-third-party-data-providers.md)