# Website consolidation and content maintenance

The primary club site is `https://greyhatgt.org/` (see CNAME). The homepage currently redirects to `/about/`; use `/about/` as its canonical page until the homepage architecture changes. The seven primary content pages have distinct titles, descriptions, Open Graph metadata and canonical URLs. The sitemap uses the same trailing-slash URLs; do not put redirect aliases or `index.html` duplicates into it.

This repository contains generated HTML, not the Hexo source described by the legacy README. Edits here should be preserved if the original generator is used again.

## Remaining hosting work for issue #23

1. Inventory the live response and page content of `greyhat.gatech.edu`, `greyhatgeorgiatech.github.io`, `greyhatgt.github.io` and `greyhatgt.org`. Confirm which legacy pages have equivalents and which contain unique archives before redirecting them.
2. With GT/Plesk access, configure permanent server-side redirects from duplicate pages to their corresponding primary pages. Preserve meaningful paths; do not discard unique archived content or send every legacy page to the homepage.
3. In the legacy GitHub Pages repository, configure the appropriate domain/redirect migration. This repository cannot alter another account's Pages configuration.
4. Verify that both HTTP and HTTPS aliases reach the expected HTTPS canonical URL without loops. Check the root and at least one nested page per hostname.
5. Update club profiles and bios that link to legacy domains, using the relevant account access.
6. Submit `https://greyhatgt.org/sitemap.xml` in the club's Search Console. Record the initial indexing state and search performance for “GreyHat Georgia Tech,” then compare after crawling. Rankings are not an acceptance test that a code change alone can guarantee.

WRECKCTF and Hat n Dagger are distinct sites; do not redirect them into the club site.

## Deployment

The GitHub Pages API reported legacy publishing from `master` at `/` on 2026-09-19. Target this change at `master`; merging can publish the site. The checked-in Actions workflow still targets `NewUpdatedWebsite`, so it is not the current publishing mechanism. This change does not switch Pages settings or trigger a production deployment.

## Competition results

The homepage's selected results were checked on 2026-09-19 against:

- [CSAW finals 2025](https://ctftime.org/event/2982): 18th.
- [CSAW finals 2024](https://ctftime.org/event/2567): 4th.
- [BuckeyeCTF 2024](https://ctftime.org/event/2449): 3rd.
- [CSAW finals 2023](https://ctftime.org/event/2091): 2nd.

The displayed placement is the position on the linked CTFtime scoreboard. Do not infer regional, student-only or other division ranks from it. Add photos only with an approved source and useful alt text. Optional photos and recaps are not required for the text results to work.

## Alumni and writeups

Keep existing alumni entries until graduation dates, former positions and publication preferences are verified. Sort new confirmed records by graduation date descending, then former role seniority. Do not infer real names or dates from Discord handles. New competition members and submitted writeups require the reviewed form data and captain confirmation; a CTFtime roster is not a substitute for that review.
