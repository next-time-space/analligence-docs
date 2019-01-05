---
title: "Engagement Formatter"
---

# Engagement Formatter

Engagement formatter allows to format data that's been captured from segment. Few cases be like, we want to consider case in sensitivity or merge two different engagement values and consider as one. Those after capture format can be done using Engagement Formatter.

Use the catalog page to navigate to engagement formatter

 <img alt="Analligence format data" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_format_data_1.png">

## Format capture value to UPPER or lower case

(1) Click on **Case Sensitive** tab on Engagement formatter.

 <img alt="Analligence format data case sensitive" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_format_data_case_sensitive.png">

(2) The situations are, when you capture user input in text field, user may do use lower, upper or mixed case. Now if we want to consider "Desktop" and "desktop" as one engagement value, we may have to format after capture value to either lower case or upper case.

(3) By default all engagements are user's case. It completely on how user submitting data. If you want to change the after captured value's case select the case you want to format and hit **save icon** on the top.

## Merge two engagement data

**Situation:** Sometimes we want to merge 2 different segment value as one value. 

>Ex, in our current example, we have data from breadcrumb and data from user clicked product, it makes sense to merge these 2 and see one output. Scenarios like 2 segments are considered as one engagement data, we would go for merging engagement.

**Restrictions:** There are some restriction for engagement merge. Both engagement should point to same segment and configuration for Interactions should be same. Otherwise your will get merge compatibility error.

(1) Click on **Merge Engagements** tab, the compatible engagements will be sorted next to each other. You can select two or more engagement of same kind and hit **Merge** icon from toolbar.

(2) Provide name for marge. If merging is compatible, engagement will be merged and it will show merge name on all engagements you selected.

 <img alt="Analligence format - Merge engagement" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_format_data_merge.png">

(3) To delete merge, select two or more engagement and hit **Delete** icon from toolbar.

## Post capture formatting

**Situation:** There will be some situations to format the captured data even more, if it's a long text, just get me the first 10 chars or if the captured data is an URL, get the exact query param value. So these problems can be addressed using post capture formatting.

(1) Click on **Post Capture Rules** tab and pick the engagement data you want to format click **Add** button in action column.

 <img alt="Analligence format - post capture" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_format_data_format.png">

 (2) Side bar will show many formatting options, select the option and provide required field value.

 (3) Engagement can accept more than one formatting, so add more format rules if required and the formatting will be performed the same order as you see in the list.

## Next Step

We are pretty much done with designing our segment and assigning engagements to segment. Next step will be create a build for our segment data. Check out [Build Space](/docs/editors/build-space)