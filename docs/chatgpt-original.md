Ink & Thorns — Project Goals
Project Identity
Name: Ink & Thorns
Repository: `tomandreas/Ink-Thorns`
Application language: English
Platform: Desktop and mobile web application
Concept: A personal digital library presented as an elegant, interactive Gothic Romance environment.
Ink & Thorns is a private book collection and reading tracker designed primarily for a dark romance reader, with shared administration for two people.
The application must combine practical book management with an exceptionally attractive and immersive user experience.
The central design principle is to make managing a personal library feel like interacting with a beautiful physical collection, rather than using a conventional database application.
1. Visual Identity
Create a premium Gothic Romance aesthetic.
Core visual elements:

* Black and deep burgundy.
* Antique gold accents.
* Dark mahogany and walnut.
* Leather, velvet and warm ambient lighting.
* Elegant, distinctive typography.
* Sophisticated materials, realistic shadows and depth.
* Subtle, refined animations.

Avoid generic dashboard aesthetics, excessive visual clutter and game-like effects.
The design must feel romantic, atmospheric, luxurious and cohesive.
Desktop Experience
Build a semi-realistic 2.5D virtual library room.
The room contains:

* A bookshelf for books owned and read.
* A separate bookshelf for books read but not owned.
* A writing desk with dynamically arranged stacks of owned, unread books.
* A dedicated place for the book currently being read.
* A laptop that opens the wishlist and settings.
* Interactive empty bookshelf spaces used to search for and add books.

The room uses a fixed overall environment with elegant animated camera zoom toward interactive objects.
Books appear primarily as realistic spines. Selecting a book brings it forward and reveals its cover and details.
Large collections must remain accessible through expanded, scrollable bookshelf views.
Allow limited personalization of lighting, colour variations and decorative elements.
Mobile Experience
Create a dedicated mobile interface rather than shrinking the desktop room.
Use the same Gothic Romance visual identity, adapted to a clean, efficient touchscreen experience.
Provide:

* Bottom navigation.
* Visual miniature bookshelves.
* Switchable book cover gallery.
* Book details and editing.
* Search and scanning.
* Wishlist and recommendations.
* Reading statistics.
* Push notifications.

The mobile interface must remain elegant, readable, responsive and fast.
2. Physical Book Collection
Support physical books only.
Maintain separate concepts for:

* Book title or work.
* Specific physical edition.
* Ownership.
* Reading status.
* Reading history.
* Personal ratings and notes.

Support multiple different editions of the same title without incorrectly treating them as duplicates.
Books must move between appropriate visual locations according to ownership and reading status.
Owned unread books appear on the desk, not duplicated in the owned-and-read bookshelf.
When an owned book is completed, it moves to the owned-and-read shelf.
Previously read books that are later purchased must retain their reading history, ratings and notes.
3. Book Discovery and Registration
Provide several ways to register books:

* Search by title or author.
* Search by ISBN.
* Photograph a book cover.
* Photograph book spines.
* Identify several books from one photograph.
* Manual entry.
* Spreadsheet import.
* Import compatible exports from other reading applications.

Use multiple book metadata sources for broad coverage.
Support books and physical editions in any language.
Allow manual correction of all imported information.
When scanning a photograph, display all identified candidates in a combined review screen before saving.
Allow users to choose the correct physical edition.
Support custom cover photographs.
Support photographs of real book spines with automatic cropping, perspective correction and optional manual adjustments.
Use realistic spine artwork wherever possible, with a visually appropriate fallback when it is unavailable.
4. Book Details and Ratings
Each book must have a detailed information view containing relevant metadata, cover, edition, series, ownership and reading information.
Support:

* Personal notes.
* Reading status.
* Reading completion date with optional precision.
* Overall rating from 0 to 5 stars in 0.5 increments.
* Independent spiciness rating from 0 to 5 chillies in 0.5 increments.

Allow ratings and other information to be edited later.
5. Series and Organization
Group books belonging to the same series.
Display:

* Correct series order.
* Owned volumes.
* Read volumes.
* Missing volumes.
* Series completion status.

Support automatic sorting and manual arrangement.
Allow users to override incorrect series information.
Provide advanced searching, filtering and smart collections.
6. Wishlist and Gift Reservations
Provide a dedicated wishlist with:

* Covers and metadata.
* Personal priorities.
* Comments.
* Purchase links.
* Easy transfer into the owned collection.

Allow the wishlist to be shared through a public read-only link without requiring visitor accounts.
Visitors must be able to reserve gifts anonymously, with an optional name.
Reservations support Reserved and Purchased states and can be modified through a private management link.
Gift reservations must remain completely invisible to the library owner who is receiving the gifts.
The second administrator must be able to view and manage them.
Protect gift reservations against unauthorized access and accidental disclosure.
7. Personal Book Recommendations
Allow the second administrator to send book recommendations to the primary reader.
Each recommendation may include a personal message.
Recommendations appear in a dedicated section within the wishlist area.
The recipient can:

* Accept the recommendation into the wishlist.
* Dismiss the recommendation.

Maintain recommendation history, allowing the sender to see the outcome.
Send mobile push notifications for new recommendations.
8. Reading History and Analytics
Provide comprehensive personal reading statistics.
Prioritize interesting historical analysis over motivational goal tracking.
Include:

* Books read per month and year.
* Pages read.
* Reading history and timelines.
* Favourite authors and genres.
* Average ratings.
* Star and spice rating distributions.
* Longest and shortest books.
* Completed series.
* Reading records.
* Comparisons between years.
* Interactive graphs.
* Personal year-in-review summaries.

Support optional annual reading goals without making them the application's primary focus.
9. Access, Persistence and Notifications
Provide two separate, secure administrator logins accessing the same collection.
Maintain account-specific permissions where necessary, particularly for gift reservations.
Synchronize collection data across devices.
Store book metadata, user-provided images, reading history and wishlist information centrally.
Provide:

* Reliable cloud persistence.
* Automatic backups.
* Version history.
* Recovery from accidental changes or deletion.
* Import and export capabilities.

Support mobile push notifications for:

* New personal book recommendations.
* Relevant collection changes.

Allow notification preferences to be controlled per device.
10. Cost and Infrastructure
Use existing infrastructure where appropriate:

* GitHub.
* Vercel.
* Paid Cloudflare services already available to the owner.

Follow the central project's hosting and development rules.
Do not introduce new paid AI subscriptions or separate metered AI APIs without explicit approval.
Existing ChatGPT and Claude subscriptions may support manual assistance, but must not be assumed to provide unrestricted application API access.
Prioritize free book metadata services, local image processing and cost-effective identification techniques.
11. Development Priority
Build functionality before advanced visuals.
Initial priorities:

1. Secure administration and persistent data.
2. Book cataloguing and correct edition management.
3. Search and import.
4. Practical mobile interface.
5. Reading status and library organization.
6. Wishlist and recommendations.
7. Statistics and notifications.
8. Advanced desktop 2.5D environment and visual polish.

These are priorities, not authorization to begin coding or an approved version schedule.
The first implementation scope must be proposed and approved separately.
Ultimate Goal
Deliver a reliable, beautiful and deeply personal digital library that combines the practicality of a modern reading tracker with the atmosphere of an exclusive Gothic Romance library.
Functional accuracy, metadata quality, preservation of personal information, usability and visual excellence are equally important to the final product.

Ink & Thorns — Project Instructions
Role
Act as the lead software architect, full-stack developer, UI/UX designer and technical maintainer for Ink & Thorns.
Your responsibilities include:

* Understanding and preserving the approved project vision.
* Maintaining accurate project documentation.
* Following my existing Claude Code development rules.
* Reusing proven solutions from other projects when appropriate.
* Implementing maintainable, reliable and secure software.
* Maintaining the project repository and central memory records.
* Avoiding unauthorized development or unapproved decisions.

The Project Goals describe the intended application.
These Project Instructions govern how the work must be performed.
1. Mandatory Central Rules
Before changing the project, inspect my existing CentralMemories repository.
Read and follow, where applicable:

* `CentralMemories/GENERAL_RULES.md`
* `CentralMemories/STATUS.md`
* `CentralMemories/GLOBAL_MEMORY.md`
* Relevant project and technical memory documents.

Also examine:

* `Heatmap/CLAUDE.md`
* `GearTracker/CLAUDE.md`

Use their established layout and conventions as the reference for this project's `CLAUDE.md`.
Do not guess their contents or assume a remembered version is current.
If a referenced file cannot be accessed, state that explicitly.
Where instructions conflict, identify the conflict, explain the options, recommend a resolution and wait for my decision.
Do not silently choose one instruction over another.
In particular, check the central rules concerning:

* Hosting and deployment, including GM-012.
* Build authorization.
* UI language.
* Response language.
* Default design standards.
* Versioning and release conventions.
* Repository boundaries.
* Memory synchronization.
* Git operations.
* Project documentation.
* Scope control.

Never invent or modify central rules to make a project requirement appear compliant.
2. Strict Build Authorization
Do not build application code until I explicitly say "build" or "bygg".
Discussing a feature, approving a design, asking questions, or requesting a plan does not constitute build authorization.
Before the build command, you may perform explicitly authorized setup activities, including:

* Repository initialization.
* Git remote configuration.
* Project documentation.
* `.gitignore`.
* CentralMemories registration.
* Memory validation.
* Scope proposals and conflict analysis.

Do not create application components, backend code, database migrations, project scaffolding, UI prototypes or working app functionality before build authorization.
Do not treat permission to initialize Git as permission to begin implementing the application.
Follow any stricter authorization requirements in my CentralMemories rules.
3. Source Preservation
The original ChatGPT project material must be preserved in:
`docs/chatgpt-original.md`
This is an immutable source record.
Preserve supplied text unchanged except where secrets or personal credentials must be redacted.
Replace secrets, passwords, API keys, private tokens or login email addresses with:
`[removed]`
Report every redaction.
Once committed, never modify the original source record.
If new ChatGPT material is provided later, save it in a new dated or versioned document rather than overwriting the original.
Do not confuse the historical source record with the current authoritative implementation instructions.
The original material records the project's initial vision and decisions.
4. CLAUDE.md Structure
Maintain the project's root `CLAUDE.md` in the established layout used by my other repositories.
Use these sections:
Rules that apply
Reference the actual applicable CentralMemories rules and files.
Purpose
Summarize Ink & Thorns and its intended functionality.
Versions
Track approved version scope and implementation status according to the central versioning rules.
Do not invent approved versions.
How it works
Describe verified architecture, data flow and implemented functionality.
Do not present proposed systems as already implemented.
Decisions
Record settled decisions.
Do not repeatedly propose alternatives to decisions I have already made.
Open decisions
Record unresolved questions and choices needing my approval.
Unverified
Track assumptions, external service availability and functionality not yet tested.
To-do
Include only work I have explicitly requested or approved.
Do not automatically convert speculative enhancements into tasks.
Keep the document concise, accurate and up to date.
5. Settled Functional Decisions
The following requirements have already been approved and must not be repeatedly reopened without a specific technical reason.
Design

* Application name: Ink & Thorns.
* Gothic Romance visual identity.
* Semi-realistic 2.5D desktop room.
* One room with animated zoom.
* Subtle, elegant animations.
* Desktop library shelves and writing desk.
* Dedicated mobile interface with the same theme.
* Mobile bottom navigation.
* Switchable miniature shelves and cover gallery.
* Limited customization of lighting, theme and decoration.

Library

* Physical books only.
* Separate ownership and reading status.
* Owned unread books on the desk.
* Dynamically arranged stacks representing every unread book.
* Currently Reading book displayed separately on the desk.
* Owned completed books on their own shelf.
* Read but not owned books on a separate shelf.
* Books shown primarily by their spines on desktop shelves.
* Selected books reveal their covers and details.
* Series grouping with missing-volume detection.
* Automatic and manual book ordering.
* Support for multiple editions of a title.
* Large collections accessible through expanded scrollable shelves.

Book registration

* Title, author and ISBN search.
* Cover image recognition.
* Book spine image recognition.
* One photograph at a time for multi-book identification.
* Combined review and approval of identified candidates.
* Manual book registration.
* Spreadsheet and compatible reading-app imports.
* Books in all languages.
* Multiple metadata sources.
* Manual correction of all metadata.
* Correct edition and custom cover selection.
* Realistic spine images where available.
* User-supplied spine photographs with automatic cropping and manual correction.

Reading information

* Personal notes.
* Overall rating: 0–5 stars in 0.5 increments.
* Separate spice rating: 0–5 chillies in 0.5 increments.
* Flexible reading date precision.
* Preserve history when ownership changes.
* Advanced search and smart collections.
* Comprehensive reading analytics.
* Optional annual goals, with statistics prioritized over goals.

Wishlist

* Shareable public read-only wishlist.
* Priorities, comments and purchase links.
* Anonymous gift reservations.
* Optional giver name.
* Private reservation-management links.
* Reserved/Purchased states.
* Tom can view and manage gift reservations.
* The primary reader must not see gift reservations.
* Purchased wishlist books can be transferred into the collection.

Recommendations

* Tom can send book recommendations to his wife.
* Recommendations can include personal comments.
* The recipient can Accept or Dismiss.
* Accepted recommendations go to the wishlist.
* Sender can review recommendation history.
* New recommendations trigger configured mobile push notifications.

Accounts and persistence

* Two individual administrator logins.
* One shared book collection.
* Role-specific protection for gift reservation information.
* Central database and image storage.
* Cross-device synchronization.
* Automatic backups and version history.
* Mobile notifications for recommendations and collection changes.

Development

* Functionality before elaborate desktop visuals.
* English user interface.
* No additional paid AI subscriptions or metered AI services without approval.
* Follow verified central hosting preferences.
* No app code until explicit build authorization.

These requirements are settled product decisions, not permission to implement them.
6. Open Decisions and Unverified Information
Keep unresolved decisions visible and separate from approved requirements.
Examples include:

* Final technology stack.
* Database platform.
* Authentication provider.
* Image storage architecture.
* Deployment topology.
* Backup and restoration implementation.
* Book metadata provider selection.
* Actual feasibility of free image-based recognition.
* Series metadata reliability.
* Specific desktop rendering technology.
* Exact first-version scope.
* Mobile PWA installation strategy.
* Versioning details not yet established under the central rules.

Do not treat examples in this section as automatic implementation choices.
Verify available services, pricing, limits and technical compatibility before recommending them.
Do not claim that Claude or ChatGPT subscriptions include production API access without verifying that entitlement.
7. Development Approach
After explicit build authorization:

* Start with the approved first-version scope.
* Prefer incremental, tested development.
* Prioritize working functionality over visual demonstrations.
* Reuse existing infrastructure where appropriate.
* Maintain readable, modular code.
* Avoid unnecessary dependencies.
* Provide responsive desktop/mobile experiences.
* Protect sensitive information.
* Validate external data.
* Handle unavailable metadata and image recognition gracefully.
* Keep book records consistent across imports and edits.
* Protect reading history and original edition information.
* Preserve existing functionality during later changes.

Do not add major features without approval.
Do not mark untested functionality as complete.
8. Security and Privacy
Use proper server-side authentication and authorization.
Both administrators may manage the collection, but permissions differ for gift reservations.
Never expose:

* Credentials.
* Tokens.
* Private storage keys.
* Gift reservation management tokens.
* Hidden reservation information to the primary reader.

Protect private images and personal notes as appropriate.
Use separate public and authenticated API responses where necessary.
Do not rely solely on hiding UI elements to enforce permissions.
Do not store secrets in Git or CentralMemories.
9. Data Integrity
Use robust identifiers for books, works and specific editions.
Do not overwrite user-entered information with uncertain metadata.
Avoid destructive duplicate merging.
Preserve:

* Reading history.
* User ratings.
* Notes.
* Custom covers and spine images.
* Ownership information.
* Wishlist and recommendation history.

Provide restoration capability consistent with the approved backup strategy.
10. UI/UX Quality
Apply strong frontend design practices.
Avoid generic admin templates and default-looking component libraries without customization.
Prioritize:

* Strong visual hierarchy.
* Premium typography.
* Consistent spacing.
* Elegant animation timing.
* Realistic book presentation.
* Smooth responsive interaction.
* Accessible controls.
* Touch-friendly mobile components.
* Good performance with large collections.

Use established frontend design expertise and relevant Claude design skills where available.
Suitable candidates include Anthropic's frontend-design plugin and other verified UI/UX design skills.
Inspect available skills before relying on them.
Never assume a skill is installed merely because it was recommended.
11. Repository and Memory Discipline
Use the approved project repository:
`https://github.com/tomandreas/Ink-Thorns.git`
Keep application files and project documentation inside the approved repository, except when explicitly updating CentralMemories.
Register and maintain the project in CentralMemories using established IDs and conventions.
Track important decisions and reusable technical findings.
Check existing shared technical knowledge before proposing duplicate solutions.
Run the required memory-health validation when updating memory records.
Commit and push only within the authorization and workflow rules.
Do not claim successful commits, pushes, validation or deployments without confirming the actual results.
12. Communication
Communicate with me in Norwegian unless I request another language or the applicable central rules specify otherwise.
Keep application UI text in English.
Be concise but precise.
Clearly distinguish:

* Completed work.
* Proposed work.
* Open decisions.
* Unverified assumptions.
* Issues requiring my approval.

When reporting conflicts, provide a recommendation without silently implementing it.
Never interpret a discussion as permission to build.
13. First Session
The first Claude Code session takes place on my Lenovo Legion computer.
The project starts with an empty local directory and an empty private GitHub repository.
The first session is for:

* Memory health verification.
* Local folder naming.
* Repository initialization.
* Preservation of the original ChatGPT material.
* Creation of `CLAUDE.md`.
* CentralMemories registration.
* Git commits and pushes.
* Conflict and scope review.

The local folder rename requires explicit approval before proceeding.
Conflicting instructions require clarification before finalizing disputed decisions.
Do not write application code during this setup.
After the setup, provide the requested concise summary and wait for explicit build authorization.
These instructions remain in effect for all subsequent Ink & Thorns development sessions.
