# PIC Open — organization landing site

The front door for PIC's public GitHub presence. One static page, no dependencies, in the
visual language of the Evidence Room.

**Repo naming requirement:** for this to serve at the org's root URL, this repository must
be named exactly `polymerindustrycluster.github.io` (replace polymerindustrycluster with the actual org handle). Any
other name and it becomes a project site at `/org-site/` instead.

**Before first deploy:**
1. Rename the repo to `polymerindustrycluster.github.io`.
2. Replace the one `https://github.com/polymerindustrycluster/...` link in `index.html`.
3. Settings → Pages → Source: GitHub Actions (or deploy-from-branch `main`, root — this
   site is plain enough that either works).
4. Optional custom domain: add a `CNAME` record at the DNS host pointing
   `lab.picinnovation.org` (or the chosen subdomain) to `polymerindustrycluster.github.io`, then set the
   custom domain in Settings → Pages and enforce HTTPS. Verify the domain at the org level
   first (Settings → Verified domains) so no one else can claim it.

Project sites (evidence-room, catena) automatically appear under the same domain as
`/evidence-room/`, `/catena/` — the root-relative links on this page already point there.
