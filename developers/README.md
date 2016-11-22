#	Developers Accessibility Guides

### Goals
These guidelines will cover the major things you need to know in order for your products to be "production ready" and meet the minimum of standards in Section 508 and the Web Content Accessibility Guidelines 2.0. Level AA standards 

### Assumptions
This can include people who are blind, color-blind, or have low vision, those who are deaf or have hearing difficulties, people with mobility impairments which may be temporary or permanent, or people with cognitive disabilities. Design for people who are young old, power users, casual users, and those who just enjoy a quality experience.

### Requirements
| Title        | User Story           | Importance  | Notes |
| ------------- |:------------- |:-----|:-----|
| Use ARIA labels appropriately | Relevant ARIA roles for elements | 	Must Have | http://www.w3.org/TR/wai-aria-practices/#aria_ex |
| Keyboard Navigable | Check that all pages can be navigated via the keyboard and forms can be submitted using the keyboard. | Must Have | |
| Alternate Descriptions should be Provided for all Photos and Graphics  |When you add images (photos, graphics, logos) to your web page, you must also provide “alternative language tag” (ALT) descriptions for each one.  | Must Have |  |
|Presentation and Structure Needs to be Separate|Some users(i.e. color blind) input their own custom CSS stylesheets. To make this possible, the structure(html) of our pages need to be separate from our styles.(css) Choice of fonts, color, margins and size should be given to the hands of our users. | must have |  |
|Accessible Javascript|Some event handlers are dependent upon use of a mouse or keyboard. These are called device dependent event handlers. Other event handlers are device independent and are triggered by both the mouse and keyboard or by other means. | Should Have |  |
|Validate Your WebPages|Provide appropriate document structure. The topics listed here cover the majority of web accessibility issues, however, to ensure that your page complies with ADA/Section 508 Stardards, check it with a web accessibility checker.|Must Have |http://cynthiasays.com  http://wave.webaim.org  |
|Include a Skip-Links and Skip Navigation |This helps those using text reader technologies. Users should have a method that allows them to skip to navigation links. Users should also be able to skip to frequently visited areas of the page such as: the searchbox, main content, search filters, and navigation. A link to accessibility services page should also be used. This is will be used primarily as a backup for scenarios when something is broken on the page and we want users to get the accessibility page for help.|Must Have  |Options: Skip to Search, Skip to Main Content, Skip to Navigation, Skip to Accessibility Services  |
|Avoid using Frames|Frames are not inaccessible to modern screen readers, but they can be disorienting. If you use frames, give each frame a descriptive title attribute value. Keyboard shortcuts allow the reader to jump quickly between frames, so brief and descriptive titles are a necessity.|Must Have|  |
|Don't Use opacity: 0 to hide elements|Web browsers support many ways to hide elements — display: none (“hide and set width/height to 0”), visibility: hidden (“hide but take up the same space”), and aria-hidden=true (“screenreaders should ignore this”). Many of these are well-supported by modern screenreaders. But using opacity: 0 to hide things is well-supported by no one.|Must Have|  |
|	Does the tab order make sense (top-to-bottom, left-to-right)  | Run your website through a screen reader then look away. Does the tab order and navigation make sense? Would a blind user be confused navigating through your website? |Must Have  | 	http://www.nvaccess.org/, ChromeVox (Chrome extension), VoiceOver - Built into MacOS, Google Talkback (Android) |
|Jump Navigation the UVA Library  |Ensure that the UVA Library Jump Menu (for screen readers) contains a link to the following: Main Content, Main Navigation, Search Bar, and the Accessibility Services Page  |Must Have  |  |

### Automated QA For Developers
Below is a list of automated tasks that can be included in each project
| Task          | Documentation | 
| ------------- |:------------- | 
| one           |               | 
| two           |               |  
| three         |               |    
