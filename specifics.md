What it is

    A job-matching app for people starting out
    You give it your resume, it finds and ranks the jobs that fit you best
    Runs on an open-weight model, locally, so your resume stays on your computer

Who it’s for

    Students looking for part-time jobs and internships
    Recent grads applying for first jobs
    Career changers with transferable skills
    Not for recruiters

The problem

    Job boards return thousands of irrelevant results
    Keyword search misses good fits
    Distance is ignored, even though in-person applying works well for beginners
    Most tools send your resume to a third-party server
    “Entry level” postings often hide unrealistic requirements

What it does

    Reads and structures your resume
    Matches jobs by meaning, not keywords
    Scores jobs higher the closer they are to you
    Explains why you fit, what’s missing, and how to close the gap
    Suggests resume rewording based only on what’s already in your resume
    Flags red flags in postings

How the location scoring works

    Each job gets a fit score and a proximity score
    Final score = fit x (1 - w) + proximity x w
    w is adjustable, so someone with a car can turn it down
    Remote jobs aren’t penalized
    Users enter a neighbourhood or postal area, not an exact address
    Nearby jobs get a “walk-in” tag

How the AI is used

    Parse the resume
    Match it to each job
    Explain the match and the gaps
    Verify every claim against the resume so nothing is invented
    Model: Gemma or Qwen through Ollama

Tech (to be confirmed)

    Backend: Python + FastAPI
    Frontend: React + Vite
    Data: sample job postings with coordinates
    Location: distance calculated locally

Known limits

    Job data is a sample set, since scraping job boards breaks their terms
    Distance is a rough proxy for your chances
    Smaller models are faster but less accurate

Next steps

    Pick a name
    Confirm the tech stack
    Build the MVP: paste resume, enter location, get a ranked list
