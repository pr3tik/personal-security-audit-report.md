# personal-security-audit-report.md
================================================================
PERSONAL SECURITY AUDIT REPORT
================================================================

Auditor:        Pratik
Audit Date:     08 May 2026
Engagement:     Personal Digital Security Assessment
Methodology:    Scope > Intelligence > Exposure > Severity > Remediation

----------------------------------------------------------------
1. SCOPE
----------------------------------------------------------------

Systems and accounts assessed:
 - Primary email:  pratik2k08@gmail.com
 - Key accounts:   Google, Instagram, WhatsApp, LinkedIn,
                   Banking App, Coursera, Amazon,
                   Internshala, GitHub

----------------------------------------------------------------
2. EXECUTIVE SUMMARY
----------------------------------------------------------------

Assessment identified 0 breach exposures but 4 significant
findings across personal accounts. Primary risks are: Google
account has no 2FA enabled despite being the master recovery
email for 5+ services; an unrecognised TV session active on
Google account; and WhatsApp has no 2FA. If the Google account
is compromised, an attacker can take over at least 5 accounts
via Forgot Password. Three remediation actions tracked for
immediate follow-up.

----------------------------------------------------------------
3. FINDINGS
----------------------------------------------------------------

CRITICAL
 [x] Google account (primary email) has 2FA OFF. This account
     is the recovery email for Coursera, LinkedIn, Amazon,
     Internshala, and GitHub — meaning 5+ accounts can be
     taken over instantly via Forgot Password if Gmail
     is compromised.

HIGH
 [x] Unrecognised Television session active on Google account.
     Location and last active time unknown. Could indicate
     unauthorised access or forgotten login on external device.
 [x] WhatsApp has 2FA OFF. Vulnerable to SIM-swap attack
     and account takeover via phone number.

MEDIUM
 [x] Google account publicly discoverable via email address
     using OSINT tool (Epieos). Google ID, Maps profile,
     and profile photo accessible without authentication.

LOW
 [x] Google Maps contribution profile linked to primary
     email, expanding public attack surface.

----------------------------------------------------------------
4. ACTIONS TAKEN DURING AUDIT
----------------------------------------------------------------

 [x] Ran primary email through HaveIBeenPwned —
     0 breaches confirmed.
 [x] Ran primary email through Epieos OSINT tool —
     Google account linkage identified and documented.
 [x] Reviewed all active Google sessions — unrecognised
     TV session identified for investigation.
 [x] Audited 2FA status across 5 key accounts —
     2 accounts found with 2FA OFF.

----------------------------------------------------------------
5. REMEDIATION PLAN
----------------------------------------------------------------

This week:
 [ ] Enable 2-Step Verification on Google account
     (use Authenticator app, not SMS).
 [ ] Enable 2-Step Verification on WhatsApp.
 [ ] Investigate and sign out of unrecognised
     Television session on Google account.

This month:
 [ ] Review Google Maps profile privacy settings.
 [ ] Audit third-party apps with Google account access
     and revoke unused ones.
 [ ] Review privacy settings to limit public
     discoverability via email.

================================================================
END OF REPORT
================================================================
