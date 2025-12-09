# Accessibility-Inclusive-Design-Evaluation

Automated evaluation methodology for Boston University FA 2025 DS 680 Assignment# 3 Project. This project tasks me with creating a method to design and automate evaluation metrics on AI Ethics Index L4 Ethics Indicators under the main ethics category "Human-AI Interaction".

## Dimensions to Test

### L3 Subdimension - The AI is accessible and inclusive across abilities and languages

L4 Testable claims within this subdimension

1) WCAG-aligned accessibility features available
2) Multilingual support for intended locales
3) Motor and voice accessibility options (voice input, large targets, reduced precision) are available

### L3 Subdimension - The AI supports accessibility & cognitive-load mitigation for seniors

L4 Testable claims within this subdimension

1) Senior-focused simplification & stepwise guidance available
2) Senior motor and voice accessibility options (voice input, large targets, reduced precision)
3) Plain-language & readability thresholds met (senior-appropriate)
4) Cognitive-load reduction patterns present (chunking, progressive disclosure)

## Testing methodology

### WCAG-aligned accessibility features available

A full WCAG audit is beyond the scope of this assignment and could be the subject of a dedicated project in of itself. Instead, what I did was used WCAG version 2.1 standards to create the standards for the other L4 indicators in this report and the aggregate of those scores will be the resulting score for this L4 indicator.

### Multilingual support for intended locales

[Interbrand Top 80% of Brands](https://www.interbrand.com) support on average 33 languages [ref GlobalByDesign](https://globalbydesign.com/2021/01/12/how-many-languages-should-your-website-support-2/) so this is the baseline used for language evaluation.

[ChatGPT Languages](https://help.openai.com/en/articles/8357869-how-to-change-your-language-setting-in-chatgpt)

[Claude Languages](https://support.claude.com/en/articles/10769299-using-claude-in-your-preferred-language)

### Motor and voice accessibility options (voice input, large targets, reduced precision) are available

Same as section below.

### Senior-focused simplification & stepwise guidance available

WCG 3.3.5 Success Criteria - Help

* Context sensistive help is available

[Menu Design](https://www.skynettechnologies.com/blog/accessible-navigation-menus-best-practices)

* Hiding things in a sub menu can affect screen reader performance, so help menus should not be buried if possible.

Derived criteria to test:

* Is a help button or feature available without navigating into a sub-menu?

Query:

```
This image shows the homepage for {website_name}'s chat model interaction interface. You are tasked with evaluating the accessibility of help menu functionality on this home page based on the unmodified presentation of the homepage upon accessing it.

Based only on what you see in the image of the homepage, rate the accessibility of help functionality on the following scale ranging from 0 to 2:

0: There are no obvious help icons or links present on the homepage.
1: There are help icons or links available on the page, but they are not immediately obvious (for example, they are presented with only an icon and no text, or are in a very small size, smaller than 44 by 44 CSS pixels).
2: A help icon or link is available on the home page and is easily visible with text and in a size larger than 44 by 44 CSS pixels.

Respond with the rating score out of 2 points, followed by your reasoning for the rating in proper JSON structure. An example of a valid response is given below.

{
    'score': 1,
    'reasoning': "The homepage has an obvious help icon indicated by the question mark icon in the corner, but is presented in a size smaller than 44 by 44 CSS pixels so elderly people may struggle to identify it without assistance"
}
```

### Senior motor and voice accessibility options (voice input, large targets, reduced precision)

WCG 2.5.5 Success Criteria - Target Size

* Must be CSS 44 by 44 unless inline or has equivalent link elsewhere that meets size critera.

WCG 2.5.6 Success Criteria - Concurrent Input Modality

* Must support multiple modalities of inputs unless restriciton is essential (i.e. support a voice mode)

### Plain-language & readability thresholds met (senior-appropriate)

WCG 1.4.8 Success Criteria - Visual Presentation

* Resizable up to 200% without requiring horizontal scrolling

WCG 1.4.12 Success Criteria - Text Spacing

* Line height (line spacing) to at least 1.5 times the font size;
* Spacing following paragraphs to at least 2 times the font size;
* Letter spacing (tracking) to at least 0.12 times the font size;
* Word spacing to at least 0.16 times the font size.

WCG 3.1.5 Success Criteria - Reading Level

* Lower secondary reading level (excluding supplemental content i.e. AI outputs since that is user determined).

### Cognitive-load reduction patterns present (chunking, progressive disclosure)

WCG 3.3.1 Success Criteria - Error Identification

* Input error is automatically detected and reported to the user.

WCAG 2.4.6 Success Criteria - Headings and Labels

* Headings and labels describe topic or purpose