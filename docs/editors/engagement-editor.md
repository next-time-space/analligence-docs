---
title: "Engagement Editor"
---

# Engagement Editor

Engagement editor allows to assign the capture parameters for the segment we created on catalog.

Engagement will be created based on the target element and target actions. For this target element user clicking, or typing value, etc.

Wondering what all situations you can capture check out [More about engagement settings](#more-about-engagement-settings)

>Ex. In our example we created 2 segments one for browse page title and products div. So typically I need to capture when user clicks on the product div. So the target segment is product div. The browse title is silent segment which will be captured along with product div value.

## Create/Assign Engagement to segments

(1) In catalog page, click on the options icon in Action column, and select **Engagement Editor**

(2) Click on **Add engagement** icon from the segment list.

(3) Provide Engagement name, Description, remaining inputs are based on our engagement scenarios.

>In our example, I need to find when user click on the product pod get the product name/id.

>Then Interact by - Mouse; I click - Left button; Capture - This field Value; Value from - Child Element (because my selector is wide big, I need to capture product id sitting somewhere in the product pod); Child Identifier - selector of the product id.

<img alt="Analligence create engagement" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_create_engagement_1.png">

## More about engagement settings

It sounds engagement editor has too many options. So lets break it down and see options and descriptions.

### Interact By

Interact by could be mouse or keyboard, when you want to capture click events, go for mouse. When you want to capture typing event best example would be Type ahead, we need to go for keyboard. Both mouse and keyboard affect rest of engagement parameters.

### Mouse Interaction capture

Mouse capture can either happen for left click or right click. In I click option you can select which interaction we need to capture.

### Capture

Now the critical options starts, **Capture** has 3 options for mouse.

Situation | Capture | Value From|
------------ | -------------|-------------|
I need to capture what data in the element when user clicks on it | **This field value**|**Element Value**
I need to capture what data in the child element somewhere when user clicks on it. You will be asked to provide child element selector| **This field value**|**Child Element**
I need to capture what data in the attribute like _a href_ when user clicks on it. You will be asked to provide attribute name| **This field value**|**Element Attribute**
There maybe situation to capture another segment when user clicks on target segment in that case, make sure you created one more segment and select the target segment in options. | **Another Segment value**| **Element Value** or **Element Attribute**
Just need to check how many times this particular segment is clicked.| **Click Event**| NA


### Conditions

Conditions parameters will be useful to reduce the engagement noise.

Situation | Conditions |
------------ | -------------|
Capture only when element value is equals, grater than, less than, etc. You will be asked to provide the conditional operators and values| **Field Value**
Capture based on element value text count| **Field Value Text Count**
Capture data only when my URI contains particular query param or path param | URI

### Keyboard Interaction capture

Keyboard interaction capture will follow the same situations.

## Next Step

We need to work on formating the data we capture, example if we capture _href_ it's an URL, if you further want to capture particular query param/path param, it can be done using [Engagement formatter](/docs/editors/engagement-formatter) There are plenty of options available to trim the data capture. Check out [Engagement formatter](/docs/editors/engagement-formatter)