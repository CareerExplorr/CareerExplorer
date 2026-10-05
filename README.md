=
CAREER EXPLORER  (Career Skill Tree)
=

Explore 7,706 US jobs across 267 careers and 23 fields: the skills each job
uses, the talents it grows or lets fade, what it takes to get in, and how
hard it is to switch from one job to another.

Live site:  https://careerexplorr.github.io/CareerExplorer/

No sign-up and no install. The site runs entirely in your browser.


------------------------------------------------------------------------------
 QUICK START: HOW TO USE THE SITE
------------------------------------------------------------------------------

The site has two tabs at the top: Explorer and Career switch.

EXPLORER

  1. Find a job. Type in the search box (job titles, other names for a job,
     careers or skills), or open the tree: field > career > branch > job.

  2. Read the job card. It shows the 10 skills that set the job apart, its
     talent scores, the career's 50 core skills and the 20 universal skills.

  3. Look at the surface (the 3D chart). Green peaks are talents a job
     grows, red dips are talents it lets fade, on a scale of -5 to +5.
       - Drag to rotate, scroll to zoom, or use 3D / Map / Side and + / -.
       - All fields: every field side by side. Click a field to see its
         careers, then click a career to open it.
       - This career: every job in one career.
       - Compare jobs: jobs you have added with the Compare button
         (up to 40, from any field).

  4. Highlight what matters to you.
       - Click a talent name beside the surface to highlight it across
         every row. Click it again to remove it. You can highlight several.
       - Click a point on the surface to pin it. It stays highlighted with
         its value until you click the same point again.
       - The bar under the surface lists what is highlighted. It also has
         a "Highlight a talent..." menu (handy on phones) and Clear all.

CAREER SWITCH

  1. In "From", pick your current job.
  2. In "To", pick a job or a whole career.
     (Or press "Plan a switch" on any job card, or try an example.)
  3. Read the result:
       - Verdict: Close move, Moderate move, Big move or Major career
         change, with a breakdown of what drives it.
       - Education and credentials: the typical path in, new licenses or
         certificates you would need, what employers often prefer, and a
         rough timeline.
       - Stepping stones: a route through one or two in-between jobs, shown
         when it is easier than going direct.
       - Easiest next moves from your job, and easiest ways into the target.
       - Skills: which ones you already have, partly have, or need to learn.
       - Talent shift: what you would lean on more, and use less.
  4. Click any job in the results to plan that move instead, or use Swap to
     reverse the direction.


------------------------------------------------------------------------------
 ABOUT THE PROJECT
------------------------------------------------------------------------------

WHAT IS IN THE DATA

  23 fields              Healthcare, Engineering, Trades, Military, and more
  267 careers            each with 50 core skills and its own set of
                         tailored talents
  7,706 jobs             each with 10 skills that set it apart from
                         neighboring jobs
  18,938 job titles      job names plus other names people search for
  20 universal skills    skills every job uses
  24 shared talents      one common scale, so jobs from different fields
                         can be compared on the same surface
  Entry requirements     education level, typical path in, required and
                         preferred credentials, and years to qualify, for
                         every career, plus overrides for specialties

  The layers stack: every job has the 20 universal skills, its career's 50
  core skills, and its own 10. None of a job's 10 repeats a universal skill.

HOW THE CAREER SWITCH ESTIMATE WORKS

  Each move gets a score from 0 (same job) to 1 (start over), built from:

    40%  education and credentials you do not have yet
    35%  core skills of the target career you are missing
    15%  skills that set the target job apart that you are missing
    10%  difference in talent scores

  Skill gaps count for more when the target takes longer to learn. Skills
  are matched by meaning, not exact wording, so a related skill you already
  have counts as partial credit. Score bands:

    under 0.25   Close move
    0.25-0.40    Moderate move
    0.40-0.60    Big move
    0.60 and up  Major career change

  Stepping stones are only suggested when the route is easier overall than
  going direct, and they never send you far backward in education or
  seniority or past the target in seniority.

PROJECT FILES

  index.html          The whole site: page layout, styles and code
  data/meta.js        Fields, careers, core skills, search index
  data/d-*.js         One file per field (23 files), loaded only when needed
  data/switch.js      Career switch data: skill vocabulary, entry
                      requirements, precomputed next moves and ways in
  _config.yml         GitHub Pages settings (index.html does not use the
                      theme)
  LICENSE             MIT License
  README.md           Short description shown on the GitHub repo page
  README.txt          This file

  Keep index.html and the data folder side by side. The page looks for its
  data in data/, so moving the .js files elsewhere breaks the site.

HOW IT IS BUILT

  Plain HTML, CSS and JavaScript. No frameworks, no build step, no server,
  no database, no cookies and no analytics. The only outside request is for
  web fonts from Google Fonts. Light and dark mode follow your system
  setting. The 3D surface is drawn on an HTML canvas.

RUN IT ON YOUR COMPUTER

  Option 1: double-click index.html to open it in your browser.
  Option 2: open a terminal in this folder and run

      python -m http.server 8000

  then go to http://localhost:8000

------------------------------------------------------------------------------
 IMPORTANT NOTES
------------------------------------------------------------------------------

  - Skill lists, talent scores and entry requirements are expert-informed
    estimates built from standard job descriptions, licensing and training
    requirements, and professional society specialties. They are not survey
    data.
  - Duties, pay and licensing rules vary by employer, state and seniority.
    Check your state's licensing board before you commit to a path.
  - Switch scores compare typical requirements. Your own experience,
    location and employer can make a move easier or harder.
  - US jobs only.


------------------------------------------------------------------------------
 LICENSE AND CREDITS
------------------------------------------------------------------------------

  MIT License, Copyright (c) 2026 alex-m-0. See the LICENSE file.
  Made with AI.
