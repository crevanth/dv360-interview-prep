# DV360 & Programmatic Advertising Interview Questions & Answers

This document contains a comprehensive list of questions and answers related to Display & Video 360 (DV360) and the broader programmatic advertising ecosystem. It's designed for individuals preparing for roles in digital advertising, particularly those involving programmatic campaign management.

---

## I. Programmatic Fundamentals & Ecosystem

### **1. What is Programmatic Advertising in your own words?**

* **Answer:** Basically, programmatic advertising means using technology, like special software, to automatically buy and sell digital ad spaces online in real-time. Instead of people negotiating deals for weeks, computers do it in milliseconds. This software decides where to place ads based on rules we set – like who we want to reach, what websites they visit, where they are located, and our campaign goals – making advertising faster, more efficient, and targeted to the right audience.

### **2. Can you explain the difference between Programmatic Direct, Private Marketplace (PMP), and Open Auction (RTB)?**

* **Answer:** Think of it like buying goods:
    * **Open Auction (RTB - Real-Time Bidding):** Like a huge public market (e.g., a wholesale bazaar) where many sellers offer their ad spaces, and many buyers (advertisers) bid on them instantly. You get wide reach, but less control over exactly where your ad shows up sometimes.
    * **Private Marketplace (PMP):** Like a special, invite-only section of the market. Certain premium sellers (publishers) invite specific buyers they trust. Buyers bid against each other, usually above a minimum price (floor price). You get better quality placements and more transparency than the open market. Access is via a special code (Deal ID).
    * **Programmatic Direct (includes Programmatic Guaranteed - PG):** Like making a direct deal with a specific shop owner. The advertiser agrees to buy a fixed amount of ad space from a specific publisher at a fixed price. It guarantees the ad placement and price but offers less flexibility. It uses the same technology (Deal ID) for setup and reporting, making it more efficient than old manual deals.

### **3. Describe the typical journey of an ad impression request in the Real-Time Bidding (RTB) ecosystem, from user visit to ad rendering.**

* **Answer:** It happens incredibly fast, in less time than blinking!
    1.  **User Visits:** Someone opens a website or app with ad space.
    2.  **Signal Sent:** The website/app tells the publisher's system (SSP) "I have space for an ad!" and sends info about the user (like a cookie ID, not their name) and the page content.
    3.  **Auction Announced:** The SSP sends out a message (bid request) to many potential buyers (DSPs) saying, "Ad space available, here's the info, who wants to bid?"
    4.  **Buyers Decide:** Each DSP checks if this ad space and user match any of their active advertiser campaigns based on targeting rules (audience, location, time, etc.).
    5.  **Bids Placed:** If it's a match, the DSP quickly decides how much that ad space is worth to their advertiser and submits a bid price.
    6.  **Winner Chosen:** The SSP picks the highest bidder.
    7.  **Ad Delivered:** The SSP tells the winning DSP, "You won!" The winner's system then sends the actual ad (picture, video) back through the system.
    8.  **Ad Shown:** The ad appears on the user's screen in the designated space.

### **4. What is the role of a Demand-Side Platform (DSP)?**

* **Answer:** A DSP is the software platform that advertisers or their agencies use to buy ads programmatically. Think of it as the advertiser's "buying agent" in the automated market. It helps them:
    * Access ad spaces available across many different websites and apps (via SSPs/Exchanges).
    * Set up campaigns with specific targeting rules (who to reach, where, when).
    * Automatically bid on relevant ad spaces in real-time auctions.
    * Manage budgets and control spending.
    * See reports on how the campaigns are performing.

### **5. What is the role of a Supply-Side Platform (SSP)?**

* **Answer:** An SSP is the software platform that website/app owners (publishers) use to sell their ad spaces programmatically. It's the publisher's "selling agent". It helps them:
    * Make their ad spaces available to many potential buyers (DSPs/Exchanges) at once.
    * Manage which advertisers can buy their space and set minimum prices (floor prices).
    * Maximize the money they earn from selling ad space.
    * Get reports on how much inventory they sold and for how much.

### **6. What is an Ad Exchange, and how does it differ from an SSP or DSP?**

* **Answer:** An Ad Exchange is like the central marketplace itself – the technology platform that connects multiple buyers (via DSPs) and multiple sellers (via SSPs) together to conduct the real-time auctions.
    * **Difference:** DSPs work for the buyers, SSPs work for the sellers, and the Ad Exchange is the neutral trading floor in the middle where they meet to transact.

### **7. What is an Ad Server, and why is it important in digital advertising?**

* **Answer:** An ad server is a core piece of technology used to store ad creatives (the actual banners or videos), deliver them to the correct ad slot on a webpage or app, and count how many times the ad was shown (impressions) and clicked.
    * **Importance:** It's crucial for actually *showing* the ads and providing a reliable, often independent, count for reporting and billing. Platforms like Campaign Manager 360 (CM360) act as third-party ad servers (3PAS) for advertisers, giving them centralized control and measurement across different buying platforms. Publishers also use their own ad servers.

### **8. Explain the difference between a first-party cookie and a third-party cookie.**

* **Answer:** It depends on who places the cookie:
    * **First-Party Cookie:** Placed by the website you are *directly* visiting (e.g., the online store places a cookie to remember your shopping cart). Essential for website functionality.
    * **Third-Party Cookie:** Placed by a domain *different* from the website you are visiting (e.g., an ad tech company's server places a cookie via an ad tag shown on the news website you are reading). Used mainly for tracking users across different websites for advertising purposes like targeting and measurement.

### **9. How is the impending deprecation of third-party cookies impacting programmatic advertising?**

* **Answer:** It's a major change! Without third-party cookies, reliably tracking users across different websites becomes very difficult. This impacts:
    * **Targeting:** Harder to show ads based on someone's Browse history across multiple sites (retargeting becomes limited).
    * **Measurement:** Harder to know if someone saw an ad on one site and then converted on another site later.
    * **Frequency Capping:** Harder to limit how many times one person sees the same ad across different websites.
    * **Strategy Shift:** The industry is moving towards using first-party data (data collected directly by advertisers/publishers with consent), contextual targeting (showing ads based on page content), and new privacy-focused technologies (like Google's Privacy Sandbox).

### **10. What are some alternative identifiers or solutions being explored to replace third-party cookies for targeting and measurement?**

* **Answer:** The industry is exploring several paths:
    * **First-Party Data:** Using data advertisers or publishers collect directly with user permission (like email sign-ups).
    * **Contextual Targeting:** Showing ads relevant to the webpage content itself.
    * **Universal IDs:** Trying to create shared IDs based on consented data like hashed emails (e.g., UID 2.0, RampID). Needs wide adoption.
    * **Google Privacy Sandbox:** Google's initiative with APIs like Topics (interest groups), Protected Audience API (remarketing), and Attribution Reporting API designed to support ad use cases without cross-site tracking.
    * **Data Clean Rooms:** Secure places where advertisers and publishers can compare notes (analyze combined data) without sharing raw user details.

---

## II. Ad Tech Platforms & Comparisons

### **11. What are the key functions and benefits of using Display & Video 360 (DV360)?**

* **Answer:**
    * **Functions:** DV360 is Google's powerful DSP for large advertisers and agencies. It's used to plan, buy, manage, and measure programmatic ad campaigns across a huge network of websites, apps, and even connected TVs. You can run display ads, video ads, audio ads, and more.
    * **Benefits:** Gives access to massive inventory (including Google's like YouTube, plus many others), provides very detailed targeting options (using Google's data and other sources), offers smart automated bidding to achieve goals, integrates well with other tools like Campaign Manager 360 and Google Analytics for better measurement, and allows buying through special deals (PMPs/PG).

### **12. How does DV360 provide broader reach compared to platforms focused only on their own networks?**

* **Answer:** DV360 acts as a gateway to the wider programmatic world. While some platforms primarily offer advertising only on their own websites or apps (their 'walled garden'), DV360 connects to:
    * Google's own inventory (like YouTube, Google Display Network via AdX).
    * *And* numerous other major ad exchanges and SSPs.
    * This means an advertiser using DV360 can reach users across a vast range of different publishers, websites, and apps all over the internet, not just those owned by Google, allowing for much broader reach and diverse inventory options from a single platform.

### **13. What is Campaign Manager 360 (CM360), and how does it work with DV360?**

* **Answer:** CM360 is Google's ad server and measurement tool. Its main job isn't buying ads, but rather:
    * **Serving Ads:** It stores the actual ad creatives (images, videos). When DV360 buys an ad space, it often tells CM360 to deliver the creative.
    * **Measuring Performance:** It tracks impressions, clicks, and most importantly, conversions using its own Floodlight tags placed on the advertiser's website. This provides a central, reliable count across campaigns, even if ads were bought through different platforms (like DV360, social media, etc.).
    * **How they work together:** DV360 buys the ad space, CM360 delivers the ad and measures the results (especially conversions) using Floodlights.

### **14. Why might an advertiser use both DV360 and CM360 together?**

* **Answer:** Using both gives the advertiser more control and better insights:
    * **Centralized Tracking:** CM360's Floodlights provide a single source of truth for conversion tracking across *all* digital channels where CM360 tags are used, not just DV360. This helps avoid counting the same conversion multiple times.
    * **Independent Measurement:** CM360 acts as a third-party ad server, offering an independent count of impressions and clicks compared to the buying platform's numbers.
    * **Advanced Attribution:** CM360 offers sophisticated models to understand how different channels work together to drive conversions.
    * **Verification:** Easily integrate third-party viewability and fraud tracking across all campaigns served via CM360.
    * **Creative Management:** Central place to host and manage creatives used across multiple campaigns or platforms.

### **15. Besides DV360, can you name two other major DSPs in the market?**

* **Answer:** The Trade Desk (often called TTD), Amazon DSP. (Others include Xandr Invest, MediaMath).

### **16. Can you name two major SSPs or Ad Exchanges?**

* **Answer:** Google Ad Manager (includes Google AdX), Magnite, OpenX, PubMatic.

### **17. What factors would you consider when choosing a DSP for a client?**

* **Answer:** Key things to check are:
    * **Inventory Access:** Does it connect to the websites, apps, or types of inventory (like Connected TV) the client needs?
    * **Targeting Options:** Does it have the right audience data (Google data, third-party, first-party uploads) and contextual targeting needed?
    * **Bidding & Optimization:** Are its automatic bidding features smart and effective for the client's goals (CPA, ROAS)?
    * **Reporting:** Are the reports detailed and easy to understand? Can we get the insights we need?
    * **Ease of Use:** How easy is the platform to learn and manage campaigns in?
    * **Support:** Is good technical help available when needed?
    * **Cost:** What are the platform fees? Are data costs reasonable?
    * **Integrations:** Does it work well with other tools we use (like CM360, GA)?

---

## III. DV360 Account Structure

### **18. Can you outline the typical hierarchy within a DV360 account (from Partner down to Creatives)?**

* **Answer:** It's structured like folders within folders:
    1.  **Partner:** The main account, like the head office (e.g., agency group).
    2.  **Advertiser:** Represents one specific client or brand under the Partner. All settings like tracking (Floodlights) are linked here.
    3.  **Campaign:** An organizational folder under the Advertiser, used to group activities (e.g., "Diwali Promotion 2025").
    4.  **Insertion Order (IO):** A specific plan within the Campaign, having its own total budget, dates, and overall goal (e.g., "Diwali Video Ads - Budget ₹5 Lakh").
    5.  **Line Item (LI):** The detailed execution plan within an IO, specifying exactly who to target, where to show ads (display, video), how much to bid, and its specific budget (e.g., "YouTube Skippable Ads - Target City - Budget ₹2 Lakh").
    6.  **Creative:** The actual ad image or video file assigned to Line Items.

### **19. What is the purpose of the 'Advertiser' level in DV360?**

* **Answer:** The Advertiser level is the main setup area for a specific client. Here you connect essential things like:
    * Basic Info (Name, Currency like INR, Time Zone).
    * Floodlight Configuration (linking to CM360 for conversion tracking).
    * Links to other accounts (like Google Analytics, YouTube).
    * Manage shared audience lists for that advertiser.
    * Set overall brand safety rules or frequency caps if needed.

### **20. What is a 'Campaign' in DV360 used for?**

* **Answer:** Think of the Campaign level mainly as a **folder** for organization. It helps group together multiple Insertion Orders (IOs) that belong to the same overall marketing effort or time period (like a quarterly campaign). It doesn't have its own budget or targeting, it just keeps things tidy.

### **21. What is an 'Insertion Order' (IO), and what key settings are defined at this level?**

* **Answer:** An IO is like a mini-contract or plan for a specific part of your advertising. It sets the overall rules and budget for a group of Line Items working towards one main goal.
    * **Key Settings:** Overall **Budget** (e.g., ₹10 Lakh total), **Flight Dates** (e.g., Oct 1st - Nov 15th), **Pacing** (how fast to spend - Evenly?), overall **Goal** (e.g., achieve ₹500 CPA), overall **Frequency Cap** (e.g., show max 5 ads per user per day across all LIs inside), and often default **Brand Safety** rules.

### **22. What is a 'Line Item' (LI), and what is its primary function?**

* **Answer:** The Line Item is where the real action happens – it's the detailed plan for buying specific types of ads. Its function is to execute a specific tactic within the IO's plan. Here you define:
    * **Ad Type:** Display, Video, Audio?
    * **Budget:** How much of the IO's budget this specific LI gets (e.g., ₹3 Lakh).
    * **Dates:** When this LI should run (within the IO's dates).
    * **Bidding:** How much to bid and what strategy to use (e.g., bid for clicks, bid for conversions at ₹450 CPA).
    * **Targeting:** *Exactly* who to show ads to (audience lists, location like Hyderabad, age, interests), where to show them (specific websites, apps, deals), and on what devices.
    * **Creatives:** Which specific ads (banners/videos) to run for this LI.

---

## IV. Campaign Planning & Setup Process

### **23. Walk me through the key steps you would take when planning a new programmatic campaign in DV360.**

* **Answer:** A proper plan is key for success:
    1.  **Understand Goal (Objective):** First, clearly understand what the client wants to achieve. Is it just making people aware of the brand (Awareness)? Getting them interested (Consideration)? Or making them buy something or sign up (Conversion)?
    2.  **Define Target Audience:** Who exactly are we trying to reach? Age, gender, location (e.g., only major cities in India?), interests, online behaviour? Do they have customer lists we can use?
    3.  **Set KPI:** How will we measure success? What number defines success? (e.g., Reach X million people, Get Y leads at less than ₹Z cost per lead, achieve X:1 return on spending).
    4.  **Allocate Budget & Dates:** How much money (Budget) do we have? For how long should the campaign run (Flight Dates)?
    5.  **Choose Strategy (Media Plan):** Which channels/formats make sense (Display banners? YouTube videos? Audio ads?)? Which targeting methods will work best? Should we use open auction or look for specific deals (PMPs)?
    6.  **Prepare Creatives:** What ads will we show? Do the messages match the audience and goal? Do we need different versions? Where will people land after clicking (Landing Page)?
    7.  **Setup Tracking:** Is conversion tracking ready (Floodlights)? How will we measure success accurately?
    8.  **Select Bidding:** Which bidding method suits the KPI (e.g., bid for viewability, bid for clicks, bid for conversions)?
    9.  **Plan Structure:** How will we organize the campaign in DV360 (Campaign > IO > LIs)? Use clear names!

### **24. How do you determine the primary Key Performance Indicator (KPI) for a campaign?**

* **Answer:** The primary KPI should directly measure the main goal of the campaign. We need to ask the client or stakeholder, "What does success look like for this specific campaign?"
    * If the goal is Brand Awareness, the KPI might be **Viewability Rate (%)** or **Reach**.
    * If the goal is Website Traffic/Interest, the KPI could be **Click-Through Rate (CTR)** or low **Cost Per Click (CPC)**.
    * If the goal is Leads or Sales, the KPI must be **Cost Per Acquisition (CPA)** or **Return On Ad Spend (ROAS)**.
    * The KPI is the main number we will track closely to see if the campaign is working.

### **25. How do client objectives (e.g., Awareness, Consideration, Conversion) influence campaign strategy and setup in DV360?**

* **Answer:** The objective changes everything:
    * **Awareness:** Goal is broad reach. Strategy = Target wide audiences (general interests, demographics). Use formats like video (bumpers, non-skip) or large display banners. Bidding = Focus on impressions (CPM) or viewable impressions (vCPM). Measure success by Reach, Frequency, Viewability.
    * **Consideration:** Goal is engagement. Strategy = Target people showing interest (in-market for the product, searching related terms, visited website but didn't buy). Use formats like clickable banners, native ads, skippable YouTube ads. Bidding = Focus on clicks (CPC) or views (CPV). Measure success by CTR, Site Visits, Video View Rate.
    * **Conversion:** Goal is action (sale/lead). Strategy = Target high-intent audiences (people who abandoned cart, past buyers, lookalikes of buyers). Use formats like standard display with strong offers, dynamic ads showing products, YouTube action ads. Bidding = Focus on conversions (tCPA, tROAS). Measure success by Conversions, CPA, ROAS.

### **26. Where do you set the overall budget and flight dates for a specific initiative within DV360?**

* **Answer:** The total budget (like the overall approved spend) and the main start/end dates for a campaign phase are set at the **Insertion Order (IO)** level.

### **27. How do you approach setting budgets at the Insertion Order vs. Line Item level?**

* **Answer:** It's like managing household expenses:
    * **IO Budget:** This is the total money allocated for the whole project or period (e.g., ₹10 Lakh for the entire Diwali campaign). It's the maximum limit.
    * **LI Budget:** This is how you divide the total IO budget among different activities (e.g., ₹4 Lakh for YouTube ads LI, ₹3 Lakh for Remarketing display LI, ₹3 Lakh for Prospecting display LI). You allocate based on which activity is expected to contribute most to the goal or has the potential to reach the right audience effectively. The sum of LI budgets should match the IO budget for that period.

### **28. What is frequency capping, and where can it be set in DV360? Why is it important?**

* **Answer:**
    * **What:** Frequency capping is setting a limit on how many times a single person sees your ad within a specific time (e.g., maximum 3 times per day).
    * **Where:** Can be set at the **Insertion Order (IO)** level (applies to all LIs inside) and/or more specifically at the **Line Item (LI)** level.
    * **Why Important:** It's crucial because showing the same ad too many times annoys people (ad fatigue) and wastes money. Capping helps reach more *different* people with your budget and keeps the user experience better.

### **29. What information is crucial to gather from a client brief before starting campaign setup?**

* **Answer:** To do a good job, we need clear instructions. Key things to get from the client brief are:
    * **Main Goal:** What is the #1 objective? (Awareness, Leads, Sales?)
    * **Success Metric (KPI):** How will we measure success? (Target CPA? Target ROAS? Viewability %?)
    * **Budget:** Exactly how much money can we spend?
    * **Dates:** When should the campaign start and end?
    * **Target Audience:** Who are we trying to reach? (Age, location - e.g., specific cities in India, interests?) Any customer lists?
    * **Rules/Restrictions:** Any websites, content types, or locations to avoid? Brand safety rules?
    * **Ads (Creatives):** What ads (banners, videos) will be used? What is the message? Where does the ad click lead to (Landing Page URL)?
    * **Tracking:** Is conversion tracking (Floodlights) properly set up?
    * **Past Learnings:** What worked well or badly in previous campaigns?

---

## V. DV360 Insertion Order (IO) Settings

### **30. What are the different IO pacing options in DV360 (e.g., ASAP, Even, Ahead), and when would you use each?**

* **Answer:** Pacing controls how fast the IO budget is spent:
    * **Even:** Spends the budget smoothly throughout the campaign dates. Best for most campaigns to ensure consistent visibility. (Like eating your meals at regular times).
    * **ASAP (As fast as possible):** Tries to spend the budget very quickly at the start. Use only for very short campaigns or urgent promotions where getting results immediately is critical. (Like eating all your food at breakfast). Risk: Budget might finish too early.
    * **Ahead:** Spends the budget slightly faster than 'Even' pacing. Can be useful if you expect delivery to be harder later in the campaign, or want to gain early momentum. (Like eating a bit more for lunch than dinner).

### **31. Besides budget, flight dates, and pacing, what other critical settings are managed at the IO level?**

* **Answer:** The IO level also sets other important rules for the Line Items inside it:
    * **Performance Goal:** The main KPI the IO aims for (influences LI bidding).
    * **Frequency Cap:** Overall limit on ad views per user.
    * **Brand Safety:** Default rules about avoiding unsafe content (sensitivity filters, content labels).
    * **Default Targeting (Optional):** Can set default Geo, Language, Demographics (but usually refined at LI level).
    * **Verification:** Link third-party tracking tags (IAS, DV, Moat).

### **32. Can you set specific performance goals (KPIs) at the IO level? How does this impact optimization?**

* **Answer:** Yes, you set the primary performance goal (like Target CPA, Target CTR, Target Viewability %) for the entire IO. This tells DV360 what success looks like overall for this part of the plan. It acts as a guide for the automatic bidding strategies working within the Line Items, pushing them collectively towards achieving that main IO goal. It also helps focus reporting on what matters most.

---

## VI. DV360 Line Item (LI) Deep Dive

### **33. What are the main Line Item types available in DV360?**

* **Answer:** Line Item types define the kind of ad you are running:
    * **Display:** For image banners, HTML5 ads, native ads on websites and apps.
    * **Video:** For video ads (often split into YouTube vs. other web/app video).
    * **Audio:** For ads on music streaming or podcasts.
    * **Mobile App Install:** Focused specifically on driving installs for an app.

### **34. Within a Display Line Item, what are common formats you might run?**

* **Answer:** Common display formats include:
    * **Standard:** Regular image ads (like JPEG, GIF).
    * **HTML5:** More interactive, animated ads.
    * **Native:** Ads designed to look like part of the website's normal content.
    * **Rich Media:** Advanced ads with features like video or expansion.

### **35. What targeting options are configured specifically at the Line Item level?**

* **Answer:** Most of the detailed targeting happens here:
    * **Audiences:** Choosing specific lists (like remarketing lists, in-market audiences, custom lists) to include or exclude.
    * **Inventory Source:** Selecting specific websites, apps, ad exchanges, or special deals (PMPs/PGs). Creating allow/block lists.
    * **Geography:** Pinpointing specific cities, regions, or even areas around a location (radius).
    * **Demographics:** Refining age/gender.
    * **Viewability:** Setting a minimum viewability % target.
    * **Keywords/Categories (Contextual):** Targeting pages about certain topics.
    * **Technology:** Targeting specific devices, browsers, or operating systems.
    * **Brand Safety:** Applying specific keyword blocks or refining category exclusions inherited from the IO.

### **36. Can you explain what "Inherited Targeting" means? What settings typically cascade down from the IO to the LI?**

* **Answer:** Inherited targeting simply means that some settings you apply at the higher Insertion Order (IO) level are automatically passed down and applied to all the Line Items (LIs) created underneath it.
    * **Typically Inherited:** Brand Safety rules (like sensitivity filters), IO-level Frequency Caps, and sometimes default Geo/Demo/Language settings if they were set at the IO level.
    * **What's *Not* Inherited (Set at LI):** Specific Audience lists, specific Inventory sources (like Deals or exchanges), the Bid Strategy, the LI's own budget, and specific creative assignments are almost always set uniquely at the Line Item level. An LI can usually make inherited settings *stricter* (e.g., add more blocked keywords) but not usually *looser*.

### **37. How do you select inventory sources for a Line Item?**

* **Answer:** Within the Line Item settings, you go to "Inventory Source" targeting. Here you can choose:
    * **Public Inventory:** Target inventory broadly available on selected Ad Exchanges (like Google AdX, OpenX etc.).
    * **Deals & Auction Packages:** Target specific Private Marketplace (PMP) deals, Programmatic Guaranteed (PG) deals, or curated inventory packages by entering their unique Deal ID.
    * **Specific Lists:** Target only specific websites/apps using an Allowlist, or exclude specific ones using a Blocklist.

### **38. What is the difference between targeting "Public Inventory" versus specific "Deals"?**

* **Answer:**
    * **Public Inventory (Open Auction):** Buying from the wide open market. Pros: Huge scale/reach. Cons: Less control over exact placement quality, variable pricing.
    * **Deals (PMP/PG):** Buying from specific publishers via pre-arranged agreements (using Deal IDs). Pros: Better quality control, more transparency, access to premium spots, potentially better brand safety. Cons: Usually costs more (higher CPM), less scale than open auction. PG deals offer guaranteed delivery at a fixed price.

---

## VII. YouTube & Partners Line Items in DV360

### **39. What are the main objectives you can choose when setting up a YouTube & Partners Line Item in DV360?**

* **Answer:** You align your YouTube LI with your marketing goal. Common objectives available influence how the LI optimizes:
    * **Brand awareness and reach:** Goal is to show ads to many unique people. Uses tCPM bidding.
    * **Product and brand consideration:** Goal is to get people interested and watching your videos. Uses CPV bidding.
    * **Website traffic:** Goal is to drive clicks to your website. Uses Maximize Clicks or tCPA bidding.
    * **Leads / Sales (Action):** Goal is to get direct responses like sign-ups or purchases. Uses tCPA, tROAS, or Maximize Conversions bidding.

### **40. Based on the chosen objective, what are the corresponding bid strategies typically used for YouTube campaigns?**

* **Answer:** The bid strategy matches the objective:
    * Awareness/Reach -> **Target CPM (tCPM)** (pay per impression)
    * Consideration -> **Cost Per View (CPV)** (pay per view or interaction)
    * Traffic -> **Maximize Clicks** or sometimes tCPA
    * Leads/Sales -> **Target CPA (tCPA)**, **Target ROAS (tROAS)**, or **Maximize Conversions/Value**

### **41. What are the different YouTube ad formats available via DV360?**

* **Answer:** You can run several types:
    * **Skippable In-Stream:** Plays before/during/after videos, user can skip after 5 secs. (Good for telling a story if engaging).
    * **Non-Skippable In-Stream:** Max 15 secs, cannot be skipped. (Good for guaranteed message delivery).
    * **Bumper Ads:** Max 6 secs, non-skippable. (Good for quick reminders, high frequency).
    * **In-Feed Video Ads:** Appear in search results/related videos/homepage feed as a thumbnail + text. User must click to watch. (Good for capturing interest when users are actively Browse).

### **42. What is the difference between a skippable in-stream ad and a non-skippable in-stream ad in terms of length and billing?**

* **Answer:**
    * **Skippable:** Various lengths possible (even long), but user can skip after 5 seconds. You typically pay on CPV (Cost Per View - if they watch 30s/full or interact) or CPM (if goal is awareness).
    * **Non-Skippable:** Short, max 15 seconds (sometimes 20s). Cannot be skipped. You pay on Target CPM (per thousand impressions).

### **43. What is a Bumper Ad, and what type of campaign goal is it best suited for?**

* **Answer:** A Bumper Ad is a super short (6 seconds max), non-skippable video ad shown before, during, or after a YouTube video. Because it's short and guarantees viewing, it's perfect for **Brand awareness and reach**. Great for quick, memorable messages or reinforcing a main campaign theme frequently. Billed on Target CPM.

### **44. What were "TrueView for Action" campaigns, and how has that concept evolved into current YouTube Action formats?**

* **Answer:** "TrueView for Action" was the old name for YouTube campaigns focused purely on getting conversions (clicks, leads, sales). They used features like strong call-to-action buttons and conversion-based bidding (like tCPA). The *idea* still exists, but now you achieve it by selecting **Leads**, **Sales**, or **Website Traffic** as your objective for a YouTube Line Item in DV360. The platform then automatically uses the action-driving features and bidding strategies associated with that goal.

### **45. Can you target YouTube Masthead inventory via standard DV360 Line Items?**

* **Answer:** Normally, no. The Masthead (the big banner ad space on the YouTube homepage) is usually sold directly by Google on a reservation basis (fixed price for a day or impressions), not through the regular DV360 auction system.

### **46. How do you set up an "Efficient Reach" Line Item for YouTube?**

* **Answer:** To maximize reach efficiently on YouTube:
    1.  Choose the **Brand awareness and reach** objective.
    2.  Select **Efficient Reach** as the specific goal subtype.
    3.  Use **Target CPM (tCPM)** bidding.
    4.  Often combine **Bumper Ads** (6s) and **Skippable In-Stream Ads** within the same LI to let Google's system optimize for the lowest cost per reached user.
    5.  Set a **Frequency Cap** goal (e.g., target reaching users an average of X times per week) to control exposure while maximizing unique users reached within budget.

### **47. What's the process for creating a non-skippable ad Line Item on YouTube?**

* **Answer:**
    1.  Choose the **Brand awareness and reach** objective.
    2.  Select **Non-skippable in-stream** as the Ad Format within the LI setup.
    3.  Assign only non-skippable creatives (15 seconds or shorter).
    4.  Use **Target CPM (tCPM)** bidding, as you pay per impression for non-skippable ads.
    5.  Apply relevant targeting (audience, geo, etc.).

### **48. How do Ad Sequence Line Items work on YouTube?**

* **Answer:** Ad Sequence LIs allow you to tell a story by showing a series of video ads to the same person in a specific order you define.
    1.  Choose the **Brand awareness and reach** or **Product and brand consideration** objective.
    2.  Select **Ad sequence** as the subtype/strategy.
    3.  Define the sequence steps: Add video creatives in the desired order.
    4.  Set rules for progression (e.g., move to step 2 after user sees step 1 impression/view, or skips step 1).
    5.  Apply targeting and bidding (often tCPM or CPV depending on goal).
    * Use case: Introduce a problem, then solution; showcase different product features sequentially. Requires users to be identifiable across sessions.

### **49. What is Target Frequency buying on YouTube?**

* **Answer:** Target Frequency buying is an option under the **Brand awareness and reach** objective. Instead of just maximizing reach, you set a specific **target frequency** (e.g., aim to reach users an average of 3 times per week). DV360's system will then optimize bidding and delivery to achieve that desired average frequency level across your target audience within the budget and flight dates. It helps ensure users see the message multiple times for better recall, without over-exposing them.

### **50. How do you optimize for Video Views (Consideration) on YouTube?**

* **Answer:** To get more people to actively watch your videos:
    1.  Choose the **Product and brand consideration** objective.
    2.  Use **Cost Per View (CPV)** bidding. You set a maximum price you're willing to pay for a view (a view is counted if someone watches 30 seconds, the full ad if shorter, or interacts).
    3.  Focus on **Engaging Creative:** The first 5 seconds are critical (especially for skippable ads) to capture attention. Make sure the video is interesting and relevant to the target audience.
    4.  Use **Skippable In-Stream** or **In-Feed Video Ad** formats, as these are optimized for views/engagement.
    5.  Target audiences likely to be interested in your content (relevant In-Market, Custom Audiences, Remarketing).
    6.  Monitor **View Rate (VTR)** and **VCR** (quartiles) to see how engaging the video is and where people drop off. A/B test different video versions.

### **51. What objective and settings correspond to driving conversions on YouTube via DV360?**

* **Answer:** To drive actions like sales or leads from YouTube ads:
    1.  Choose the **Leads** or **Sales** objective (or potentially **Website Traffic** depending on the specific action).
    2.  Use conversion-focused bid strategies: **Target CPA (tCPA)**, **Target ROAS (tROAS)**, or **Maximize Conversions/Value**.
    3.  Utilize **Video Action Campaign** principles/formats – these often use skippable in-stream but include prominent features like Calls-to-Action buttons, headlines, sitelinks, and end screens designed to encourage clicks and conversions.
    4.  Ensure accurate **Conversion Tracking** (Floodlights with values for ROAS) is set up and linked.
    5.  Target high-intent audiences (remarketing, customer match, similar audiences based on converters, relevant in-market or custom audiences).

---

## VIII. Targeting Strategies & Options

### **52. What are First-Party audiences in DV360? Provide examples.**

* **Answer:** First-Party audiences are lists of users created from data an advertiser collects directly from its own customers or website/app visitors. This data is owned by the advertiser. Examples in DV360 include:
    * **Website Visitors (Remarketing):** Users who visited specific pages or sections of the advertiser's website (tracked via Floodlight tags or Google Analytics).
    * **App Users:** Users who interacted with the advertiser's mobile app (tracked via Floodlight or GA4).
    * **Customer Match:** Lists of customer emails, phone numbers, or mailing addresses uploaded by the advertiser (hashed for privacy) to match against Google users.
    * **CRM Data:** Lists derived from the advertiser's Customer Relationship Management system, often onboarded via approved third-party partners.
    * **Conversion-Based Audiences:** Users who completed specific Floodlight conversion actions (e.g., purchasers, lead submitters).

### **53. What are Google Audiences? Explain Affinity, In-Market, and Custom Audiences.**

* **Answer:** Google Audiences are audience segments created and provided by Google based on user activity across Google properties (Search, YouTube, Maps, Gmail, Discover, Google Display Network). Key types include:
    * **Affinity Audiences:** Represent broad, long-term interests, lifestyles, and habits based on users' overall online behavior (e.g., "Movie Lovers," "Cooking Enthusiasts," "Travel Buffs"). Good for upper-funnel awareness campaigns targeting general interests.
    * **In-Market Audiences:** Identify users who are actively researching, comparing, and showing strong intent to purchase a specific product or service category *in the near future* (e.g., "In-market for SUVs," "In-market for Home Mortgages"). Based on recent clicks, searches, site visits, conversions. Good for mid-to-lower funnel consideration and conversion goals.
    * **Custom Audiences:** Allow advertisers to create more tailored audiences based on specific inputs:
        * *Keywords:* Users who searched for particular terms on Google.
        * *URLs:* Users who visited specific types of websites.
        * *Apps:* Users who use particular mobile apps.
        * *Places:* Users who recently visited certain types of physical locations (using Google Maps data).
        Offers more precision and flexibility than standard Affinity or In-Market segments.

### **54. When would you use an Affinity audience versus an In-Market audience?**

* **Answer:**
    * **Use Affinity:** For **Awareness** campaigns. When you want to reach a broad audience with general, long-term interests related to your product category to build brand recognition or introduce a new product/service. Example: A new streaming service targeting "Movie Lovers" and "TV Fans."
    * **Use In-Market:** For **Consideration** or **Conversion** campaigns. When you want to reach users who are actively researching and close to making a purchase decision in your specific category. Example: A car dealership targeting users "In-market for SUVs" or "In-market for Used Cars."

### **55. How do you create Custom Audiences, and what inputs can you use?**

* **Answer:** Custom Audiences are created within the DV360 interface (or Google Ads, then shared). You define them by providing specific inputs related to user behavior or interests:
    * **Keywords:** Enter search terms that your ideal audience might use on Google (e.g., "noise cancelling headphones," "best wireless earbuds").
    * **URLs:** Enter specific website addresses (URLs) that your audience might visit (e.g., tech review sites, competitor websites).
    * **Apps:** Enter names of mobile apps your audience might use (e.g., specific airline apps, fitness tracking apps).
    * **Places:** Select types of physical locations users might visit (e.g., "Coffee Shops," "Electronics Stores," based on Google Maps data).
    You can combine these inputs and specify whether the audience should reach people *with any* of these interests/behaviors (broader reach) or *based on search activity* (more intent-focused).

### **56. What are Similar Audiences (Lookalikes), and how are they generated?**

* **Answer:** Similar Audiences (often called Lookalikes on other platforms) are audiences automatically created by Google's machine learning algorithms. They find new users who share characteristics and online behaviors similar to users on an existing first-party "seed" list (e.g., website visitors, converters, Customer Match list). Google analyzes the seed list for common traits (interests, demographics, Browse patterns) and then finds other users across its network who exhibit similar patterns. They are used to expand reach beyond existing remarketing lists to find potential new customers who resemble current valuable customers.

### **57. What are Third-Party audiences, and what should you consider before using them?**

* **Answer:** Third-Party audiences are segments created and sold by external data providers (e.g., Acxiom, Oracle Data Cloud, Experian) and made available for targeting within DSPs like DV360. These segments cover a wide range of demographics, purchase behaviors, financial attributes, life events, etc., based on offline and online data collection.
    * **Considerations Before Using:**
        * **Cost:** They usually incur an additional CPM data fee on top of the media cost.
        * **Relevance & Accuracy:** Data quality and recency can vary by provider and segment. Assess if the segment truly matches your target audience.
        * **Overlap:** Check for potential overlap with first-party or Google audiences you are already using (to avoid paying extra for users you could reach otherwise).
        * **Privacy Compliance:** Ensure the data provider adheres to privacy regulations (like GDPR, CCPA).
        * **Scale:** Verify if the segment size is sufficient for your campaign goals in the target region.
        * **Performance:** Test performance against other audience types before scaling significantly.

### **58. Explain contextual targeting. How does it differ from audience targeting?**

* **Answer:**
    * **Contextual Targeting:** Places ads based on the *content* of the webpage or app the user is currently viewing. It analyzes keywords, topics, and the overall theme of the page to determine relevance. Example: Placing an ad for running shoes on an article about marathon training.
    * **Difference from Audience Targeting:** Audience targeting focuses on *who the user is* based on their past behavior, interests, or demographics, regardless of the content they are viewing at that moment. Contextual targeting focuses on *where the ad appears* based on the immediate environment's content, without relying on user history or cookies. Contextual is becoming more important as third-party cookies phase out.

### **59. What types of geographical targeting options are available in DV360?**

* **Answer:** DV360 offers granular geo-targeting:
    * **Country, Region/State, City:** Standard large-area targeting.
    * **Postal Code/PIN Code:** Targeting specific postal areas.
    * **Radius Targeting:** Targeting a specific radius (in miles or kilometers) around a point of interest (e.g., a physical store address).
    * **Exclusion:** Ability to exclude any of the above geographic levels.

### **60. How can you utilize demographic and technological targeting?**

* **Answer:**
    * **Demographic Targeting:** Allows targeting or excluding users based on:
        * *Age:* Predefined age brackets (e.g., 18-24, 25-34).
        * *Gender:* Male, Female, Unknown.
        * *Parental Status:* Parent, Not a parent, Unknown.
        * *Household Income:* (Available in some regions, often based on inferred data).
    * **Technological Targeting:** Allows targeting based on:
        * *Device Type:* Desktop, Mobile, Tablet, Connected TV.
        * *Operating System:* iOS, Android, Windows, macOS, specific versions.
        * *Browser:* Chrome, Safari, Firefox, Edge, etc.
        * *Device Model:* Specific phone or tablet models (e.g., iPhone 14, Samsung Galaxy S23).
        * *Network Carrier/ISP & Connection Speed:* (e.g., WiFi vs Cellular).
    * *Use:* Refine reach to specific user groups, tailor creative messaging (e.g., different OS for app install ads), or exclude irrelevant segments.

### **61. What is viewability targeting, and how can you set minimum viewability thresholds for your Line Items?**

* **Answer:** Viewability targeting allows you to optimize ad delivery towards impressions predicted to be viewable according to certain standards (e.g., MRC standard: 50% of pixels on screen for 1 second for display, 2 seconds for video).
    * **Setting Thresholds:** Within the Line Item settings, under "Viewability" targeting (powered by Google's Active View technology), you can set a minimum predicted viewability percentage threshold (e.g., target only impressions predicted to have >60% or >70% viewability). Bidding strategies like vCPM also inherently optimize for viewability.
    * *Use:* Improves the chances that your ads are actually seen, crucial for branding campaigns where visibility is paramount. Targeting higher thresholds may reduce reach and increase CPMs.

### **62. Explain Brand Safety controls in DV360. How can you prevent ads from showing next to inappropriate content?**

* **Answer:** DV360 offers multiple layers of brand safety controls, typically set at the Advertiser or IO level and inherited/refined at the LI level:
    * **Sensitive Category Exclusions:** Block ads from appearing alongside content categorized as sensitive (e.g., Tragedy & Conflict, Sensitive Social Issues, Profanity, Sexually Suggestive). Multiple tiers of sensitivity can be selected.
    * **Digital Content Labels:** Exclude content based on maturity ratings (e.g., DL-G, DL-PG, DL-T, DL-MA - similar to movie ratings). Allows excluding content not suitable for general audiences.
    * **Application Exclusions:** Block ads from appearing on specific mobile apps or app categories.
    * **Keyword Blocking (Contextual):** Create lists of negative keywords. Ads will be blocked from pages where these keywords are detected in the content.
    * **Placement Exclusions (URL/App Blocklists):** Maintain lists of specific websites or apps where you never want your ads to appear.
    * **Third-Party Verification Integration:** Apply pre-bid avoidance segments and post-serve monitoring tags from vendors like IAS, DoubleVerify, Moat to enforce specific brand safety rules and get independent measurement.

### **63. Can you apply negative targeting (exclusions) in DV360? At what levels?**

* **Answer:** Yes, negative targeting is crucial for efficiency and brand safety. Exclusions can be applied at multiple levels:
    * **Advertiser Level:** Some exclusions like Blocked Apps might be managed here.
    * **Insertion Order (IO) Level:** Geo exclusions, Demographic exclusions, Language exclusions, Keyword blocklists, Placement blocklists, Sensitive Category exclusions, Digital Content Label exclusions can be set here and inherited by LIs.
    * **Line Item (LI) Level:** All the exclusions available at the IO level can be applied or refined here. Additionally, specific Audience Lists can be excluded, and specific Exchanges or Deals can be excluded from the inventory pool.

---

## IX. Creatives & Ad Serving

### **64. How are creatives assigned to Line Items in DV360?**

* **Answer:** Creatives are first uploaded or associated at the Advertiser level in DV360. Then, within a specific Line Item's settings, you navigate to the "Creatives" section. Here, you can select one or more eligible creatives (based on format and size compatibility with the LI's targeting and inventory) from the Advertiser's library to assign to that Line Item. Multiple creatives can be assigned to a single LI for rotation or optimization.

### **65. What are the different creative rotation options (Even, Optimized, Weighted, Sequential), and when would you use each?**

* **Answer:** Creative rotation settings (at the LI level) control how assigned creatives are served:
    * **Even:** Distributes impressions as evenly as possible among all active creatives. Use for A/B testing creatives fairly to compare performance head-to-head.
    * **Optimized:** Uses Google's machine learning to automatically serve the creatives predicted to perform best (based on CTR, Conversion Rate, Viewability, or the LI's goal) more often. Use after an initial testing phase or when maximizing performance is the priority.
    * **Weighted:** Allows you to manually assign a percentage weight to each creative, controlling its serving frequency relative to others. Use when you have specific reasons to prioritize certain messages or offers manually.
    * **Sequential:** Serves creatives in a specific, predefined order to tell a story over multiple impressions to the same user. Requires users to be identifiable across impressions (e.g., via cookies/IDs).

### **66. What is Dynamic Creative Optimization (DCO), and how can it be used in DV360?**

* **Answer:** DCO is an ad technology that automatically generates personalized ads in real-time by assembling predefined creative components (images, headlines, CTAs, etc.) based on specific data points about the user or context (e.g., location, past Browse behavior, audience segment, weather).
    * **Use in DV360:** DV360 supports DCO through integration with Google's dynamic creative formats (e.g., for retail remarketing showing previously viewed products) or by using creatives built in Google Web Designer or third-party DCO platforms (like Google Studio, formerly DoubleClick Studio, or Celtra, Jivox) whose tags are then trafficked in DV360. It allows for tailoring ad messages at scale to increase relevance and performance, particularly effective for remarketing and product-focused campaigns.

### **67. What are VAST and VPAID tags primarily used for? What's the key difference?**

* **Answer:** Both are standards for serving video ads programmatically.
    * **VAST (Video Ad Serving Template):** The industry standard XML protocol for communication between ad servers and video players. It provides the player with essential information: the location of the video file, its duration, tracking URLs for impressions/clicks/quartiles, companion ads, skippability rules. Focuses on standardized delivery and tracking.
    * **VPAID (Video Player Ad-Serving Interface Definition):** An older standard designed to enable rich interactivity *within* the video ad unit itself (e.g., clickable overlays, forms, games). It essentially allows executable code to run inside the player.
    * **Key Difference:** VAST focuses on standardized delivery and basic tracking of the video ad. VPAID enables complex interactivity within the ad but introduces potential performance issues, security risks, and measurement inconsistencies. VPAID usage is declining in favor of VAST combined with newer interactivity/measurement standards like SIMID and OMID.

### **68. What is an MRAID tag used for?**

* **Answer:** MRAID (Mobile Rich Media Ad Interface Definitions) is the standard API for rich media ads designed to run within mobile *app* environments. It provides a standardized way for HTML5 ads to interact with the features of a mobile app and the device itself, such as expanding the ad, detecting device orientation, accessing the camera or calendar (with permission), or closing the ad. It ensures interactive ads work consistently across different apps that support the MRAID standard.

### **69. What's the difference between using an iFrame tag versus a JavaScript tag for display ads? What are the pros and cons?**

* **Answer:** These are two methods for implementing third-party ad server tags (like CM360 tags) on a publisher's page:
    * **iFrame (Inline Frame) Tag:** Creates a self-contained HTML document (a sandbox) embedded within the main webpage. The ad content loads and executes entirely within this frame.
        * *Pros:* More secure (ad code cannot easily interfere with the main page), simpler for publishers.
        * *Cons:* Can sometimes limit ad interactivity with the main page, historically posed challenges for viewability measurement (though less so now).
    * **JavaScript Tag:** Executes code directly within the context of the main webpage.
        * *Pros:* Allows for more complex ad interactions (like page takeovers, expanding ads that push content), potentially provides more accurate measurement data (can access page information).
        * *Cons:* Less secure (malicious code could potentially affect the page), might slightly impact page load speed if the script is heavy or slow.
    * *Usage:* JavaScript tags are often preferred for rich media and when advanced measurement is needed, while iFrames offer better security and simplicity. Ad servers typically provide both options.

---

## X. Budgeting & Bidding Strategies

### **70. Explain how DV360's automatic bidding strategies work (e.g., tCPA, tROAS, Maximize Conversions, Maximize Viewability).**

* **Answer:** Automatic (or Algorithmic) bidding strategies leverage Google's machine learning to adjust bids in real-time for each individual auction based on the likelihood of achieving a specific campaign goal, using a vast range of contextual and user signals.
    * **Target CPA (tCPA):** Aims to get as many conversions as possible at or below the target Cost Per Acquisition (CPA) you set. Bids are raised for auctions deemed likely to convert and lowered for less promising ones. Requires sufficient conversion data.
    * **Target ROAS (tROAS):** Aims to maximize conversion value while achieving an average Return On Ad Spend (ROAS) target you set. Bids are adjusted based on predicted conversion value relative to cost. Requires conversion tracking with values passed.
    * **Maximize Conversions:** Aims to get the most possible conversions within your budget, without targeting a specific CPA. Bids automatically to capture conversion opportunities.
    * **Maximize Conversion Value:** Aims to maximize the total value of conversions within your budget, without targeting a specific ROAS. Focuses on high-value conversions.
    * **Maximize Viewability (using Active View tCPM):** Aims to maximize the number of viewable impressions by bidding higher for inventory predicted to have high viewability, targeting a specific viewable CPM goal.

### **71. What is the difference between Fixed (Manual) bidding and Automatic (Algorithmic) bidding? When might you prefer one over the other?**

* **Answer:**
    * **Fixed (Manual) Bidding:** You manually set a specific maximum bid price (e.g., ₹300 CPM, ₹10 CPC). The system will not bid higher than this set amount. Requires constant monitoring and manual adjustments based on performance data.
        * *Prefer When:* You need absolute control over maximum bids, have very specific performance insights dictating precise bids, lack sufficient conversion data for automated strategies, or are testing very specific inventory segments.
    * **Automatic (Algorithmic) Bidding:** You set a performance goal (tCPA, tROAS, Max Viewability, etc.), and the platform's algorithms automatically adjust bids for each auction in real-time based on predicted likelihood of achieving that goal.
        * *Prefer When:* You have clear performance goals (especially conversion-based), sufficient data volume for algorithms to learn, want to leverage machine learning for optimization across many signals, or want to reduce manual bid management effort. Generally recommended for performance-focused campaigns with adequate data.

### **72. What does Target CPA (tCPA) bidding optimize towards? What is required for it to work effectively?**

* **Answer:** tCPA bidding optimizes towards achieving **conversions** (as defined by your Floodlight or conversion tracker) at or below a specific average **Cost Per Acquisition (CPA)** that you set as the target. It automatically sets bids higher or lower based on the calculated probability of a user converting in that specific auction.
    * **Required for Effectiveness:** Sufficient conversion volume is crucial. Google generally recommends a minimum number of conversions (e.g., 15-30 conversions within the last 30 days, though more is better) for the specific conversion goal the tCPA strategy is optimizing towards, allowing the algorithm enough data to learn effectively. Accurate conversion tracking must be in place.

### **73. What does Target ROAS (tROAS) bidding optimize towards? What input does it require?**

* **Answer:** tROAS bidding optimizes towards maximizing **conversion value** while achieving a target **Return On Ad Spend (ROAS)**. ROAS is calculated as (Conversion Value / Ad Cost) * 100%. The algorithm bids higher for auctions predicted to result in high-value conversions and lower for less valuable ones, aiming for the average ROAS target you set.
    * **Required Input:** Requires conversion tracking that passes dynamic **conversion values** (e.g., the actual revenue from a sale) back to the platform via Floodlight tags or other tracking methods. Also requires sufficient conversion volume with associated values for learning.

### **74. What does Target CPM (tCPM) bidding optimize for in the context of YouTube?**

* **Answer:** In the context of YouTube campaigns focused on **Brand awareness and reach**, Target CPM (tCPM) bidding optimizes bids to maximize unique reach or deliver impressions efficiently. You set an average target CPM you're willing to pay, and the system tries to achieve that average while reaching as many relevant users as possible.

### **75. What does Viewable CPM (Active View - tCPM) bidding optimize for?**

* **Answer:** Viewable CPM (often referred to as Target Viewable CPM or tCPM optimizing for viewability) optimizes bids specifically to maximize the number of **viewable impressions** according to the MRC standard (50% pixels for 1 sec display / 2 secs video). You set a target average CPM for these viewable impressions, and the system bids higher on inventory predicted to be highly viewable. It prioritizes viewability over just serving impressions.

### **76. How does the "Maximize Conversions" bid strategy work?**

* **Answer:** The Maximize Conversions bid strategy automatically sets bids to help get the **most possible conversions** for your campaign while spending your budget. It doesn't target a specific CPA; instead, it tries to capture every available conversion opportunity within the daily or flight budget constraints. It's useful when the primary goal is volume of conversions, and you're less concerned about hitting a precise CPA target for every conversion, as long as the budget is spent efficiently towards generating conversions.

### **77. Can you adjust bids based on specific targeting dimensions (e.g., audience list, demographic, geo)?**

* **Answer:** While DV360's automated bidding strategies largely manage bids automatically at the auction level, you *can* influence bidding indirectly or apply adjustments in certain scenarios:
    * **Bid Multipliers (Less Common with Full Automation):** In some contexts or with certain manual/semi-manual strategies, you might apply bid multipliers (e.g., bid +20% for a specific high-value audience list). However, fully automated strategies like tCPA/tROAS incorporate these signals internally, making manual multipliers less necessary or even counterproductive.
    * **Segmenting Line Items:** A common approach is to create separate Line Items for high-priority segments (e.g., a dedicated LI for remarketing audiences with a potentially higher tCPA goal than a prospecting LI). This allows the bid strategy to optimize differently for distinct segments.
    * **Custom Bidding:** Advanced users can create custom bidding scripts using Python, allowing for highly specific bid adjustments based on virtually any combination of dimensions available to the platform.

---

## XI. Floodlights & Conversion Tracking

### **78. What is a Floodlight tag? What platform generates it?**

* **Answer:** A Floodlight tag is a piece of HTML code (typically an image pixel or JavaScript) used for conversion tracking within the Google Marketing Platform. It's generated by **Campaign Manager 360 (CM360)**. When placed on an advertiser's website (e.g., on a purchase confirmation page or lead submission thank-you page), it fires when a user completes that action, sending data back to CM360/DV360 servers.

### **79. What are the two main types of Floodlight activities (Counter vs. Sales)? When would you use each?**

* **Answer:**
    * **Counter Activity:** Used to count the *number of times* users perform a specific action (e.g., visiting a key webpage, signing up for a newsletter, submitting a lead form). Each firing counts as one conversion event. Use when the value of each conversion is the same, or you're just tracking volume.
    * **Sales Activity:** Used to track the *number of sales* made or the *number of items purchased*, and crucially, allows capturing the **monetary value** of each transaction. Use for e-commerce purchases or any conversion where capturing revenue or variable value is important (e.g., tracking different subscription values).

### **80. What is the difference between a Standard and a Unique counter Floodlight?**

* **Answer:** This applies to Counter activities:
    * **Standard:** Counts *every* conversion that happens after a user clicks or views an ad within the lookback window, even if the same user converts multiple times.
    * **Unique:** Counts only the *first* conversion per unique user within each 24-hour period (midnight to midnight, US Eastern Time). Useful for tracking actions like leads or sign-ups where you only want to count each individual user once per day, regardless of how many times they submit the form.

### **81. What are Custom Floodlight Variables (`u=` variables)? Give an example of how they might be used.**

* **Answer:** Custom Floodlight Variables allow you to capture additional, non-personally identifiable information (passed dynamically from the advertiser's website) alongside the standard conversion data when a Floodlight tag fires. They use the `u=` parameter in the tag (e.g., `u1=value1;u2=value2`).
    * **Example:** An airline advertiser could use custom variables on their booking confirmation Floodlight tag to capture:
        * `u1=[booking_class]` (e.g., "economy", "business")
        * `u2=[trip_type]` (e.g., "oneway", "roundtrip")
        * `u3=[destination_region]` (e.g., "europe", "asia")
    * This data can then be used in CM360/DV360 reporting for deeper analysis (e.g., which campaigns drive more business class bookings?) or potentially for building more granular audience lists.

### **82. For Sales tags, what key variables are typically captured (`qty=`, `cost=`, `ord=`)?**

* **Answer:** Sales activity tags are designed to capture transactional details:
    * `qty=[quantity]`: The number of items sold in the transaction. Required if the counting method is "Items Sold".
    * `cost=[revenue]`: The total monetary value (revenue) of the transaction. Required if the counting method is "Transactions" and you want to track value for ROAS calculations.
    * `ord=[order_id]`: A unique identifier for the transaction (e.g., Order ID, Confirmation Number). This is crucial for preventing duplicate conversion counting if a user refreshes the confirmation page. It should be a unique value for each transaction.

### **83. What are common methods for implementing Floodlight tags on a website?**

* **Answer:**
    * **Google Tag Manager (GTM):** The recommended method. Floodlight tags can be easily configured and deployed via GTM containers without needing to directly edit website code for every tag update. GTM allows for easier management of triggers (when the tag should fire) and variables (data to capture).
    * **Direct Placement (Hardcoding):** Placing the Floodlight tag code directly into the HTML source code of the relevant webpages. Requires developer resources and is less flexible than GTM.
    * **Platform Integrations:** Some e-commerce platforms or CMS might have specific integrations or plugins designed to facilitate Floodlight implementation.

### **84. How can you verify if a Floodlight tag is implemented correctly and firing?**

* **Answer:**
    * **Google Tag Assistant (Chrome Extension):** Install the extension, enable it, and navigate to the webpage where the Floodlight should fire (e.g., the thank-you page after submitting a form). Trigger the action. Tag Assistant will list detected Google tags, including Floodlights, and show their status (Green=OK, Red=Error). Click on the Floodlight tag to see details like Activity ID, Group ID, and custom variables passed.
    * **Browser Developer Tools (Network Tab):** Open Dev Tools (usually F12), go to the Network tab. Filter requests by "fls.doubleclick.net" or the specific Floodlight ID. Trigger the conversion action. Look for a successful network request (Status 200 OK) to the Floodlight server (`fls.doubleclick.net`). Inspect the request payload/URL to ensure the correct parameters (Activity ID, Group ID, `ord=`, `u=` vars, `cost=`, `qty=`) are being sent.
    * **CM360/DV360 Reporting:** Check the conversion reports in the platform. After some delay (minutes to hours), you should start seeing conversions attributed to your test clicks/views if everything is working and linked correctly. Look for expected volume and values.
    * **CM360 Floodlight Implementation Report:** This report in CM360 can show firing frequency and identify pages with potential implementation issues, though it's less real-time than browser tools.

### **85. How are Floodlight conversions linked back to DV360 campaigns?**

* **Answer:** The linkage happens through user identifiers and attribution logic:
    1.  **Ad Interaction:** When a user sees (impression) or clicks on an ad served via DV360 (and trafficked through CM360), a Google Marketing Platform cookie (or other identifier like Mobile ID) is associated with that user and interaction.
    2.  **Conversion Event:** When the same user later visits the advertiser's site and triggers a Floodlight tag (e.g., makes a purchase), the tag fires and sends information back to CM360/DV360 servers, including the user's GMP identifier.
    3.  **Attribution:** The system checks if this user's identifier matches one associated with a recent ad interaction (within the defined click-through and view-through lookback windows). If a match is found based on the chosen attribution model, the conversion is credited to the corresponding DV360 campaign, IO, LI, creative, etc.

### **86. What is an attribution model? Can you name a few common models?**

* **Answer:** An attribution model is a rule, or set of rules, that determines how credit for conversions is assigned to different advertising touchpoints (clicks, impressions) along a user's path to conversion. It helps understand which channels or interactions contribute most effectively.
    * **Common Models:**
        * **Last Click:** Gives 100% credit to the very last click before the conversion.
        * **First Click:** Gives 100% credit to the first click in the user's journey.
        * **Linear:** Distributes credit equally across all clicks in the path.
        * **Time Decay:** Gives more credit to clicks closer in time to the conversion.
        * **Position-Based (U-Shaped):** Gives more credit to the first and last clicks (e.g., 40% each), distributing the remaining 20% among middle interactions.
        * **Data-Driven Attribution (DDA):** Uses machine learning algorithms to analyze actual conversion paths and assigns credit based on the calculated contribution of each touchpoint (available in GMP, requires sufficient data).

### **87. How do lookback windows work for Floodlight conversions (click-through vs. view-through)?**

* **Answer:** Lookback windows define the period *before* a conversion occurs during which a preceding ad interaction (click or impression) is eligible to receive credit. They are set within CM360's Floodlight configuration.
    * **Click-Through Lookback Window:** The maximum time allowed between a user *clicking* an ad and completing a conversion for that click to be credited. (e.g., 30 days). If a user clicks an ad and converts 35 days later, a 30-day window means that click won't get credit.
    * **View-Through Lookback Window:** The maximum time allowed between a user *seeing* (viewable impression) an ad and completing a conversion *without clicking* for that impression to be credited. This window is typically much shorter than the click-through window (e.g., 1 day, 7 days). It helps measure the impact of viewable ads that influence conversions even without a direct click.

---

## XII. Measurement, KPIs & Reporting

### **88. What are the most important metrics to monitor for an Awareness campaign?**

* **Answer:** Impressions, Reach, Frequency, Viewable Impressions, Viewability Rate (%), Viewable CPM (vCPM), Cost Per Mille (CPM), Video Completion Rate (VCR - especially % complete), Audio Completion Rate, Brand Lift study results (if applicable).

### **89. What metrics are key for a Consideration or Traffic-driving campaign?**

* **Answer:** Clicks, Click-Through Rate (CTR), Cost Per Click (CPC), Site Visits/Sessions, Pages per Session, Bounce Rate, Time on Site, Video View Rate (VTR - % viewed), Cost Per View (CPV), Engagement Rate (for specific engagement actions).

### **90. What are the primary metrics for a Conversion-focused campaign?**

* **Answer:** Conversions (Total, Post-Click, Post-View), Conversion Rate (CVR), Cost Per Acquisition (CPA) or Cost Per Lead (CPL), Revenue (Total Conversion Value), Return On Ad Spend (ROAS), Average Order Value (AOV).

### **91. Can you write down the formulas for CTR, VCR, CPA, ROAS, and Viewability Rate?**

* **Answer:**
    * `CTR = (Total Clicks / Total Impressions) * 100%`
    * `VCR = (Total Video Completions / Total Video Starts or Views) * 100%`
    * `CPA = Total Cost / Total Conversions`
    * `ROAS = (Total Conversion Value (Revenue) / Total Cost) * 100%` (Often expressed as a ratio, e.g., 4:1, which equals 400%)
    * `Viewability Rate = (Viewable Impressions / Measurable Impressions) * 100%`

### **92. Where in DV360 can you find performance reporting? What dimensions and metrics are commonly analyzed?**

* **Answer:** Performance reporting is found in several places within DV360:
    * **Dashboard View:** High-level overview of campaign/IO/LI performance against goals.
    * **Insights Tab:** Includes various pre-built reports like Audience Performance, Placement Performance, Creative Performance, Geo Performance, Basic Reports (Standard Report Builder).
    * **Offline Reporting (Report Builder):** The most powerful option. Allows creating highly customized reports by selecting specific dimensions, metrics, date ranges, and filters. Reports can be run once or scheduled.
    * **Common Dimensions Analyzed:** Date, Campaign, IO, LI, Creative, Audience List, Placement (Site/App), Device Type, Geography, Environment, Viewability Bucket, Time of Day, etc.
    * **Common Metrics Analyzed:** Impressions, Clicks, CTR, Views, VTR, Completions, VCR, Conversions (Total, Post-Click, Post-View), CPA, Revenue, ROAS, Spend, CPM, vCPM, CPC, Reach, Frequency, Viewability Rate.

### **93. What is the difference between a standard Impression and a Viewable Impression?**

* **Answer:**
    * **Standard Impression:** Counted when an ad creative is successfully fetched and begins to load on the user's device/page. It *doesn't* guarantee the user actually saw the ad (it could have loaded below the fold or been scrolled past quickly).
    * **Viewable Impression:** Counted only if the ad meets the industry standard (MRC) criteria for having an *opportunity* to be seen: at least 50% of the ad's pixels in view on the screen for at least 1 continuous second (for display ads) or 2 continuous seconds (for video ads). Viewability metrics provide a better measure of whether ads had a chance to make an impact.

### **94. How do you interpret Video Completion Rate (VCR) data (e.g., 25%, 50%, 75%, 100%)?**

* **Answer:** VCR data shows how engaging your video creative is by indicating how much of it users are watching.
    * **High Start Rate (vs Impressions):** Indicates the video loads correctly.
    * **High 25% / 50% Completion:** Shows users are initially engaged and watch past the early seconds (important for skippable ads).
    * **High 75% Completion:** Suggests strong engagement through the majority of the video.
    * **High 100% Completion (Complete):** Indicates users watched the entire video message. This is a strong signal of interest and message delivery, especially valuable for branding or detailed product explanations.
    * **Drop-off Analysis:** Analyzing where users drop off (e.g., a sharp drop between 25% and 50%) can provide insights into parts of the video that might be less engaging or where messaging could be improved. VCR benchmarks vary significantly based on ad length, format (skippable vs non-skip), placement, and targeting.

---

## XIII. Optimization Techniques & Troubleshooting

### **95. Your campaign is underpacing significantly. What steps would you take to troubleshoot and fix it?**

* **Answer:** Underpacing means not spending the budget fast enough. Here’s a practical checklist:
    1.  **Check Basics:** Are the IO/LI active? Are the dates correct? Is there budget assigned? Simple things first!
    2.  **Check Bids:** Are your bids too low compared to auction win rates or floor prices? Gradually increase fixed bids or check if automated bidding goals (tCPA/tROAS) are too restrictive for current performance. The system won't bid if it can't meet the target. Try relaxing the target a bit.
    3.  **Check Targeting:** Is your audience too small or too niche? Are you targeting only a very small area? Do you have too many negative keywords or website exclusions blocking delivery? Try carefully broadening the targeting (e.g., add relevant audiences, remove excessive restrictions).
    4.  **Check Inventory:** Are you limiting yourself to only specific websites or deals? Is that inventory actually available? Try allowing access to more exchanges or check if the Deal IDs are active.
    5.  **Check Restrictions:** Are frequency caps too aggressive? Is viewability targeting too high (>70-80% can severely limit scale)? Are brand safety filters overly restrictive? Try slightly loosening these *if* appropriate.
    6.  **Check Creatives:** Are all your ads approved? Do you have ads for all the sizes needed for the placements you're targeting?

### **96. Your campaign is overpacing. What adjustments would you make?**

* **Answer:** Overpacing means spending too fast, risking finishing the budget early. To slow it down:
    1.  **Check Pacing Setting:** Make sure it's set to 'Even' if you want smooth delivery.
    2.  **Lower Bids:** If using manual bids, reduce them gradually. If using automatic bids, make the target stricter (e.g., lower the tCPA target, increase the tROAS target).
    3.  **Narrow Targeting:** Focus more on the best-performing audiences, locations, or device types. Pause things that aren't working well or are very expensive. Add more negative keywords or placements.
    4.  **Tighten Restrictions:** Lower the frequency cap (e.g., from 5 per day to 3 per day). If viewability isn't the main goal, you could slightly increase the target threshold. Apply stricter brand safety if needed.
    5.  **Optimize Creatives:** Pause low-performing creatives that might be winning bids inefficiently.
    6.  **Shift Budget:** Maybe move some budget to another campaign/IO that needs it more and is performing well but under budget.

### **97. A Line Item has a very low CTR. What are potential causes and how would you try to improve it?**

* **Answer:** Low CTR means people see the ad but don't click. Reasons could be:
    * **Boring/Irrelevant Ad:** The creative (image/text) isn't interesting or doesn't match what the audience cares about.
    * **Wrong Audience:** Showing the ad to people who are simply not interested in the offer.
    * **Bad Placements:** Ad showing on cluttered websites or places where clicks are unlikely.
    * **No Clear Call-to-Action (CTA):** The ad doesn't tell people what to do (e.g., "Click Here," "Learn More," "Shop Now").
    * **Ad Fatigue:** People have seen the same ad too many times.
    * **How to Improve:**
        * **Test Creatives:** Try different images, headlines, colours, and especially different CTAs. Make it eye-catching and clear what the benefit is.
        * **Refine Audience:** Check if the audience targeting is correct. Pause audiences with very low CTR. Try more specific audiences.
        * **Check Placements:** Look at the placement report. Block websites/apps with lots of impressions but zero clicks. Focus on better quality sites.
        * **Refresh Ads:** If ads have been running long, introduce new versions to combat ad fatigue.

### **98. Viewability for a campaign is below target. What optimization tactics could you employ?**

* **Answer:** If ads aren't being seen enough (low viewability):
    * **Target for Viewability:** In LI settings, set a minimum viewability percentage target (e.g., >60%). The system will try to buy only slots predicted to meet this.
    * **Use Viewable Bidding:** Use the 'Target Viewable CPM' (Active View tCPM) bid strategy.
    * **Check Placements:** Analyze reports to find websites/apps with low viewability scores and block them. Create allowlists of known high-viewability sites.
    * **Use Deals:** PMP deals often offer higher viewability inventory from premium publishers.
    * **Check Creatives:** Some ad sizes naturally have better viewability (e.g., vertical sizes). Make sure your ads load quickly (optimize file size).

### **99. Conversion volume is low, but Floodlights seem to be firing correctly. What areas would you investigate?**

* **Answer:** If tracking is okay, but conversions are low, look at the user journey:
    1.  **Is the Ad Relevant?** Does the ad promise something the landing page delivers? Is the targeting reaching people actually likely to convert? Check audience performance.
    2.  **Landing Page Issues:** Is the landing page loading fast? Is it easy to use, especially on mobile? Is the offer clear? Is the 'buy' or 'sign up' button easy to find and use? Test it yourself!
    3.  **Traffic Quality:** Are you getting lots of clicks from low-quality websites or apps that never convert? Check the placement report and block bad sources.
    4.  **Offer / Competition:** Is the product/offer itself attractive? What are competitors offering? Maybe the price/value isn't right?
    5.  **Attribution:** Are conversions happening, but maybe being credited to other channels if using Last Click model? Check different attribution models. Check if view-through conversions are being tracked.
    6.  **Bidding:** Is your bid strategy (like tCPA) set too restrictively, preventing bids on potentially converting users?

### **100. How would you approach optimizing a campaign towards a lower CPA?**

* **Answer:** Lowering CPA (Cost Per Acquisition/Conversion) means getting conversions more cheaply:
    1.  **Focus on What Works:** Analyze reports – find the audiences, placements, creatives, devices, times of day that already give good CPA. Shift more budget towards these winners.
    2.  **Cut Waste:** Pause or exclude anything with high spend and high CPA (poor performing audiences, placements, geos). Be strict about cutting things that don't bring results efficiently.
    3.  **Improve Conversion Rate:** This is key!
        * Make sure ads match the landing page exactly.
        * Work on making the landing page better (faster, clearer, easier to convert).
        * Test ad creatives with stronger offers or clearer calls-to-action.
    4.  **Refine Bidding:** Use tCPA bidding and set a realistic target. If performance improves, you can gradually try lowering the target CPA.
    5.  **Negative Targeting:** Use negative keywords (contextual) and exclude irrelevant audiences.

### **101. How would you optimize towards a higher ROAS?**

* **Answer:** Higher ROAS (Return On Ad Spend) means getting more revenue back for every rupee spent. Focus on value:
    1.  **Track Value:** Make sure Floodlight Sales tags are correctly capturing the revenue amount for each conversion.
    2.  **Use Value Bidding:** Use tROAS or Maximize Conversion Value bid strategies. These focus on getting high-value sales, not just any sale.
    3.  **Find High-Value Sources:** Analyze reports to see which audiences, products, placements, or campaigns drive the most *revenue* (not just conversions). Focus budget there.
    4.  **Target High-Value Customers:** If possible, target past high-spending customers (via Customer Match) or audiences known to have higher purchasing power.
    5.  **Promote Profitable Items:** If possible, focus ads on higher-margin products.
    6.  **Dynamic Ads:** Use dynamic creatives to show relevant products, especially effective for e-commerce remarketing.

### **102. How do you approach optimizing placements in DV360?**

* **Answer:** Optimizing placements is very important for getting good value and protecting the brand.
    1.  **Regularly Check Reports:** Look at the Placement report (found under Insights). Sort by Spend to see where the money is going. Check performance metrics (CTR, Conversions, CPA, Viewability) for each site/app.
    2.  **Identify Bad Placements:** Find sites/apps spending significant budget with poor performance (high CPA, low CTR, low viewability) or those that are clearly irrelevant/unsafe for the brand.
    3.  **Create Blocklists (Exclusions):** Add these poor-performing or unsafe URLs/apps to a Placement blocklist and apply it to your Line Items or IOs. This stops wasting money there.
    4.  **Identify Good Placements:** Note down placements that consistently perform well and are brand-safe.
    5.  **Consider Allowlists (Optional):** For very high control (often needed for specific brand safety or performance goals), create an Allowlist containing *only* the approved, high-performing placements. Apply this to the Line Item – it will *only* run on these specified sites/apps. This drastically limits reach but maximizes control.
    6.  **Use Verification Data:** If using IAS/DV/Moat, check their reports for flagged placements based on viewability, fraud, or brand safety issues and add them to blocklists.

### **103. What steps do you take to optimize audience targeting mid-flight?**

* **Answer:** Audience performance can change, so mid-flight checks are needed:
    1.  **Analyze Audience Performance Report:** Check which specific audience lists (First-party, Google, Third-party, Custom) are driving results (conversions, low CPA, high ROAS) and which are just spending money.
    2.  **Allocate Budget:** Shift budget away from underperforming audiences towards the top performers.
    3.  **Refine Targeting:** Pause audiences that are clearly not working after giving them a fair chance.
    4.  **Add Negative Audiences:** If you identify characteristics of users who click but never convert, try creating an audience of those users to exclude them.
    5.  **Test New Audiences:** Carefully introduce new, relevant audiences (e.g., a new In-Market segment, a Similar Audience based on recent converters) with a small test budget to see if they perform well.
    6.  **Check Audience Overlap:** Use the Audience Composition report to see if your different audiences are overlapping a lot. If so, simplify by pausing redundant ones.

### **104. How do you optimize creative performance in DV360?**

* **Answer:** Making sure the ads themselves work well is vital:
    1.  **Use Creative Rotation Wisely:** Start with 'Even' rotation to give all creatives a fair chance for testing. After getting enough data (impressions/clicks), switch to 'Optimized' rotation to let DV360 automatically show the best performers more often.
    2.  **A/B Test Elements:** Don't just test completely different ads. Test variations – different headlines, different images, different button colours, different Calls-to-Action (CTAs). Find out which *elements* drive better results.
    3.  **Analyze Creative Reports:** Regularly check the Creative report to see which specific ads have the best CTR, Conversion Rate, Viewability, etc. Pause the ones that are clearly underperforming.
    4.  **Refresh Creatives:** Ads get old ('ad fatigue'). Introduce new creatives regularly (e.g., every few weeks or months, depending on campaign intensity) to keep things fresh and maintain performance.
    5.  **Match Creative to Audience:** Ensure the message and visual style of the creative strongly resonates with the specific audience segment you are targeting with that Line Item.
    6.  **Consider Dynamic Creative (DCO):** For product-focused campaigns, use DCO to automatically show the most relevant products or messages to each user, which usually improves performance.

### **105. How do you balance multiple KPIs (e.g., maintaining high Viewability while achieving a low CPA)?**

* **Answer:** Balancing different goals can be tricky, as optimizing for one might hurt another (e.g., highest viewability inventory often costs more, increasing CPA). Strategies include:
    1.  **Prioritize:** Understand which KPI is *most* important for the campaign's success. Is the main goal conversions (CPA is primary), or is it branding (Viewability is primary)? Focus optimization efforts there first.
    2.  **Set Realistic Targets:** Don't aim for perfection on all metrics simultaneously. Set achievable targets for both primary and secondary KPIs.
    3.  **Segment Strategy:** Use different Line Items for different priorities.
        * Have one LI heavily optimized for conversions (tCPA bidding, targeting lower funnel audiences) even if viewability is just okay.
        * Have another LI focused on reaching users with high viewability (vCPM bidding, targeting broader audiences on premium placements) where CPA might be higher or not the main focus.
    4.  **Find the Sweet Spot:** Analyze performance across different viewability levels or placement types. Maybe inventory with 60-70% viewability converts almost as well as 80%+ viewability inventory but costs much less. Find the balance point that delivers acceptable performance on both metrics within budget.
    5.  **Use Weighted Goals (Advanced):** Custom Bidding algorithms could potentially be set up to optimize towards a combined score based on multiple weighted KPIs, but this requires advanced setup.

### **106. My automated bid strategy isn't performing well (e.g., high CPA, not spending). What should I check first?**

* **Answer:** If automated bidding (like tCPA, tROAS) isn't working as expected:
    1.  **Conversion Tracking:** Is it working perfectly? Are conversions being recorded accurately and quickly? Are values being passed correctly (for tROAS)? Without good data, the algorithm can't work. Check Floodlights using Tag Assistant / Network tools.
    2.  **Conversion Volume:** Is there enough recent conversion data for the algorithm to learn properly? (Rule of thumb: often need 15-30+ conversions in the last 30 days for the *specific goal* it's optimizing for). If volume is too low, the algorithm struggles. Consider optimizing towards an upper-funnel conversion (micro-conversion) temporarily or using a broader strategy initially.
    3.  **Learning Period:** Has the strategy had enough time to learn? Automated bidding usually needs several days (sometimes up to a week or two) after being enabled or after major changes to stabilize performance. Avoid making constant changes during this period.
    4.  **Target Realism:** Is your target CPA too low or your target ROAS too high compared to historical performance or what's realistically achievable? If the target is impossible, the algorithm might severely limit bids and reduce spending/delivery. Try setting a more achievable target initially.
    5.  **Budget Constraints:** Is the budget too small relative to the target CPA/ROAS? If your tCPA is ₹1000, but your daily budget is only ₹500, the system might struggle to get even one conversion per day to optimize effectively. Ensure budget allows for several conversions per day ideally.
    6.  **Other Restrictions:** Are overly narrow targeting, very high viewability targets, or strict brand safety rules limiting the algorithm's ability to find eligible impressions where it predicts a conversion might happen?

---

## XIV. Programmatic Deals

### **107. What is a Private Marketplace (PMP) deal? How is it set up in DV360?**

* **Answer:** A PMP is like a VIP section of the ad market. A publisher invites specific advertisers to bid on their special inventory (often premium placements). It's an auction, but only for those invited, usually with a minimum price (floor price).
    * **Setup:** The publisher gives the advertiser a unique 'Deal ID'. In DV360, you create a Line Item, go to 'Inventory Source', choose 'Deals', and enter this Deal ID. Your LI will then bid only on inventory available through that specific deal.

### **108. What is a Programmatic Guaranteed (PG) deal? What are its key characteristics?**

* **Answer:** PG is like booking a specific ad spot directly with the publisher, but using technology to manage it.
    * **Characteristics:** Fixed Price (CPM agreed upfront), Guaranteed Volume (you are promised a certain number of impressions), runs on specific inventory for specific dates. It offers predictability like old direct deals but with programmatic efficiency.
    * **Setup:** Also uses a Deal ID provided by the publisher, entered in the LI's Inventory Source settings. The LI settings (budget, dates, CPM) must match the agreed terms.

### **109. Why would an advertiser choose to use PMP or PG deals instead of relying solely on the Open Auction?**

* **Answer:** For better control and quality:
    * **Quality Placements:** Get access to better, often premium, ad spots.
    * **Brand Safety:** Higher confidence that ads will appear in safe, appropriate environments.
    * **Transparency:** Know exactly which websites/apps your ads are running on.
    * **First Look:** PMPs might offer access to inventory before it goes to the open market.
    * **Guaranteed Delivery (PG):** Ensures your ad runs in a specific place for important campaigns.
    * **Reaching Niche Audiences:** Access specific audiences available only through certain premium publishers.

---

## XV. Industry Landscape

### **110. What changes did the advertising industry see after the implementation of GDPR law in the European Union?**

* **Answer:** GDPR (General Data Protection Regulation) forced major changes, especially around user privacy:
    * **Consent Became Key:** Websites needed clear user consent (opt-in) before collecting or using personal data for tracking/targeting, leading to the rise of Consent Management Platforms (CMPs or cookie banners).
    * **Data Restrictions:** Stricter rules on what data could be collected and how it could be used (purpose limitation, data minimization).
    * **User Rights:** Users gained more rights (like accessing or deleting their data).
    * **Targeting Impact:** Reduced reliance on third-party data; increased focus on first-party data and contextual targeting.
    * **Compliance Burden:** Companies needed to ensure their processes and tech partners were compliant, leading to audits and process changes.

### **111. What is Brand safety and how does it work?**

* **Answer:** Brand safety is about protecting a brand's reputation by ensuring its ads don't appear next to harmful, inappropriate, or objectionable content (like hate speech, fake news, violence, etc.).
    * **How it works:**
        * **Content Analysis:** Technology scans web pages/videos to understand their content and categorize them (e.g., news, sports, sensitive topics).
        * **Platform Controls (DV360):** Advertisers set rules in the platform to avoid certain sensitive categories, specific keywords, or low-quality digital content labels.
        * **Blocklists:** Maintaining lists of specific unsafe websites/apps to exclude.
        * **Third-Party Verification:** Using tools like IAS, DoubleVerify, Moat that provide an extra layer of protection by checking inventory before bidding (pre-bid) or reporting where ads appeared after serving (post-bid).

---
