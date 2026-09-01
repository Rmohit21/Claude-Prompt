# Prompt for Claude in Chrome — Find UI/UX Designer Jobs → Export to Excel

Use this with the **Claude for Chrome** extension so it browses job boards on your behalf and hands you back an Excel file.

## Prompt (copy & paste)

> You are browsing on my behalf in Chrome. Find **UI/UX Designer** jobs that are **currently hiring in Ahmedabad, Gujarat, India** for someone with **1.5+ years of experience**, then compile everything into an **Excel (.xlsx) spreadsheet** I can download.
>
> **Where to search** (open each in a tab and collect results):
> 1. Indeed — https://in.indeed.com/jobs?q=UI+UX+Designer&l=Ahmedabad%2C+Gujarat
> 2. LinkedIn Jobs — https://www.linkedin.com/jobs/search/?keywords=UI%20UX%20Designer&location=Ahmedabad
> 3. Naukri — https://www.naukri.com/ui-ux-designer-jobs-in-ahmedabad
> 4. Foundit (Monster) — https://www.foundit.in/search/ui-ux-designer-jobs-in-ahmedabad
>
> **Filter rules — only keep a job if ALL are true:**
> - Title is UI/UX Designer or close (UX Designer, UI Designer, Product Designer, Interaction Designer, Visual/Web Designer).
> - Required experience is **1.5+ years** — include listings asking "1–3 years" or "1.5 to 3 years". **Exclude** fresher/0-year roles and senior/lead roles needing 5+ years.
> - Location is **Ahmedabad** (on-site, hybrid, or remote roles open to Ahmedabad are fine).
> - Posted within the **last 30 days** where the date is shown.
>
> **Build the spreadsheet with these columns (one row per job):**
> | # | Job Title | Company | Location | Work Mode | Experience Required | Key Skills | Posted Date | Salary (if listed) | Source Site | Application Link |
>
> **Rules for the output:**
> - De-duplicate jobs that appear on more than one site (keep the one with the most detail; note other sources in the same row).
> - Sort by **Posted Date**, newest first.
> - Put the newest / best-fit matches for ~1.5–2 years experience at the top and **bold** those rows.
> - Add a first sheet named **"Summary"** with: total jobs found, count per source site, and the date range of postings. Put the job list on a second sheet named **"Jobs"**.
> - Keep every **Application Link** as a live clickable hyperlink.
> - Do not invent data — if a field isn't listed on the page, leave it blank.
>
> When finished, **give me the .xlsx file to download** and a one-paragraph summary of how many jobs you found and the top 3 you'd apply to first.

## Notes

- If a site asks you to log in (LinkedIn, Naukri), pause and let me sign in, then continue.
- Respect each site's pagination — collect at least the first 2–3 pages of results per site before filtering.
- If any site is blocked or shows a CAPTCHA, skip it and note that in the Summary sheet.

## Quick tweaks

- **Different city:** replace "Ahmedabad" everywhere with your city.
- **Different experience:** change "1.5+ years" and the include/exclude rules.
- **More/fewer boards:** add or remove URLs in the "Where to search" list.
