# Final-Group-Project-ReadMe
Final Group Project: Love and Laugh – RomCom Discovery API

By Sinafek Liyew & Abby Baumgarten
Live Site: https://loveandlaugh-romcom-site.onrender.com

Information Story & Use Case

The Problem

- Many users struggle to find romantic comedies that match how they feel. Mainstream platforms make it hard to filter by emotional tone. Users face decision fatigue, vague genre tags, and no way to search by mood.

The Story

- We created the RomCom Discovery API, a portable information product that helps users find rom-coms based on how they want to feel—cozy, hopeful, nostalgic, etc. This makes emotional discovery faster and more meaningful.

Motivation

- Rom-coms spark joy, comfort, and connection. Structuring information by emotional metadata makes it more useful to humans, not just machines. It turns a flat movie list into a guided emotional experience.


Requirements & Scope
In Scope:

    Mood-based discovery via consistent metadata

    Real-time filtering of movies by mood, genre, platform, and year

    API-driven website for simple, portable access

Out of Scope:

    User accounts or personalization

    Video playback or licensing

    Machine learning recommendations

FAIR Assessment of Existing Information Sources

- Principle	Assessment of IMDb, TMDb, OMDb, etc.
- Findable	Moderate — mostly title and genre search
- Accessible	High — public APIs available
- Interoperable	Low — inconsistent schemas and genre/platform tags
- Reusable	Limited — metadata lacks emotional or human-centered tagging


Improvements Made to the Metadata Structure

We transformed flat entertainment data into a more portable emotional metadata format:

    Controlled vocabulary for mood_tags, platforms, genre_tags

    Flattened structure into JSON with consistent keys and values

    Added new fields: poster, director_images, user_reviews, decade_summary

    Used a REST-style API to support real-time queries


System Architecture (Portable Structure)
- Layer	Technology Used
- Frontend	HTML + CSS + JavaScript
- Backend	Flask (Python)
- Data Layer	JSON file (romcom_movies_list.json) — no SQL or cloud DB
- Hosting	Render (for live deployment)
- API	GET routes like /api/movies/mood/Cozy for dynamic filtering

Quality, Performance & Security

Quality Measures:

    Used consistent tag formats (e.g., "Cozy" not "cozy")

    Validated JSON structure with online tools

    Manually checked each movie entry

    Tested API in browser and terminal

Performance:

    Fast response due to lightweight JSON backend

    Supports dynamic filtering without reloading pages

Security:

    Public read-only API

    No user login = no personal data collected = low risk

Key Takeaways

    Clean metadata = better, more emotional user experience

    Simple architecture = easy to maintain and expand

    Emotional filters = deeper connection between users and content

    Real-time filtering = fun, engaging discovery experience

Future Improvements

    Add more data — thousands of romcoms remain unlisted

    Introduce a real-time database — let users add reviews or submissions

    Automate platform availability updates

    Connect to physical stores or libraries to find rare or offline romcoms

