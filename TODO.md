# Reddit Narrator: to do

From the app review on 2026-10-24. Verdict: **not working, not ready to market.**

- [ ] **Reddit blocks it.** Unauthenticated requests to reddit.com's .json endpoints now get "403 Blocked", even
      with a browser user agent. Options: register an app and use Reddit's official API (OAuth, rate limits and
      Reddit's developer terms apply, and the calls would need to go through your own Worker so the app secret
      stays secret), or shelve it. The site card already says "Waiting on Reddit API".
- [ ] **Third-party proxy.** As a backup it fetches through api.allorigins.win, a public CORS proxy, which sees
      every post link people open. Remove it when moving to the official API (the site's privacy policy says
      nothing is sent to Sixth Day Studios, which is true, but this third party isn't mentioned).
- [ ] **No README**, and the repo is public. Add a README; make the repo private if it ever holds an API secret.
