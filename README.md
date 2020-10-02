# Horiseon Website - Refactoring & Accessibility

## Summary 
A refactor of the HTML/CSS for Horiseon Social Solution Services, Inc, a marketing company, was requested; the objective was to increase the website's accessibility. I have learned alot from the experienced engineers and professors on this subject, but know I needed to learn more about what accessibility is as wehow is it measured or quantitifed to hopefully provide users an easier experience engaging with online content.

## Horiseon's User Story
> As a marketing agency, we want a codebase that follows accessibility standards 
> so that our own site is optimized for search engines.

## Acceptance Criteria
Accessibility standards will be met when:
- Semantic HTML elements will be incorporated into the source code
- The structure of the HTML elements flow logically, independent of style or position of elements
- All image elements have a corresponding alt property
- Heading attributes fall in sequential order
- The title element is concise and descriptive

## Semantic Improvements
- Changed the class="header" div to a header block
- Changed the div within the header block to a nav block
- Changed all references to .header div selector to .header nav within the style.css file
- Fixed an anchor that pointed to a div ID that didn't exist, causing broken functionality
- The side-panel in the main body content was changed from div to the favorably-semantic 'aside'
- Wrapped the body's main content in a main block to designate what is main from what is inside the header, footer or hero-image areas

## CSS Cleanup & Consolidation
- Lines of CSS reduced by ~40%
	- Former number of lines: 200
	- Current number of lines: 120

- Consolidation of CSS classes:
	- Number of former class selectors: 31
	- Number of current class selectors:  17

## Primary Referential Sources
 - [Accessibility | MDN](https://developer.mozilla.org/en-US/docs/Web/Accessibility) | https://developer.mozilla.org/en-US/docs/Web/Accessibility
 - [WBC Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/) | https://www.w3.org/WAI/fundamentals/accessibility-principles/
