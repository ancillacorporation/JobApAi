# Privacy Policy

Last updated: september 26 2025

This Privacy Policy explains how AutoApAI (the “Extension”) processes information to provide its features. By using the Extension, you agree to this policy.

## What the Extension does

AutoApAI helps you complete job applications by generating suggestions based on:

- Text you provide (e.g., CV/resume, job description, application form text)
- Optional account credentials if you choose to sign up/sign in (email/password)

## Data the Extension processes

- User-provided content: CV/resume text, job description text, application form text
- Optional OpenAI API key (BYOK): If you choose to bring your own key, it is stored locally in Chrome Sync storage and used only to call OpenAI on your behalf
- Optional auth session: If you choose to sign up/sign in, an access token is stored locally in Chrome Sync storage to maintain your session
- Technical identifiers: A locally generated client identifier may be used to manage free-trial usage limits

## How data is used

- Content generation: Your provided text is sent to OpenAI to generate resumes, cover letters, and form suggestions
- Trial enforcement: A usage counter (with a minimal identifier) is maintained to enforce a free-trial limit
- Optional authentication: If you sign up/sign in, requests to Supabase are used to validate your account

## Where data goes

Depending on your settings:

- OpenAI: The Extension may send your content to the OpenAI API (either using your BYOK key or via our backend during the free trial). We do not sell your data. See OpenAI’s policies for how they handle request data
- Our backend (hosted on Vercel): When you do not use BYOK, generation requests may be proxied through our backend to apply trial limits
- Supabase: If you choose to create an account or sign in, the Extension communicates with our Supabase project for authentication and trial usage tracking

## What we do NOT do

- No analytics or advertising trackers
- No sale of personal data
- No background collection without user action: The Extension processes text only when you use its features

## Data retention

- BYOK key and auth session tokens are stored locally on your device (Chrome Sync). You can clear them anytime via the Options page or by uninstalling the Extension
- Trial usage counters are stored in our database to enforce the free-trial limit. Request content (your pasted text) is not stored by our backend beyond processing

## Security

- All communications with OpenAI, our backend, and Supabase use HTTPS
- BYOK keys are never transmitted to us when you choose to call OpenAI directly from the Extension

## Children’s privacy

The Extension is not directed to children under the age of 13, and we do not knowingly collect data from children

## Contact

If you have questions or requests regarding this policy, contact: clientservice@ancillaco.com
