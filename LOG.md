# Daily Log

One short entry per study day. Newest at the top.
## Day 10: CSS Cascade and Specificity
- **Learned**:
  - Learned what the CSS Cascade is and how the browser decides which CSS declaration to apply when multiple rules target the same element.
  - Learned the basic specificity priority for normal author CSS selectors: ID > Class > Element > Universal.
  - Understood that ID selectors such as #title have higher specificity than class selectors such as .title.
  - Understood that class selectors have higher specificity than element selectors such as h1 or p.
  - Learned that the universal selector * targets all elements and contributes zero specificity.
  - Learned how to calculate CSS specificity using the format (ID, Class, Element).
  - Practiced calculating specificity for combined selectors such as #profile .card h2 = (1, 1, 1).
  - Practiced calculating specificity for #header #logo .active p span = (2, 1, 2).
  - Learned that when competing declarations have equal priority and specificity, the later rule in the stylesheet wins through source order.
  - Learned how inline CSS is written using the style attribute and why it wins over normal stylesheet declarations in the examples practiced.
  - Learned what !important does and how it gives a declaration priority over normal declarations in the same cascade context.
  - Understood that !important should be used sparingly because it can make CSS harder to maintain.
  - Reviewed the main Cascade decision factors: importance, origin and cascade layers, specificity, and source order.
  - Understood that the examples focused mainly on normal author CSS declarations, while the full CSS Cascade has additional rules.
- **Built / Practiced**:
  - Compared element, class, ID, and universal selectors to identify which declaration wins.
  - Practiced examples where ID selectors override class and element selectors.
  - Practiced equal-specificity examples and identified the last matching rule as the winner.
  - Compared inline styles with normal stylesheet declarations.
  - Practiced an example where color: green !important overrides a normal inline color: orange declaration.
  - Calculated specificity scores for individual and combined selectors.
  - Completed quick-check questions covering selector priority, source order, inline CSS, !important, and specificity calculations.
  - Completed a final code-output prediction exercise using element, class, and ID selectors.
- **Hard part**:
  - Remembering that the last CSS rule does not always win; specificity and other Cascade factors matter first.
  - Distinguishing ID specificity from class and element specificity.
  - Calculating specificity by counting IDs, classes, and elements separately.
  - Understanding that the universal selector contributes zero specificity.
  - Understanding when source order decides the winner.
  - Understanding the relationship between inline styles and !important.
  - Remembering that !important does not bypass every rule of the full CSS Cascade.
- **Tomorrow**:
  - Review Day 10 CSS Cascade and specificity concepts.
  - Continue the frontend learning roadmap with the next lesson.
  - Practice identifying winning CSS declarations and calculating specificity.
  - Apply the Cascade and specificity rules when styling real webpage components.

## Day 9: CSS Overflow and Content Handling**

- **Learned**:

  - Learned what CSS overflow is and why it is used when content exceeds an element's available space.
  - Learned the four main `overflow` values: `visible`, `hidden`, `scroll`, and `auto`.
  - Understood that `overflow: visible` allows content to extend outside its container.
  - Understood that `overflow: hidden` clips overflowing content without displaying scrollbars.
  - Learned that `overflow: scroll` provides scrollbars and `overflow: auto` displays them when needed.
  - Learned how `overflow-x` controls horizontal overflow and `overflow-y` controls vertical overflow.
  - Practiced combining `overflow-x: hidden` with `overflow-y: auto` to hide horizontal overflow while allowing vertical scrolling when needed.
  - Learned how `text-overflow: ellipsis` displays `...` when text is truncated.
  - Learned how `white-space: nowrap` keeps text on one line.
  - Understood that `text-overflow: ellipsis` is commonly combined with `white-space: nowrap` and `overflow: hidden`.
  - Reviewed how `width: 90%` and `max-width: 350px` work together to create a flexible card that does not exceed 350px.

- **Built / Practiced**:

  - Completed five quick-check questions covering overflow values, horizontal and vertical overflow, and text truncation; all five answers were correct.
  - Analyzed a scrollable project-card example using `overflow-y: auto` and `overflow-x: hidden`.
  - Analyzed a project title example using `white-space: nowrap`, `overflow: hidden`, and `text-overflow: ellipsis`.
  - Explained how responsive width and maximum width work together with overflow properties in a project card.

- **Hard part**:

  - Distinguishing `overflow: scroll` from `overflow: auto`.
  - Understanding the difference between horizontal overflow and vertical overflow.
  - Understanding that `overflow-x: hidden` clips overflowing content rather than intelligently truncating text.
  - Understanding that ellipsis indicates truncated text, not that more content is loading.
  - Understanding how `width: 90%` and `max-width: 350px` work together.

- **Tomorrow**:

  - Review Day 9 CSS overflow and text-truncation concepts.
  - Continue the frontend learning roadmap with the next lesson.
  - Practice applying CSS overflow properties when building layouts and components.

## Day 8: CSS Sizing Units

- **Learned**:
- Learned what CSS pixels (px) are and how they provide fixed sizing for properties such as width, height, and padding.
- Learned how percentages (%) work as relative values based on the relevant dimension of the parent or containing block.
- Practiced calculating percentage widths, including 50% of 800px = 400px and 75% of 800px = 600px.
- Learned how em relates to the parent font size when used for font-size.
- Practiced calculating em values, including 2em of a 18px parent font size = 36px and 1.5em of a 20px parent font size = 30px.
- Learned how rem (Root EM) relates to the root HTML font size.
- Practiced calculating rem values, including 1.5rem of a 16px root font size = 24px and 2rem = 32px.
- Understood the difference between em and rem: em uses the parent font size for font-size, while rem uses the root HTML font size.
- Learned how vh represents a percentage of the viewport height and how 100vh can be used for a full-height hero section.
- Practiced calculating vh values, including 50vh of an 800px viewport height = 400px and 25vh = 200px.
- Learned how vw represents a percentage of the viewport width.
- Practiced calculating vw values, including 25vw of a 1000px viewport width = 250px and 50vw of a 1200px viewport width = 600px.
- Compared fixed sizing (px), relative sizing (% / em / rem), and viewport-based sizing (vh / vw).
- Learned how width, max-width, and min-height can be combined to create flexible layouts.
- Understood that min-height sets a minimum height, so the element can be exactly that height or taller.
- **Built / Practiced**:
- Completed quick-check questions on px, %, em, rem, vh, and vw.
- Completed a five-question revision quiz with all five answers correct.
- Practiced analyzing a responsive profile-card CSS example using width: 90%, max-width: 400px, padding: 1.5rem, min-height: 50vh, and border-radius: 12px.
- Explained what each sizing property in the profile-card example does and corrected the meaning of min-height.
- **Hard part**:
- Remembering which reference size each relative unit depends on.
- Distinguishing em (parent font size) from rem (root HTML font size).
- Distinguishing viewport height (vh) from viewport width (vw).
- Calculating percentage, em, rem, vh, and vw values correctly.
- Understanding that min-height means at least the specified height, not exactly that height.
- Understanding how width: 90%, max-width: 400px, and min-height: 50vh work together in a responsive card.
- **Tomorrow**:
- Review Day 8 CSS sizing units and their differences.
- Continue the frontend learning roadmap with the next lesson.
- Practice applying sizing units in responsive HTML and CSS layouts.

## Day 7: CSS Variables and Reusable Styles
- **Learned**:
  - Understood what CSS variables (custom properties) are and why they help avoid repeating values.
  - Learned how to define reusable CSS variables inside the :root selector.
  - Practiced naming custom properties with the -- prefix, such as --primary-color.
  - Learned how to access CSS variables using the var() function.
  - Understood how changing one variable updates every CSS property that uses it.
  - Practiced creating reusable color variables for primary, background, card, and text colors.
  - Practiced creating reusable spacing variables for small, medium, and large spacing.
  - Learned how to reuse spacing variables for padding, margin, and gap.
  - Practiced creating typography variables for font sizes and font weights.
  - Reviewed common font-weight values: 400, 500, 600, and 700.
  - Learned how to create reusable border-radius variables.
  - Learned how to provide a fallback value inside var().
  - Understood how CSS variables can form a small reusable design system.
- **Built**:
  - A reusable CSS variable collection inside :root, organized into colors, spacing, typography, and border-radius categories.
  - A profile page using semantic HTML elements, including main, section, headings, paragraphs, and a button.
  - A profile card styled with reusable color, spacing, typography, and border-radius variables.
  - A profile avatar/logo using a .logo class and Flexbox.
  - A centered profile-card layout using Flexbox.
  - A reusable styling example for cards, headings, paragraphs, and buttons.
  - A Day 7 revision quiz covering :root, var(), reusable variables, fallback values, and custom-property naming.
- Hard part:
  - Understanding why :root is commonly used for globally reusable CSS variables.
  - Remembering that custom property names must begin with --.
  - Understanding how var() accesses a custom property.
  - Understanding how one variable can be reused by multiple elements and properties.
  - Choosing meaningful names for color, spacing, typography, and radius variables.
  - Understanding when and how to use fallback values in var().
  - Applying the variables consistently throughout the profile-card stylesheet.
- **Tomorrow**:
  - Begin Day 8 and learn CSS sizing units such as px, %, em, rem, vh, and vw.
  - Understand the differences between fixed, relative, and viewport-based units.
  - Practice using sizing units for responsive layouts.
  - Review CSS variables and the reusable profile-card design system.
  - Continue following the frontend learning roadmap one lesson and exercise at a time.

## Day 6: CSS Interactions, Transitions, Transforms, Shadows and Animations
- **Learned**:
  - Learned CSS pseudo-classes and how they style elements in different interaction states.
  - Practiced :hover for styling an element when the pointer is over it.
  - Practiced :focus for styling focused inputs, including using outline and border-color.
  - Practiced :active for styling an element while it is being activated or pressed.
  - Learned how CSS transitions make changes between states happen smoothly.
  - Practiced the transition shorthand using a property, duration, and timing function.
  - Learned the meaning of ease, ease-in-out, and transition durations such as 0.3s and 1s.
  - Understood the difference between transitioning a specific property and using transition: all.
  - Learned CSS transforms: translateX(), translateY(), scale(), and rotate().
  - Practiced positive and negative translation values to move elements right, left, down, and up.
  - Learned how scale() changes an element's size and how values below or above 1 affect its size.
  - Practiced combining multiple transform functions in one transform declaration.
  - Understood that a later transform declaration in the same CSS rule overrides an earlier one.
  - Learned how box-shadow adds depth and a shadow effect to an element.
  - Understood the horizontal offset, vertical offset, blur radius, spread radius, and color values in box-shadow.
  - Learned CSS animations using @keyframes, including from and to.
  - Practiced animation shorthand with an animation name, duration, timing function, and iteration count.
  - Learned that animations run once by default and that infinite repeats an animation continuously.
  - Learned animation directions: normal, reverse, alternate, and alternate-reverse.
  - Understood that transitions generally respond to a state change, while animations can run using defined keyframes.
- Built:
  - A button interaction exercise using :hover, :active, and :focus.
  - A button with a smooth background-color transition using transition: background-color 1s ease-in-out.
  - Transform exercises using translateX(), translateY(), scale(), and rotate().
  - A card hover effect combining translateY(-10px) and scale(1.05).
  - A styled card with a white background, 250px width, 20px padding, 10px rounded corners, and a soft shadow.
  - A card hover effect using translateY(-5px).
  - Animation examples that move a box from left to right and change its background color from red to blue.
  - An interactive profile-card styling exercise with a shadow, smooth transition, hover transform, and button hover color.
- **Hard part**:
  - Understanding the difference between :hover, :focus, and :active.
  - Understanding that a transition only animates the properties specified in the transition declaration.
  - Understanding the difference between translateX() and translateY(), and the direction of positive and negative values.
  - Understanding how scale() values change an element's size.
  - Combining multiple transform functions without writing separate transform declarations that override one another.
  - Understanding the parameters of box-shadow.
  - Understanding the difference between a transition and an animation.
  - Understanding how infinite and alternate affect animation playback.
- **Tomorrow**:
  - Begin Day 7 and learn CSS variables and reusable styles.
  - Practice defining and using custom properties with :root and var().
  - Apply reusable colors, spacing, and other values to CSS components.
  - Continue building and improving practical frontend components.
  - Review Day 6 interactions and animation concepts before moving forward.

# Day 5: CSS Responsive Design
- **Learned**:
  - Understood what responsive web design is and why webpages need to adapt to mobile, tablet, and desktop screen sizes.
  - Learned how CSS media queries work using @media.
  - Practiced using max-width for styles that apply up to a specified screen width.
  - Practiced using min-width for styles that apply from a specified screen width upward.
  - Learned how to combine media query conditions for mobile, tablet, and desktop layouts.
  - Understood mobile-first design: write the default styles for mobile, then progressively enhance the layout with min-width media queries.
  - Learned how responsive containers use percentage widths, max-width, and margin: 0 auto.
  - Learned how max-width: 100% and height: auto help images fit their containers while preserving their aspect ratio.
  - Reviewed the viewport meta tag: <meta name="viewport" content="width=device-width, initial-scale=1.0">.
  - Learned how to make a navigation bar responsive using Flexbox and media queries.
  - Reviewed flex-direction, justify-content, align-items, gap, and list-style.
  - Practiced responsive project-card layouts using CSS Grid.
  - Reviewed repeat(), auto-fit, minmax(), and gap for responsive Grid columns.
  - Reviewed element, class, ID, descendant, and grouped CSS selectors.
  - Reviewed the CSS Box Model, box-sizing: border-box, margin, and padding.
- **Built**:
  - A responsive personal portfolio mini-project using semantic HTML and CSS.
  - A page structure containing a header, navigation bar, home/hero section, About section, Projects section, and footer.
  - Navigation links connected to page sections using matching href fragment links and element IDs.
  - A Flexbox navigation bar with the logo on the left and navigation links on the right.
  - Styled home, About, and Projects sections with spacing, background colors, text alignment, and rounded corners.
  - A project-card layout using a shared Grid parent and responsive columns with repeat(auto-fit, minmax(200px, 1fr)).
  - Mobile navigation styling using a max-width: 600px media query.
  - Responsive layout practice for desktop, tablet, and mobile screen widths.
- **Hard part**:
  - Understanding when to use min-width versus max-width in media queries.
  - Understanding how mobile-first styles are overridden at larger breakpoints.
  - Understanding why a shared parent must be the Grid container when arranging multiple project cards into columns.
  - Matching CSS class selectors to the correct HTML class names.
  - Understanding how auto-fit and minmax() adapt Grid columns to the available width.
  - Avoiding repeated CSS by using grouped selectors for sections with shared styles.
  - Remembering to remove default list margin and padding when styling navigation.
  - Checking that responsive layouts do not cause horizontal overflow.
- **Tomorrow**:
  - Review Day 5 responsive design concepts.
  - Finish and test the portfolio mini-project at desktop, tablet, and mobile widths.
  - Verify that the navigation and project cards adapt correctly on smaller screens.
  - Continue following the frontend learning roadmap one lesson and exercise at a time.

## Day 4: CSS Grid

- **Learned:**
  - Understood what CSS Grid is and how it is used to create two-dimensional layouts with rows and columns.
  - Learned the difference between CSS Grid and Flexbox.
  - Understood the difference between a Grid container and Grid items.
  - Learned how to enable Grid using `display: grid`.
  - Practiced creating equal columns using `grid-template-columns`.
  - Learned how to create two equal columns using `1fr 1fr`.
  - Practiced creating three equal columns using `repeat(3, 1fr)`.
  - Learned how to create unequal columns using `1fr 2fr`.
  - Understood the CSS Grid `fr` unit and how it distributes available space.
  - Learned how to define rows using `grid-template-rows`.
  - Practiced creating fixed-height rows using `repeat(2, 100px)`.
  - Learned how `auto` adjusts row sizing based on content and available layout space.
  - Practiced adding spacing between Grid items using `gap`.
  - Learned the difference between `row-gap` and `column-gap`.
  - Learned how `repeat()` simplifies repeated Grid track definitions.
  - Practiced responsive Grid layouts using `auto-fit` and `minmax()`.
  - Understood how `minmax(200px, 1fr)` defines minimum and maximum track sizes.
  - Learned how `auto-fit` and `minmax()` work together to create responsive columns.
  - Practiced aligning Grid items using `justify-items` and `align-items`.
  - Understood the difference between horizontal and vertical alignment in Grid.
  - Learned how Grid layouts adapt to different container widths.

- **Built:**
  - A Grid layout with two equal columns and a 10px gap.
  - A Grid layout with three equal columns using `repeat(3, 1fr)`.
  - A Grid layout with two rows of 100px height.
  - A Grid layout using automatic row sizing with `grid-template-rows: auto`.
  - A responsive Grid layout using `repeat(auto-fit, minmax(200px, 1fr))`.
  - A Grid layout with centered items using `justify-items: center` and `align-items: center`.
  - A responsive skills layout containing Java, HTML, CSS, JavaScript, React, and Next.js.
  - Multiple CSS Grid exercises covering columns, rows, spacing, responsive layouts, and alignment.

- **Hard part:**
  - Understanding the difference between CSS Grid and Flexbox.
  - Understanding how Grid containers, Grid items, rows, columns, and cells work together.
  - Understanding how `1fr` and `2fr` distribute available space.
  - Understanding the difference between `grid-template-columns` and `grid-template-rows`.
  - Understanding the difference between fixed row heights and automatic row sizing.
  - Understanding how `repeat()` simplifies Grid column definitions.
  - Understanding how `auto-fit` and `minmax()` create responsive layouts.
  - Understanding how Grid items behave when the container width changes.
  - Understanding the difference between `justify-items` and `align-items`.
  - Practicing Grid syntax and correcting mistakes in CSS properties and values.

- **Tomorrow:**
  - Continue CSS fundamentals according to the roadmap.
  - Learn CSS Responsive Design and media queries.
  - Understand how webpages adapt to mobile, tablet, and desktop screen sizes.
  - Practice mobile-first design.
  - Learn how to create responsive layouts using CSS.
  - Practice making my existing HTML and CSS components responsive.
  - Review CSS Grid and Flexbox before moving forward.
  - Continue following the roadmap one lesson and exercise at a time.

---

## Day 3: CSS Fundamentals and Flexbox

- **Learned:**
  - Reviewed CSS fundamentals and how CSS connects to HTML.
  - Learned how to use external CSS files and link them using the `link` element.
  - Practiced CSS selectors: element selectors, class selectors, and ID selectors.
  - Learned the CSS Box Model: content, padding, border, and margin.
  - Practiced margin and padding shorthand values and their order.
  - Learned typography properties: `font-family`, `font-size`, `font-weight`, `line-height`, and `text-align`.
  - Practiced text colors, background colors, named colors, HEX colors, and RGB colors.
  - Learned CSS borders, border styles, and rounded corners using `border-radius`.
  - Understood the purpose of the HTML `div` element and how it groups elements inside a container.
  - Learned CSS display properties: `block`, `inline`, and `inline-block`.
  - Learned CSS positioning: `static`, `relative`, `absolute`, `fixed`, and `sticky`.
  - Practiced Flexbox basics using `display: flex`, `flex-direction`, `justify-content`, and `align-items`.
  - Learned Flexbox spacing and wrapping using `gap`, `flex-wrap`, and `align-content`.
  - Understood the Flexbox main axis and cross axis.
  - Practiced arranging elements horizontally, vertically, and across multiple rows.

- **Built:**
  - A basic HTML page styled using an external CSS stylesheet.
  - CSS selector practice using element, class, and ID selectors.
  - A styled card using width, background color, padding, border, and border radius.
  - A CSS display practice page using `inline-block`.
  - A positioning practice card with a badge placed in the top-right corner using relative and absolute positioning.
  - A Flexbox layout with Java, HTML, and CSS boxes arranged horizontally.
  - A Flexbox skills layout with Java, HTML, CSS, JavaScript, React, and Next.js boxes.
  - Multiple CSS exercises covering typography, colors, borders, positioning, spacing, and alignment.

- **Hard part:**
  - Understanding the difference between element selectors, class selectors, and ID selectors.
  - Understanding how padding, margin, border, and content contribute to the CSS Box Model.
  - Understanding the difference between `block`, `inline`, and `inline-block`.
  - Understanding how relative and absolute positioning work together.
  - Understanding why a parent container uses `position: relative` when positioning a child with `position: absolute`.
  - Understanding the difference between `justify-content` and `align-items`.
  - Understanding the Flexbox main axis and cross axis.
  - Understanding how `flex-wrap` moves items onto multiple rows.
  - Understanding the difference between `align-items` and `align-content`.
  - Practicing CSS syntax and correcting mistakes such as incorrect selectors and missing values.

- **Tomorrow:**
  - Continue CSS fundamentals according to the roadmap.
  - Learn CSS Grid and understand its layout structure.
  - Practice creating rows and columns using CSS Grid.
  - Continue practicing Flexbox and CSS layouts.
  - Build more practical HTML and CSS components.
  - Review today's CSS concepts before moving forward.
  - Continue following the roadmap one lesson and exercise at a time.

---

## Day 2: HTML Forms and Validation

- **Learned:**
  - Reviewed HTML document structure and semantic elements.
  - Practiced creating HTML forms using `form`, `label`, `input`, `textarea`, and `button`.
  - Understood the relationship between `id`, `for`, and `name` attributes.
  - Learned different input types: `text`, `email`, `password`, and `number`.
  - Practiced form validation using `required`, `minlength`, `maxlength`, `min`, `max`, and `step`.
  - Understood the difference between `minlength` and `min`.
  - Learned how radio buttons work and how the same `name` groups them together.
  - Learned how checkboxes allow users to select multiple options.
  - Practiced using `value` to identify selected form options.
  - Reviewed how browser validation prevents form submission when required fields are invalid.

- **Built:**
  - A contact form with name, email, age, and message fields.
  - A registration form with name, email, password, age, gender, skills, and message.
  - Radio buttons for selecting gender.
  - Checkboxes for selecting multiple skills, including Java, HTML, and CSS.
  - Form validation using appropriate HTML attributes.

- **Hard part:**
  - Understanding the difference between `minlength` and `min`.
  - Understanding how radio buttons use the same `name` to form a group.
  - Understanding how checkboxes allow multiple selections.
  - Understanding how `id`, `name`, and `value` work together in forms.
  - Understanding why a form cannot submit when one or more fields fail validation.

- **Tomorrow:**
  - Begin CSS fundamentals according to the roadmap.
  - Learn how CSS connects to HTML.
  - Practice CSS selectors and basic styling.
  - Start styling my semantic resume.
  - Continue following the roadmap one lesson and exercise at a time.

---

## Day 1: Semantic HTML

- **Learned:**
  - Frontend vs. backend and how they work together.
  - HTML fundamentals: tags, elements, attributes, and document structure.
  - Semantic HTML: `header`, `main`, `section`, and `footer`.
  - Headings, paragraphs, ordered and unordered lists.
  - Links, images, and the purpose of the `alt` attribute.
  - HTML forms: `form`, `label`, `input`, `textarea`, and `button`.
  - Form attributes: `id`, `name`, `for`, `type`, `required`, `placeholder`, `rows`, and `maxlength`.
  - Form `action`, GET vs. POST, and the basic browser-to-backend request flow.
  - Accessibility basics and the DOM parent-child tree structure.

- **Built:**
  - A semantic HTML resume with sections for personal information, skills, education, projects, and contact.
  - A contact form with name, email, message, labels, required fields, and a submit button.

- **Hard part:**
  - Understanding the difference between `head` and `header`, and `body` and `main`.
  - Understanding how `label`, `for`, `id`, and `name` work together in forms.
  - Understanding how HTML elements form a parent-child tree and how form data reaches a backend.

- **Tomorrow:**
  - Continue practicing HTML fundamentals.
  - Review and improve my semantic resume.
  - Practice HTML forms, attributes, and accessibility.
  - Continue following the roadmap before moving to CSS.