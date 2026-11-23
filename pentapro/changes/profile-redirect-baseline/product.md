# PRODUCT · Profile redirect baseline

Confirmed from [index.html](../../../index.html): the current page declares English and redirects visitors to `https://github.com/teknolista` using both a zero-delay meta refresh and `window.location.replace`. A visible body link provides a manual path; the same URL is canonical. README describes the profile website.

Proposed IDs: REDIRECT-01 keeps those four destinations consistent; REDIRECT-02 keeps the visible fallback link usable when script execution is unavailable. A future change must define whether redirecting remains intended before replacing it with a new website. Expected failure case: automatic navigation unavailable leaves a visible destination link. Browser behavior, timing and external destination availability were not tested.
