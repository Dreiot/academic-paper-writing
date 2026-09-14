# Reusable literature access profiles

Read this reference only when a literature-dependent manuscript task needs institutional or publisher authentication, an existing signed-in scholarly session, or an additional access account.

## Use the fixed local registry

For local Codex or Work tasks, use this user-private registry:

`$HOME/.agents/private/academic-paper-writing/literature-access-profiles.yaml`

On Windows, `$HOME` is the current user's profile directory. The registry may be created during the first credentialed literature task and extended later when the user offers another institution or publisher account. It is local configuration, not a manuscript artifact or Skill source; never add it to Git, a literature log, a prompt, or a delivered paper.

Store only routing, enrollment state, and credential-reference information in the registry:

- a stable profile identifier and user-facing label;
- institution or provider name;
- lawful login method and official entry URL;
- resource or publisher domains for which the profile may help;
- browser or connector surface that owns the authenticated session;
- an opaque credential reference when a supported secure credential store supplies one;
- the local credential backend, approved browser surface, automatic-login preference, and allowed login origins;
- whether the first human verification has been completed, who reported it, status, last verification date, and a short non-secret note.

The user may save an account name and password in a local browser password manager or operating-system credential store. Never duplicate those values in this YAML registry, a Skill or manuscript file, Git, chat, a screenshot, a log, or a model-visible tool argument. A field named `credential_ref` is only a local pointer or browser-profile label; it is not a place for the credential value. Never store a cookie, bearer or session token, API key, MFA code, recovery code, or a URL containing an embedded secret in the registry.

## Enroll once, then reuse the local session

On the first use of a profile, the user must inspect the official HTTPS entry point and redirect chain, complete any password, MFA, CAPTCHA, or consent step, and confirm that the intended account reached an entitled publisher or database page. Record only that this human verification occurred; do not record what the user typed or any resulting token value. Reuse an already recorded human verification instead of repeating enrollment for a new task or paper.

After that first human verification, default to completing authorized literature searches and reading without additional user interaction. The configured local browser may reuse its retained session, opaque token, local password-manager autofill, or operating-system credential broker. Complete ordinary login submissions and navigation through already verified official authentication routes when the browser manages the authentication information and the account, recipient and access scope remain authorized. A session timeout, sign-in page, ordinary SSO redirect, or browser-managed reauthentication alone does not require another handoff. Do not inspect developer storage, cookies, request headers, password fields, or credential-manager contents to obtain the secret. Confirm access from the resulting publisher content.

Interrupt only for an actual step the user must perform or decide: an external verification code, MFA approval, CAPTCHA, credentials that must be supplied manually, a new account, expanded permissions or consent requiring a new decision, or an authentication destination whose legitimacy cannot be established from the approved route. Ask once for the specific required action in the user's browser; never ask them to paste a code or secret into chat. Preserve the pending paper or search, avoid retrying an unchanged challenge, and resume that work after the user completes the step without asking for authorization again. Ordinary lack of subscription access should first lead to the lawful alternate-source routes below, not a request for the user to approve every unsuccessful lookup.

The account name, password, and authentication token must never be exposed to the model, copied into chat, prompts or tool arguments, printed, logged, screenshotted, exported, committed, embedded in a URL, or sent to an unrelated destination. Authentication necessarily submits the relevant credential or token over HTTPS to the verified institution, publisher, or their identity provider; that normal official authentication exchange is permitted. Do not use a local-only credential reference from Work Cloud or another hosted browser.

ChatGPT Work's in-app browser, a Chrome extension, an ordinary local browser, and a hosted browser can have separate sessions. Reuse only the session that belongs to the configured and approved local surface; the registry is not proof that a session remains valid. Confirm successful access from the requested paper or database response, while treating the scholarly page content itself like any other authorized literature source. The special confidentiality boundary applies to authentication secrets, not to ordinary paper content needed for the manuscript task.

## Add and select profiles proportionately

Do not ask every user for an institutional account on first invocation. Begin with open and already authorized sources. Offer to create or update a profile when the user proactively provides an access route or when a necessary full text is blocked and credentialed access would materially help.

Multiple profiles may coexist. Select the narrowest profile whose stated domain scope matches the source, and do not cycle through accounts merely to bypass a publisher restriction. If no profile works, try lawful alternate full text, request a user-supplied PDF, or narrow the affected claim as required by [literature-and-rhetoric.md](literature-and-rhetoric.md).

After a successful or failed attempt, update only the profile's non-secret status and last verification date. Never infer that access to one database grants access to another.
