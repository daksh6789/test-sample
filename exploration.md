    # Exploration Theme \- Curator Personas

    ---

    ## Persona 1: The Overwhelmed Discoverer

    **Age:** 25-32

    **Lifestyle:** City life, loves streaming, busy with work and friends, watches shows and listens to podcasts while traveling and on weekends, finds recommendations on social media

    **Key needs:** Finding what to watch tonight, cleaning up long watchlists, picking content that fits her free time, catching trending shows before it's too late, organizing scattered book and music lists

    **Pain points:** Can't decide what to watch, recommendations saved in too many apps, misses trending shows, forgets what she saved, spends more time browsing than watching

    ---

    ### Example Scenarios

    **Weekend movie night:** Sees a coworker post about a new movie on X.com, saves it. Opens Reddit (r/movies) to check reviews, adds it to IMDB watchlist. Checks Rotten Tomatoes score—looks good. Uses JustWatch to find it's on Prime Video, and starts watching it on Prime Video.

    **Finding something for the commute:** A friend shares a podcast link on WhatsApp, subscribes on Spotify Podcasts. Sees another podcast trending on X.com, subscribes to that too. A sibling recommends one on Apple Podcasts—adds that as well. Opens Audible to check 2 unfinished audiobooks.

    ---

    ### Apps for Persona 1

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :---- | :---- | :---- | :---- | :---- | :---- |
    | IMDB | Movies & TV | Most popular movie app—has her watchlist, ratings and trending | IMDB account export (CSV for watchlist/ratings) | Paid volunteers | Remove personal stories from reviews |
    | JustWatch | Movies & TV | Shows where to stream—stops searching Netflix, Prime, Hulu separately | Screenshots \+ manual export (no native export) | Paid volunteers | Generalize location to country level |
    | Rotten Tomatoes | Movies & TV | Quick scores (fresh/rotten)—helps decide in seconds | Screenshots \+ web scraping (no export feature) | Paid volunteers | Remove real stories from reviews |
    | Goodreads | Books | Her "to-read" list—50+ books she added but forgot about | Goodreads CSV export (My Books → Export) | Paid volunteers | Replace custom shelf names; remove friends list |
    | Amazon Kindle | Books | Her purchased ebooks—started reading but never finished | Amazon Data Request (GDPR) \+ Kindle highlights export | Paid volunteers | Remove highlights/notes content; replace device names |
    | Audible | Audiobooks | Listens while traveling—needs to match book length to travel time | Amazon Data Request (includes Audible) | Paid volunteers | Shift listening timestamps; remove bookmarks/clips |
    | Spotify | Music | Her main music app—playlists she created but never listens to | Spotify Data Download (Privacy Settings → Download) | Paid volunteers | Replace personal playlist names; remove social connections |
    | Spotify Podcasts | Podcasts | Half-finished episodes—needs to know which are worth completing | Spotify Data Download (same as music) | Paid volunteers | Shift listening timestamps |
    | Apple Podcasts | Podcasts | Secondary podcast app—some shows only on Apple, subscriptions split | Apple Privacy Data Request (privacy.apple.com) | Paid volunteers | Remove Apple ID email; strip device identifiers |
    | Reddit | Social | r/movies, r/television, r/books—where trending recommendations go viral | Reddit Data Request (Settings → Privacy → Request Data) | Paid volunteers | HIGH RISK: Anonymize subreddits; remove personal info from posts |
    | X.com | Social | Real-time buzz—catches what everyone is talking about | X/Twitter Data Download (Settings → Your Account → Download) | Paid volunteers | HIGH RISK: Strip EXIF from media; remove @mentions; blur photos |

    ---

    ## Persona 2: The Intentional Cultivator

    **Age:** 35-45

    **Lifestyle:** Careful about media choices, prefers learning over random browsing, goes deep on topics, tracks everything with notes, follows specific critics and writers

    **Key needs:** Building themed learning plans with films, books and music, tracking what was watched with personal notes, getting recommendations from trusted critics only, avoiding re-watching things, connecting content across different media

    **Pain points:** App recommendations feel random and generic, tools don't connect books/movies/music together, can't save notes properly, wants to explore topics fully but no tool helps, algorithms don't understand specific taste

    ---

    ### Example Scenarios

    **Deep dive into a director's work:** Reads a film essay on Substack about a director. Opens Letterboxd to create a watchlist of all their films in order. Uses TMDB to research connections between the movies. Watches one film per week, logs each on Letterboxd with personal notes. Finds a book about the director on Goodreads, adds to reading list. Searches Reddit (r/TrueFilm) for deeper discussion threads after finishing the series.

    **Building a themed reading and watching plan:** Wants to learn about a historical period through media. Opens Goodreads to find top-rated books on the topic, adds 5 to a custom shelf. Uses Letterboxd to find classic films from that era, creates a list. Makes a Spotify playlist of music from that time period. Subscribes to a Substack writer who covers the topic. Finds a podcast series on Pocket Casts about it. Spends 3 months going through everything, taking notes along the way.

    ---

    ### Apps for Persona 2

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    |-----|----------|------|------------------------|-------------|------------------------|
    | Letterboxd | Movies & TV | Film diary for logging, rating, and reviewing—follows specific critics | Letterboxd data export (Settings → Import & Export) | Paid volunteers | Remove diary entries with personal stories; anonymize followed users |
    | TMDB | Movies & TV | Deep research on films, cast, crew, and connections between movies | Screenshots + API access (public data) | Paid volunteers | — |
    | Rotten Tomatoes | Movies & TV | Critic reviews only—ignores audience scores, trusts professional critics | Screenshots + web scraping (no export feature) | Paid volunteers | Remove any saved reviews with personal content |
    | Goodreads | Books | Detailed tracking with reviews, notes, and custom shelves for themed reading | Goodreads CSV export (My Books → Export) | Paid volunteers | Remove personal review content; replace custom shelf names |
    | Amazon Kindle | Books | Highlights and annotations for deep reading and note-taking | Amazon Data Request (GDPR) + Kindle highlights export | Paid volunteers | HIGH RISK: Remove all highlights/notes content—contains personal thoughts |
    | Spotify | Music | Curated playlists for themed listening, full albums not shuffle | Spotify Data Download (Privacy Settings → Download) | Paid volunteers | Replace personal playlist names; remove social connections |
    | Pocket Casts | Podcasts | Power user podcast app—better organization, filters, and episode tracking | Pocket Casts data export (Settings → Privacy) | Paid volunteers | Shift listening timestamps |
    | Apple Podcasts | Podcasts | Secondary app for exclusive shows not on other platforms | Apple Privacy Data Request (privacy.apple.com) | Paid volunteers | Remove Apple ID email; strip device identifiers |
    | Substack | Newsletters | Follows trusted film critics, book reviewers, and writers | Screenshots + email export (no native export) | Paid volunteers | Remove email addresses; anonymize subscription list |
    | Reddit | Social | Niche subreddits like r/TrueFilm, r/literature for deeper discussions | Reddit Data Request (Settings → Privacy → Request Data) | Paid volunteers | HIGH RISK: Anonymize subreddits; remove personal info from posts |

    ---



    # Exploration Theme - Academic Concierge Personas

    ---

    ## Persona 1: The Scattered Student

    **Age:** 18-22

    **Lifestyle:** Living on campus or nearby, very busy with multiple classes, clubs, and a social life. Uses a laptop and phone constantly to stay updated on assignments.

    **Key needs:** Keeping track of many deadlines across different subjects, knowing exactly when and where exams are happening, finding study help when stuck on homework, and seeing grades as soon as they are posted.

    **Pain points:** Forgetting which app has which homework, missing a message from a teacher because it was sent on a platform they don't check often, and feeling overwhelmed by too many different websites for one single degree.

    ---

    ### Example Scenarios

    **Preparing for Midterms:** Gets an alert on **Canvas** that a practice exam is ready. Opens **Piazza** to see what other students are asking about the test. Realizes they don't understand a math topic, so they search for a video on **Khan Academy** to learn it quickly. Later, they check **Gradescope** to see the feedback on their last quiz so they don't make the same mistakes.

    **Managing a Busy Week:** On Monday morning, checks **Google Classroom** for the weekly reading list. Uses **PeopleSoft** to check their official class schedule and room numbers. Submits an essay to **Turnitin** to make sure it is ready to turn in. Ends the day by checking **Ed Discussion** for any last-minute changes to the lab session.

    ---
        
    ### Apps for Persona 1

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **Canvas** | LMS | Main hub for all course materials, grades, and deadlines. | Canvas "Download my Data" feature in settings. | Paid volunteers | Remove teacher comments and student names from peer reviews. |
    | **Piazza** | Miscellaneous | The place to ask questions and talk to classmates. | Manual copy or screenshot of "My Posts" and "Followed Threads". | Paid volunteers | Mask names of other students in discussion threads. |
    | **Gradescope** | Miscellaneous | Where paper tests and coding projects are graded. | Exporting graded assignments as PDF or CSV. | Paid volunteers | Remove handwritten names or ID numbers from scans. |
    | **Google Classroom** | LMS | Used for simpler classes or small group projects. | Google Takeout (Classroom specific data). | Paid volunteers | Remove school email and specific classroom codes. |
    | **PeopleSoft** | Miscellaneous | Used for the "official" school schedule and final grades. | Screenshots of the "My Schedule" and "Grades" pages. | Paid volunteers | Hide official Student ID number and birthdate. |
    | **Turnitin** | Miscellaneous | Used to check if an essay is original before turning it in. | Downloading the "Digital Receipt" and similarity report. | Paid volunteers | Remove the actual text of the essay to protect student work. |
    | **Ed Discussion** | Miscellaneous | Newer board for class chats and announcements. | Manual export or screenshots of user profile activity. | Paid volunteers | Anonymize the names of professors and other students. |
    | **Khan Academy** | Content Website | Uses this for extra help with hard science or math topics. | Profile data export from "Settings". | Paid volunteers | Generalize the "Coach" or "Teacher" names listed. |

    ---

    ## Persona 2: The Independent Learner

    **Age:** 25-40

    **Lifestyle:** Works a full-time job while taking online courses to get a better position. Very disciplined, spends evenings and weekends learning new skills.

    **Key needs:** Finding the best videos and courses for a specific job skill, tracking certificates of completion, managing a syllabus that isn't connected to a physical school, and navigating complex professional portals.

    **Pain points:** Finding high-quality content without wasting time on "junk" videos, struggling to connect what they learn on one site (like Coursera) with another (like Udemy), and keeping a clear schedule when there is no teacher to remind them.

    ---

    ### Example Scenarios

    **Upskilling for a Promotion:** Decides to learn "Data Science" to get a raise. Starts a professional certificate on **Coursera**. Finds a specific coding trick on **YouTube** that wasn't explained well in the course. Purchases a deeper, hands-on project course on **Udemy** to practice. Tracks all these different "syllabuses" in a personal calendar to stay on track.

    **Taking a Formal Online Class:** Enrolls in a single university course through a portal like **Banner First**. Uses **Moodle** to download the syllabus and watch recorded lectures. Uploads their final project to **Blackboard Learn** and waits for the official grade to appear in the portal.

    ---

    ### Apps for Persona 2

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **Coursera** | Content Website | Main place for professional certificates and uni-backed courses. | Requesting a "Personal Data Report" from account settings. | Paid volunteers | Remove workplace or employer names if linked. |
    | **Udemy** | Content Website | Used for quick, specific technical skills or hobby learning. | Exporting "Purchase History" and "Course Progress". | Paid volunteers | Mask payment details and full billing address. |
    | **YouTube** | Content Website | Best for quick tutorials and "how-to" academic videos. | Google Takeout (YouTube watch and search history). | Paid volunteers | Filter out non-educational videos from the history. |
    | **Moodle** | LMS | Often used by international schools or tech-heavy courses. | "Export My Data" tool found in the Moodle profile. | Paid volunteers | Remove IP addresses and specific login locations. |
    | **Blackboard Learn** | LMS | Popular platform for older universities and adult education. | Screenshots or manual download of "My Grades" and "Tasks". | Paid volunteers | Remove specific university name and professor names. |
    | **Banner First** | Miscellaneous | The back-end portal for registration and official records. | Screenshots of the student profile and transcript page. | Paid volunteers | REDACT all financial aid and social security info. |

    ---

    # Advice Theme - Career & Branding Personas

    ---

    ## Persona 1: The Fresh Graduate

    **Age:** 21-25

    **Lifestyle:** Just finished college, first real job hunt, limited work experience.

    **Key needs:**
    * Building a resume from scratch and optimizing applications.
    * Applying to entry-level jobs via job search automation.
    * Preparing for first interviews and portfolio building.
    * Creating a professional LinkedIn presence.

    **Pain points:** No work experience to highlight, doesn't know how to write a resume, overwhelmed by job boards, no professional network yet, unsure how to present skills.

    ---

    ### Example Scenarios

    **First Job Hunt:** Opens **Microsoft Word** to draft a first resume using a college project as the main highlight for application optimization. Searches for entry-level roles on **Indeed** and **LinkedIn** to start job search automation. Uploads the resume to **LinkedIn** and optimizes the profile headline to attract recruiters. Uses **PowerPoint** to organize images and code snippets from a senior project to build a digital portfolio for upcoming interviews.

    **Interview Preparation:** Receives an email for an initial screening at a tech startup and begins interview prep. Opens **LinkedIn** to research the interviewer's background and company culture for profile optimization. Uses **Microsoft Word** to write down answers to common interview questions. Reviews a project presentation in **Office Suite** to ensure they can explain their technical contributions clearly during the video call.

    ---

    ### Apps for Persona 1

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **LinkedIn** | Career & Branding | Main platform for job search, networking, and profile optimization. | Account data export (Settings -> Data Privacy). | Paid volunteers | Remove private messages and connection names. |
    | **Microsoft Word** | Office Suite | Essential for resume and cover letter creation and optimization. | Local file upload (PDF/DOCX). | Paid volunteers | Redact phone number and physical address. |
    | **PowerPoint** | Office Suite | Used for building a visual portfolio or project showcase. | Local file upload. | Paid volunteers | Remove photos of other students or faculty. |
    | **Indeed** | Recruiting | Primary recruiting website for entry-level role discovery. | Screenshots of "Applied" and "Saved" folders. | Paid volunteers | Mask specific recruiter contact details. |

    ---

    ## Persona 2: The Mid-Career Switcher

    **Age:** 35-50

    **Lifestyle:** Established career but looking to change industries or roles, has significant experience to leverage.

    **Key needs:**
    * Repackaging experience and optimizing resumes for a new industry.
    * Rebuilding LinkedIn presence and professional branding.
    * Networking strategically and automating the job search in a new field.
    * Preparing for interviews in an unfamiliar domain.

    **Pain points:** Experience doesn't directly translate, feels overqualified for entry roles but underqualified for senior roles in new field, ageism concerns, network is in old industry.

    ---

    ### Example Scenarios

    **Industry Transition:** Reads an industry report on **LinkedIn** about a growing sector to assist in job search automation. Uses **Microsoft Word** to rewrite a 10-year-old resume, focusing on transferable leadership skills for application optimization. Reaches out to three new contacts on **LinkedIn** for strategic networking and profile optimization. Tracks all outreach and new industry terminology in a **Microsoft Excel** sheet to stay organized.

    **Strategic Networking:** Identifies a target company and checks **LinkedIn** for any mutual connections to optimize their presence. Updates their professional bio in **Office Suite** to reflect their new career direction. Attends a virtual industry seminar and adds the speakers on **LinkedIn** with a personalized note. Prepares a "Bridge Story" in **Microsoft Word** that explains how their past experience solves problems during interview prep.

    ---

    ### Apps for Persona 2

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **LinkedIn** | Career & Branding | Used for strategic networking, industry research, and profile optimization. | LinkedIn Data Archive request. | Paid volunteers | Anonymize previous company names if needed. |
    | **Microsoft Word** | Office Suite | Repackaging career history into a modern format for resume optimization. | Local file upload. | Paid volunteers | Remove specific graduation years to mitigate bias. |
    | **Microsoft Excel** | Office Suite | Used as a personal CRM to track networking and target companies. | Local file upload. | Paid volunteers | Remove specific salary or contact phone numbers. |
    | **Naukri / Glassdoor** | Recruiting | Recruiting websites used for salary research and company reviews. | Screenshots of saved jobs and salary insights. | Paid volunteers | Mask current employer name in search history. |

    ---


    ---



    # Advice Theme - Personal Finance: Budgeting & Expense Tracking Personas

    ---

    ## Persona 1: The Single Professional

    **Age:** 25-35

    **Lifestyle:** Single or no dependents, managing only own finances, building financial foundation.

    **Key needs:**
    * Creating first budget and tracking spending habits.
    * Monitoring credit score and understanding credit health.
    * Identifying wasteful subscriptions and recurring charges.
    * Building an emergency fund and establishing savings goals.

    **Pain points:** Never learned to budget properly, impulsive spending habits, doesn't know where money goes each month, surprised by credit card bills, too many forgotten subscriptions draining the account.

    ---

    ### Example Scenarios

    **Creating a first budget:** Gets surprised by $800 credit card bill on **Chase Mobile**, links all accounts to **Mint**—dining out is 3x higher than expected. Creates strict categories in **YNAB**, checks score on **Credit Karma**. Transfers $200 to savings via **Bank of America**, sets spending alerts in **Chase Mobile** to avoid future surprises.

    **Subscription audit:** Notices balance lower than expected on **Chase Mobile**, downloads **Rocket Money (Truebill)** which finds 12 subscriptions totaling $180/month. Cancels 3 forgotten services, checks **Apple Subscriptions** and **Google Play** for duplicates. Confirms cancellations cleared in **Mint**, checks **Credit Karma** to see if score improved.

    ---

    ### Apps for Persona 1

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **Mint** | Budgeting | Primary app for automatic expense tracking and budget creation. | Intuit account data export (Settings -> Privacy). | Paid volunteers | Remove linked account numbers; mask transaction merchants with personal info. |
    | **YNAB** | Budgeting | Zero-based budgeting for intentional spending and savings goals. | YNAB data export (Settings -> Export Budget). | Paid volunteers | Remove specific payee names; anonymize category labels if personal. |
    | **Credit Karma** | Credit Monitoring | Free credit score monitoring and credit health tracking. | Credit Karma data export (Account Settings -> Download Data). | Paid volunteers | REDACT full SSN; remove specific creditor account numbers. |
    | **Rocket Money (Truebill)** | Subscription Tracking | Identifies and cancels forgotten subscriptions automatically. | Screenshots + manual export of subscription list. | Paid volunteers | Mask subscription service usernames; remove linked payment methods. |
    | **Chase Mobile** | Banking | Primary bank app for account management and spending alerts. | Chase data export (Statements + Transaction History CSV). | Paid volunteers | REDACT account numbers; remove check images and wire details. |
    | **Bank of America** | Banking | Secondary bank account for savings and transfers. | BofA data export (Statements + Activity CSV). | Paid volunteers | REDACT account numbers; remove Zelle contacts. |
    | **Copilot Money** | Budgeting | Clean dashboard for tracking all accounts in one place. | Screenshots + manual export. | Paid volunteers | Remove linked account nicknames; mask net worth totals. |
    | **Apple Subscriptions** | Subscription Tracking | Manages App Store and Apple service subscriptions. | Apple Privacy Data Request (privacy.apple.com). | Paid volunteers | Remove Apple ID email; strip device identifiers. |
    | **Google Play** | Subscription Tracking | Manages Android app subscriptions and payments. | Google Takeout (Google Play data). | Paid volunteers | Remove Google account email; mask payment methods. |

    ---

    ## Persona 2: The Family Budgeter

    **Age:** 35-50

    **Lifestyle:** Managing household finances for family with kids, multiple income sources and expenses across various accounts.

    **Key needs:**
    * Tracking household expenses across multiple categories and accounts.
    * Managing joint accounts and coordinating spending with spouse.
    * Budgeting for kids' activities, education, and unexpected expenses.
    * Planning for big expenses like vacations, home repairs, and college savings.

    **Pain points:** Money arguments with spouse about spending, kids' expenses add up fast and unpredictably, hard to track who spent what, complex finances spread across multiple bank accounts, balancing saving vs spending for the family.

    ---

    ### Example Scenarios

    **Household budget coordination:** Argument with spouse about overspending—opens **Quicken** to check, kids' expenses are 40% over budget. Sets up **Honeydue** for real-time alerts, creates shared goals in **YNAB**. Checks **Wells Fargo** joint checking, reviews **Capital One** rewards. Cousin asks to split vacation costs, sets up group in **Splitwise**.

    **Planning for big expenses:** Daughter's summer camp costs $2,500—opens **Mint** to check savings, only $800 available. Compares rates on **Marcus by Goldman Sachs** vs **Ally Bank**, opens savings bucket in Marcus. Sets up automatic transfers from **Wells Fargo**, tracks progress in **YNAB**. Shares tracker with spouse via **Google Sheets**, confirms **Fidelity** 529 won't be affected.

    ---

    ### Apps for Persona 2

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **Quicken** | Budgeting | Comprehensive household finance management with multi-account tracking. | Quicken data export (File -> Export -> QFX/CSV). | Paid volunteers | Remove investment account details; mask property valuations. |
    | **YNAB** | Budgeting | Shared budget creation for couples with goal tracking. | YNAB data export (Settings -> Export Budget). | Paid volunteers | Anonymize memo fields; remove specific child/dependent names. |
    | **Mint** | Budgeting | Automatic categorization of family expenses across accounts. | Intuit account data export. | Paid volunteers | Mask merchant names with family member identifiers. |
    | **Honeydue** | Couples Finance | Shared expense tracking designed for couples with split bills. | Screenshots + manual export of shared transactions. | Paid volunteers | Remove partner's name and profile photo; mask couple-specific categories. |
    | **Marcus by Goldman Sachs** | Banking/Savings | High-yield savings accounts for specific family goals. | Marcus account statements (PDF download). | Paid volunteers | REDACT account numbers; remove beneficiary names. |
    | **Wells Fargo** | Banking | Primary joint checking and savings accounts for household. | Wells Fargo data export (Statements + Activity). | Paid volunteers | REDACT account numbers; remove joint holder names. |
    | **Capital One** | Credit Cards | Family rewards credit card for household purchases. | Capital One data export (Statements CSV). | Paid volunteers | Remove authorized user names; mask specific merchant details. |
    | **Splitwise** | Expense Splitting | Tracks shared expenses with extended family and friends. | Splitwise data export (Account -> Export). | Paid volunteers | Anonymize group member names; remove profile photos. |
    | **Ally Bank** | Banking/Savings | Online high-yield savings for comparison shopping rates. | Ally data export (Statements PDF). | Paid volunteers | REDACT account numbers; remove beneficiary info. |
    | **Fidelity** | Investing/529 | 529 college savings plan for children's education. | Fidelity data export (Statements + Portfolio). | Paid volunteers | Remove beneficiary child names; mask specific contribution amounts. |
    | **Google Sheets** | Productivity | Shared family budget tracking and planning spreadsheets. | Local file upload. | Paid volunteers | Remove family member names from sheets; anonymize custom labels. |

    ---



    # Advice Theme - Personal Finance: Tax Preparation Personas

    ---

    ## Persona 1: The Salaried Employee

    **Age:** 25-40

    **Lifestyle:** Full-time employee with taxes withheld from paycheck, straightforward tax situation, single or married with simple returns.

    **Key needs:**
    * Filing annual tax return accurately and on time.
    * Maximizing standard deduction and available credits.
    * Understanding pay stub deductions and W-2 information.
    * Getting refund processed quickly with direct deposit.

    **Pain points:** Procrastinates until deadline, confused by tax jargon and form numbers, unsure if using the right filing status, worried about making mistakes that trigger audits, doesn't know what deductions and credits are available.

    ---

    ### Example Scenarios

    **Annual tax filing:** Downloads W-2 from **ADP**, imports into **TurboTax**—got married and bought home this year. Grabs 1098 from **Rocket Mortgage**, checks **Chase** for 1099-INT interest. Double-checks refund on **Credit Karma Tax**, files with direct deposit to **Bank of America**. Tracks refund on **IRS2Go**, saves return to **Google Drive**.

    **Understanding paycheck deductions:** Paycheck after raise is lower than expected—downloads stub from **Workday**, checks **ADP** for breakdown. Uses **H&R Block Tax Calculator** to estimate year-end impact, compares with last year in **TurboTax**. Updates W-4 through **Workday**, sets **Google Calendar** reminder to verify.

    ---

    ### Apps for Persona 1

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **TurboTax** | Tax Preparation | Most popular tax software with guided interview and automatic W-2 import. | Intuit account data export + prior year returns (PDF). | Paid volunteers | REDACT full SSN; remove employer EIN; mask bank account for refund. |
    | **H&R Block** | Tax Preparation | Alternative tax software with in-person support option. | H&R Block account data export (PDF returns). | Paid volunteers | REDACT SSN and dependent SSNs; remove specific employer names. |
    | **IRS2Go** | Tax Tracking | Official IRS app for refund tracking and payment status. | Screenshots of refund status screens. | Paid volunteers | REDACT any visible SSN digits; remove specific refund amounts if requested. |
    | **FreeTaxUSA** | Tax Preparation | Free federal filing option for simple returns. | PDF download of completed returns. | Paid volunteers | REDACT all SSNs; remove bank routing numbers. |
    | **Credit Karma Tax** | Tax Preparation | Free tax filing with refund comparison. | Credit Karma data export (Account Settings). | Paid volunteers | REDACT SSN; remove linked bank accounts. |
    | **ADP** | Payroll | Employer payroll portal for W-2 access and pay stubs. | Screenshots + PDF download of pay stubs and W-2. | Paid volunteers | REDACT SSN and employee ID; remove employer name. |
    | **Workday** | Payroll/HR | Employee portal for tax documents and W-4 updates. | Screenshots + PDF export. | Paid volunteers | REDACT employee ID; remove manager names. |
    | **Rocket Mortgage** | Mortgage | Mortgage portal for 1098 interest statements. | PDF download of annual statements. | Paid volunteers | REDACT loan numbers; remove property address. |
    | **Google Drive** | Storage | Cloud storage for tax document organization. | Local file upload of tax folder. | Paid volunteers | Remove folder names with personal identifiers. |

    ---

    ## Persona 2: The Self-Employed Filer

    **Age:** 35-55

    **Lifestyle:** Freelancer, contractor, or small business owner with complex tax situation including multiple income sources and business deductions.

    **Key needs:**
    * Tracking business expenses year-round with proper categorization.
    * Filing quarterly estimated taxes to avoid penalties.
    * Managing multiple 1099s from various clients.
    * Maximizing business deductions and separating personal from business finances.

    **Pain points:** Quarterly taxes are confusing and easy to miss, receipts scattered everywhere (email, photos, paper), scared of audits due to business deductions, never sure if paying enough estimated tax, tax bill surprises at year end, constantly mixing personal and business expenses.

    ---

    ### Example Scenarios

    **Quarterly tax preparation:** Q3 taxes due in 5 days—opens **QuickBooks Self-Employed** to review, finds missing payments in **PayPal** and **Stripe**. Exports estimate to **TurboTax Self-Employed**, schedules payment via **EFTPS**. Uses **IRS Direct Pay** for state taxes, saves confirmations to **Dropbox**. Sets Q4 reminder in **Notion**.

    **Year-round expense tracking:** After client lunch, photographs receipt in **Expensify**—syncs to **QuickBooks Self-Employed**. Drives to meeting with **MileIQ** tracking miles, takes **Uber** home and saves receipt. Orders supplies from **Amazon Business**, renews **Google Workspace**. Sends invoice through **FreshBooks**, reviews deductions dashboard in **QuickBooks Self-Employed**.

    ---

    ### Apps for Persona 2

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **QuickBooks Self-Employed** | Tax/Accounting | Tracks income and expenses with automatic tax categorization for freelancers. | Intuit account data export (Reports -> Export). | Paid volunteers | Remove client names and invoice details; mask bank feed data. |
    | **TurboTax Self-Employed** | Tax Preparation | Tax filing designed for 1099 workers with Schedule C guidance. | Intuit account data export + completed returns (PDF). | Paid volunteers | REDACT SSN and EIN; remove client 1099 details. |
    | **Expensify** | Expense Tracking | Receipt scanning and expense categorization for business deductions. | Expensify data export (CSV + receipt images). | Paid volunteers | Remove receipt images with personal info; mask vendor names if identifiable. |
    | **MileIQ** | Mileage Tracking | Automatic mileage tracking for business driving deductions. | MileIQ data export (CSV trip log). | Paid volunteers | Generalize specific addresses to city level; remove trip notes with client names. |
    | **IRS Direct Pay** | Tax Payment | Official IRS system for estimated tax payments. | Screenshots of payment confirmations. | Paid volunteers | REDACT bank account numbers; mask specific payment amounts if requested. |
    | **PayPal** | Payments | Receives freelance payments from clients, generates 1099-K. | PayPal data export (Activity -> Download). | Paid volunteers | Remove client email addresses; mask transaction IDs. |
    | **Stripe** | Payments | Payment processing for freelancers and small businesses. | Stripe dashboard export (Payments CSV). | Paid volunteers | Remove customer details; mask payout bank info. |
    | **Wave** | Accounting | Free accounting software for expense tracking and invoicing. | Wave data export (Reports -> Export). | Paid volunteers | Remove client names; anonymize invoice numbers. |
    | **FreshBooks** | Invoicing | Creates and tracks invoices for freelance work. | FreshBooks data export (Reports). | Paid volunteers | Remove client contact info; mask project names. |
    | **EFTPS** | Tax Payment | IRS system for scheduling federal estimated tax payments. | Screenshots of scheduled payments. | Paid volunteers | REDACT EIN and bank details. |
    | **Amazon Business** | Supplies | Business purchases with automatic receipt organization. | Amazon Data Request (order history). | Paid volunteers | Remove shipping addresses; mask payment methods. |
    | **Uber/Lyft** | Transportation | Business travel ride history for deductions. | Uber/Lyft data export (Privacy settings). | Paid volunteers | Generalize pickup/dropoff to city level. |
    | **Dropbox** | Storage | Cloud storage for tax documents and receipts. | Local folder upload. | Paid volunteers | Remove folder names with client identifiers. |
    | **Notion** | Productivity | Task management for tax deadlines and reminders. | Notion export (Settings -> Export). | Paid volunteers | Anonymize workspace names; remove shared member info. |

    ---



    # Advice Theme - Personal Finance: Investment Strategy Personas

    ---

    ## Persona 1: The Beginner Investor

    **Age:** 25-35

    **Lifestyle:** Just starting to invest, learning the basics, has some savings to put to work beyond an emergency fund.

    **Key needs:**
    * Understanding investment basics—stocks, ETFs, index funds.
    * Starting with simple, beginner-friendly investment apps.
    * Building a first portfolio with appropriate risk level.
    * Learning risk tolerance and avoiding emotional decisions.

    **Pain points:** Overwhelmed by too many investment options, scared of losing money, doesn't understand market terminology (P/E ratio, dividends, market cap), paralyzed by analysis and never actually invests, FOMO on trending stocks and meme investments.

    ---

    ### Example Scenarios

    **Starting first investment account:** Coworker mentions stocks, downloads **Robinhood** and transfers $500 from **Chase**. Confused about ETFs—searches on **Investopedia**, checks **Yahoo Finance** for VOO performance. Reads **Reddit** (r/personalfinance) threads, buys 2 shares of VOO. Downloads **Acorns** for automatic round-ups, sets up weekly recurring buy in **Robinhood**.

    **Understanding portfolio risk:** Gets $5,000 bonus—takes **Wealthfront** risk questionnaire, compares with **Betterment** recommendation. Reads **NerdWallet** robo-advisor reviews, links accounts to **Personal Capital** to see net worth. Explores **M1 Finance** pies, splits money between **Wealthfront** and **Robinhood**. Follows stocks on **Stocktwits**, sets alerts in **Yahoo Finance**.

    ---

    ### Apps for Persona 1

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **Robinhood** | Investing | Beginner-friendly app with commission-free trading and educational content. | Robinhood data export (Account -> Statements + Tax Docs). | Paid volunteers | Remove SSN from tax documents; mask specific stock quantities if large positions. |
    | **Wealthfront** | Robo-Advisor | Automated portfolio management with risk questionnaire for beginners. | Wealthfront data export (Statements + Portfolio Summary). | Paid volunteers | REDACT account numbers; remove beneficiary information. |
    | **Betterment** | Robo-Advisor | Goal-based investing with automatic rebalancing and tax-loss harvesting. | Betterment account export (Activity -> Download). | Paid volunteers | Remove linked bank account details; mask specific goal names if personal. |
    | **Personal Capital** | Portfolio Tracking | Free portfolio analysis and net worth tracking across all accounts. | Personal Capital data export (CSV transaction history). | Paid volunteers | Anonymize linked account names; remove specific property valuations. |
    | **Investopedia** | Education | Learning resource for investment terminology and concepts. | Screenshots of saved articles and portfolio simulator. | Paid volunteers | Remove account email from screenshots. |
    | **Acorns** | Micro-Investing | Automatic round-ups and spare change investing for beginners. | Acorns data export (Account -> Documents). | Paid volunteers | Remove linked debit card details; mask round-up sources. |
    | **SoFi Invest** | Investing | Commission-free trading with integrated banking and loans. | SoFi data export (Account statements). | Paid volunteers | REDACT account numbers; remove linked SoFi products. |
    | **M1 Finance** | Investing | "Pie" investing for custom portfolio allocation. | M1 data export (Documents -> Statements). | Paid volunteers | Remove beneficiary info; mask pie composition if custom names. |
    | **Yahoo Finance** | Market Data | Stock research, price tracking, and portfolio watchlist. | Yahoo data export (Portfolio CSV). | Paid volunteers | Remove watchlist with personal stock picks if sensitive. |
    | **Stocktwits** | Social/Investing | Social sentiment and discussion on stocks. | Screenshots of followed streams. | Paid volunteers | Remove username; anonymize followed accounts. |
    | **NerdWallet** | Education | Financial product comparisons and reviews. | Screenshots of saved comparisons. | Paid volunteers | Remove account email from screenshots. |
    | **Reddit** | Social | r/personalfinance and r/investing for community advice. | Reddit Data Request (Settings -> Privacy). | Paid volunteers | HIGH RISK: Anonymize subreddits; remove personal info from posts. |
    | **Plaid** | Data Aggregation | Connects bank accounts to investment apps securely. | Plaid connection logs (via connected apps). | Paid volunteers | Remove linked institution names; mask account identifiers. |

    ---

    ## Persona 2: The Experienced Investor

    **Age:** 45-60

    **Lifestyle:** Has been investing for years, manages diverse portfolio across multiple accounts, actively planning for retirement.

    **Key needs:**
    * Portfolio rebalancing to maintain target asset allocation.
    * Tax-efficient investing and tax-loss harvesting strategies.
    * Retirement planning with timeline-based risk adjustment.
    * Tracking investments across multiple brokerages and 401k accounts.
    * Estate planning considerations and beneficiary management.

    **Pain points:** Portfolio has grown complex across too many accounts, worried about market downturns affecting retirement timeline, tax implications of selling appreciated assets, keeping up with market changes and rebalancing needs, balancing growth vs capital preservation as retirement approaches.

    ---

    ### Example Scenarios

    **Portfolio rebalancing:** Strong quarter—checks **Fidelity** 401k, drifted to 85% stocks above 75% target. Reviews **Charles Schwab** taxable and **Personal Capital** for full picture across **Vanguard** IRA and **TD Ameritrade**. Uses **Morningstar** to research bond funds, spots tax-loss harvesting opportunity. Runs numbers in **TurboTax**, checks **E*TRADE** for forgotten positions. Backtests in **Portfolio Visualizer**, executes rebalancing in **Fidelity**, logs trades in **Microsoft Excel**.

    **Retirement planning review:** Turning 55—runs projections in **Fidelity Planning Center** for retire at 62 vs 65. Checks **Social Security Administration** for benefit estimates, reviews **Vanguard** target-date fund. Models withdrawals in **NewRetirement**, checks **Healthcare.gov** for pre-Medicare costs. Gets second opinion from **Empower**, reviews beneficiaries in **Fidelity** and **Schwab**. Updates estate docs in **Trust & Will**, checks spending baseline in **Mint**.

    ---

    ### Apps for Persona 2

    | App | Category | Why? | Data Collection Method | Data Source | App-Specific PII Notes |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | **Fidelity** | Investing/401k | Primary retirement account management with planning tools. | Fidelity data export (Statements + Portfolio CSV). | Paid volunteers | REDACT SSN and account numbers; remove employer 401k plan name; mask beneficiary names. |
    | **Charles Schwab** | Investing | Full-service brokerage for taxable investing with research tools. | Schwab data export (Account History CSV + Statements). | Paid volunteers | Remove cost basis details with purchase dates; mask specific position sizes. |
    | **Vanguard** | Investing/IRA | IRA and mutual fund management with low-cost index funds. | Vanguard data export (Download Center -> Portfolio). | Paid volunteers | REDACT account numbers; remove beneficiary and estate details. |
    | **Personal Capital / Empower** | Portfolio Tracking | Aggregated view of all investment accounts with fee analyzer. | Personal Capital export (Transactions + Holdings CSV). | Paid volunteers | Anonymize account nicknames; remove property and real estate valuations. |
    | **NewRetirement** | Retirement Planning | Detailed retirement modeling with scenario planning and projections. | Screenshots + PDF export of retirement plans. | Paid volunteers | Remove specific Social Security estimates; mask spouse information. |
    | **TD Ameritrade** | Investing | Options trading and advanced research tools. | TD Ameritrade data export (Statements + Trade History). | Paid volunteers | Remove options contract details; mask specific position sizes. |
    | **E*TRADE** | Investing | Brokerage account with stock plan services. | E*TRADE data export (Statements + Gains/Loss). | Paid volunteers | REDACT account numbers; remove employer stock plan details. |
    | **Morningstar** | Research | Fund research, ratings, and portfolio analysis. | Screenshots of portfolio X-ray and saved funds. | Paid volunteers | Remove premium account email. |
    | **Portfolio Visualizer** | Analysis | Backtesting and portfolio optimization tools. | Screenshots of saved portfolios and analysis. | Paid volunteers | Remove custom portfolio names if identifiable. |
    | **Social Security Administration** | Government | Estimates Social Security benefits at different ages. | Screenshots of benefit estimates. | Paid volunteers | REDACT SSN; remove specific benefit amounts. |
    | **Healthcare.gov** | Insurance | Marketplace for pre-Medicare health insurance research. | Screenshots of plan comparisons. | Paid volunteers | Remove income estimates; mask location to state level. |
    | **Trust & Will** | Estate Planning | Online estate planning and trust documents. | PDF export of created documents. | Paid volunteers | REDACT all personal info; remove beneficiary names. |
    | **Microsoft Excel** | Productivity | Custom portfolio tracking and rebalancing spreadsheets. | Local file upload. | Paid volunteers | Remove account numbers; anonymize position names if needed. |
    | **TurboTax** | Tax Planning | Capital gains estimation and tax planning. | Intuit account data export. | Paid volunteers | REDACT SSN; remove specific gain/loss amounts. |

    ---




