
[comment]: # (Generated from JSON file by generate_feedback_md.py)
[comment]: # (Intended to be read in GitHub's markdown renderer. Apologies if the plaintext formatting is messy.)

# LukeBriggsDev's OWASP Falihax Hackathon Feedback
*Marked by [CyberSoc](https://cybersoc.org.uk/?r=falihax-marking-lukebriggsdev)*

This is LukeBriggsDev's specific feedback. See below for the full vunerability list, including ones you may have missed.

[General hackathon feedback with full vulnerability list and solutions](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md)
## Summary
**Total mark:** 42

A great project, with clearly a huge amount of effort put in! You were able to notice many of the subtle vulnerabilities we left in there that not everyone could!

## Marking Scheme Used
We used the following marking scheme to award marks for each vulnerability, where the mark awarded for the vulnerability is the highest row in the following table fulfilled by your solution. A tick means you had to have done this to get the mark, a cross means this mark does not apply if you did this, and a dash means this is ignored for this possible mark. This mark scheme was decided after the entries had been submitted and was not known to entrants during the competition, although hints were provided as to what to include for good marks.

For each vulnerability, this is how many marks we would award:
| State a valid vulnerability | Show where it is in code | Demo it | Describe how it could be mitigated | Attempt a reasonable fix | Fix works | Explain your fix | Marks |
|-----------------------------|--------------------------|---------|------------------------------------|--------------------------|-----------|------------------|-------|
| ✔                           | ❌                        | ❌       | ❌                                  | ❌                        | -         | -                | 1     |
| ✔                           | ✔                        | ❌       | ❌                                  | ❌                        | -         | -                | 2     |
| ✔                           | -                        | ✔       | ❌                                  | ❌                        | -         | -                | 3     |
| ✔                           | -                        | -       | ✔                                  | ❌                        | -         | -                | 4     |
| ✔                           | -                        | -       | -                                  | ✔                        | ❌         | -                | 4     |
| -                           | -                        | ❌       | -                                  | ✔                        | ✔         | ❌                | 5     |
| -                           | -                        | ✔       | -                                  | ✔                        | ✔         | ❌                | 6     |
| -                           | -                        | -       | -                                  | ✔                        | ✔         | ✔                | 7     |

## Vulnerabilites Found
### [A01-02: No access control/owner check on account page](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a01-02-no-access-control/owner-check-on-account-page)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 5    |

In e69b986 you fix this bug successfully, however it would have been more efficient to use the existing [`get_accounts()`](https://github.com/LukeBriggsDev/owasp-falihax/blob/094245dde0e14bd3e1f90e42a265fa5a0e586d2f/app.py#L377-L422) function to save yourself some work here!


### [A01-03: No access control on the admin page](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a01-03-no-access-control-on-the-admin-page)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 5    |


### [A02-01: Unsuitable use of ROT-13 "encryption"](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a02-01-unsuitable-use-of-rot-13-encryption)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 5    |


### [A02-02: Random number generation is not secure](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a02-02-random-number-generation-is-not-secure)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 5    |


### [A03-01: SQL Injection](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a03-01-sql-injection)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 5    |


### [A04-02: No Password Strength Checks](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a04-02-no-password-strength-checks)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ❌           | ❌         | ❌           | 1    |


### [A04-03: No Rate Limiting](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a04-03-no-rate-limiting)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ❌           | ❌         | ❌           | 1    |


### [A05-01: Flask secret key used is not secure](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a05-01-flask-secret-key-used-is-not-secure)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ❌     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 5    |


### [A05-02: Flask debug mode is left enabled](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a05-02-flask-debug-mode-is-left-enabled)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ❌           | ❌         | ❌           | 1    |


### [A08-01: Missing Validation for Lower Bound of Transaction Amount](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a08-01-missing-validation-for-lower-bound-of-transaction-amount)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 5    |


### [A09-01: No Logging](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#a09-01-no-logging)
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ❌           | ❌         | ❌           | 1    |


### [B02-01: Bad or No Input Validation (General Cases)](https://github.com/CyberSoc-Newcastle/owasp-falihax/blob/main/VULNS.md#b02-01-bad-or-no-input-validation-general-cases)
*Maximum mark of 1 for this category*
| State | Show | Demo | Mitigate | Attempt fix | Fix works | Explain fix | Mark |
|-------|------|------|----------|-------------|-----------|-------------|------|
| ✔     | ❌    | ❌    | ❌        | ✔           | ✔         | ❌           | 1    |

## Bonus marks
Bonus marks were awarded for great non-security critical things that really stood out to us, specific to your project. Each entry below gets you one bonus mark.

### Nicely formatted readme
Your readme file is really nicely formatted using markdown, which makes it a pleasure to read. I particularly liked your use of links to commits to show where you had fixed things, which made marking so much easier!

*+1 bonus mark awarded.*

### Great commit messages
Your commits are done often, and in a (mostly) atomic way which is great practice. Your commit messages are informative, accurate and concise, and really show how the progress of development well!

*+1 bonus mark awarded.*

## Total mark
5 + 5 + 5 + 5 + 5 + 1 + 1 + 5 + 1 + 5 + 1 + 1 + 1 + 1 = 42

**Your total mark is 42**