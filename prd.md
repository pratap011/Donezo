# Product Requirement Document (PRD)

## Product Name: Donezo  
**Date:** January 4, 2025

---

## 1. Introduction  

### Purpose  
To create a platform where users can manage and track their progress across various interests such as movies, TV shows, podcasts, games, skills, and more. The platform will provide insights into user activities and suggest personalized recommendations.

### Goals and Objectives:  
- Enable users to create and manage watchlists, playlists, or activity lists.
- Provide a dashboard that displays progress and activity analytics.
- Offer personalized recommendations based on user preferences and behavior.
- Allow users to create custom tags for unique tracking purposes.

---

## 2. Key Features  

### User Authentication  
- Login/Signup using email or social media (Google, X).

### List Management
- Predefined Lists available (e.g., Movies, TV Shows, Podcasts, Games, Anime, ...)
- User can create custom lists
- Add items
  - Search for Items by name (e.g. tv shows)
  - System searches database / api to display matches
  - User selects and adds the item
  - User should be able to add an item even if the database / api does not provide a match
- Track progress (e.g., completed episodes, levels, or chapters).
  - User can mark items as completed. (by default it is pending)
  - For episodic / subitems, User can mark complete upto an episode / subitem (This assumes an ordered list of subitems)
- User can view completion percentage for a list
- When viewing a list, user is shown pending items only and also items which have a higher percentage completion to be shown on top

### Dashboard Analytics  
- Visualize activity data such as:
  - Completion rates.
  - Genres watched or played.
  - Time spent on activities.
  - Monthly insights.
  - Hours / days left for 100% completion (actual watchtime)
  - Estimated time to complete (e.g based on hours spent historically)

### Recommendations  
- Suggest items to watch, play, or learn based on:
  - User preferences.
  - Past activities.
  - Popular releases.

### Custom Progress Tracking  
- Users can create and manage tags for unique goals (e.g., "Learn Guitar").
- Track time and milestones for custom activities.

---

## 3. Functional Requirements  

### Core Features  
- Tag-based content categorization.
- Add-to-list functionality for various domains.
- Dashboard with visual progress reports.
- Episode progress tracking for TV shows.
- Personalized recommendations engine.

---

## 4. Milestones  

- **Phase 1:** Basic platform with login, tag selection, list management, tracking, and custom tags.
- **Phase 2:** Add dashboard analytics.
- **Phase 3:** Implement recommendation engine and custom tags.

