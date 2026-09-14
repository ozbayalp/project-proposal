# CampusSwipe

A swipe-based internship and job app for university students. Students swipe through roles, recruiters swipe through students, and a mutual right-swipe opens a chat.

## Team

- [Alp Ozbay](https://github.com/ozbayalp)

## What and why?

Applying to internships means filling out the same form on twenty portals and hearing nothing back. Recruiters have the opposite problem: one campus posting pulls thousands of applications, mostly from people who didn't read it.

CampusSwipe makes interest mutual. You build one profile, then swipe on roles you want. Recruiters only see students who already swiped on their posting, so every match means both sides said yes. Postings are tied to specific universities, which keeps the pool small enough that swiping still means something.

## For whom?

Students first: NYU undergrads recruiting for internships and new-grad roles, starting with CS majors. They're my classmates, so I can hand them a build and watch them use it instead of guessing.

Recruiters second: alumni hiring at their companies and startup founders looking for interns. They're reachable through campus networks and more open to a new channel than a big company's recruiting team.

Plus a small admin role to verify schools and employers and remove junk postings.

## How?

- **Student profile** — school, major, grad year, skills, links, résumé. Filled out once.
- **Role postings** — recruiters tag each role with type, field, location, and which schools can see it.
- **Student deck** — cards of roles open to your school; tap to expand, swipe right for interested.
- **Recruiter deck** — only students who already swiped on that role.
- **Matches and chat** — both swipe right, a conversation opens.
- **Filters** — students by type, field, location; recruiters by major, grad year, skills.
- **Dashboard** — what you swiped on, what matched, active chats.

Example: a junior signs up, confirms she's at NYU, fills out her profile, and sets preferences to software internships in New York. She swipes right on seven roles. That night a recruiter opens his queue, sees her card, likes her GitHub, and swipes right. They match and he asks when she's free for a screen. No application form involved.

Stretch goals: résumé parsing to auto-fill profiles, a recommendation system that reorders the deck, interview scheduling inside chats.

## Scope

Two separate user experiences plus a shared matching layer, so it's not a one-screen app. The data side covers students, employers, roles, per-school eligibility, swipes, matches, and messages, and the recruiter queue has to be built from incoming swipes rather than just listing everyone. Add résumé uploads, chat, and a mobile UI where the swipe has to feel right.

It's still doable: auth, CRUD, a filtered feed, a match check, and a chat thread are all known problems, the risky ideas are in stretch goals, and launching at one school keeps seeding and moderation small. For four to six people the work splits into the student side, the recruiter side, matching and messaging, and the data model underneath.