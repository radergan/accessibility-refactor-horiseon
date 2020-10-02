# Horiseon Website - Refactoring & Accessibility
https://radergan.github.io/accessibility-refactor-horiseon/  | [Go to the site URL](https://radergan.github.io/accessibility-refactor-horiseon/)

## Summary 
A refactor of the HTML/CSS for Horiseon Social Solution Services, Inc, a marketing company, was requested; the objective was to increase the website's accessibility. Efforts were made to:
    - Add semantics to HTML structure
    - Add missing information that is important to accessibility, incl. alt and title information
    - Consolidate and organize style information
    - Identify and resolve issues with page load speed, presumably caused by enormous image sizes

### Horiseon's User Story
> As a marketing agency, we want a codebase that follows accessibility standards 
> so that our own site is optimized for search engines.

### Acceptance Criteria
Accessibility standards will be met when:
- Semantic HTML elements will be incorporated into the source code
- The structure of the HTML elements flow logically, independent of style or position of elements
- All image elements have a corresponding alt property
- Heading attributes fall in sequential order
- The title element is concise and descriptive


## Work
A small screenshot of the final product is shown to the right. The work was spread across three types of effort, to meet the acceptance criteria:<img align="right" width="400" src="./assets/images/horiseon-site-mockup.jpg" alt="Final Mockup: Horiseon Website">
1. Semantics
2. Alteration/consolidation of CSS (necessary, to point to new semantic HTML structures)
3. Performance

### Semantics
- Changed the class="header" div to a header block
- Changed the div within the header block to a nav block
- Changed all references to .header div selector to .header nav within the style.css file
- Fixed an anchor that pointed to a div ID that didn't exist, causing broken functionality
- The side-panel in the main body content was changed from div to the favorably-semantic 'aside'
- Wrapped the body's main content in a main block to designate what is main from what is inside the header, footer or hero-image areas

### Style Cleanup / Consolidation
- Lines of CSS reduced by ~40% 
	- Former number of lines: 200
	- Current number of lines: 120

- Consolidation of CSS classes:
	- Number of former class selectors: 31
	- Number of current class selectors:  17

### Performance Improvements
    - The size of the images being pulled in to the primary-content-section
      as well as the hero-image section were not conducive to loading the
      page in a reasonable amount of time. Compressing these allowed for
      a decent boost in pageload.

### Primary Referential Sources
 - [Accessibility | MDN](https://developer.mozilla.org/en-US/docs/Web/Accessibility) | https://developer.mozilla.org/en-US/docs/Web/Accessibility
 - [WBC Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/) | https://www.w3.org/WAI/fundamentals/accessibility-principles/
