# VdoCipher (vdocipher)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

VdoCipher is a secure video hosting platform that delivers Hollywood-grade DRM (Google Widevine and Apple FairPlay) encrypted streaming for e-learning and OTT businesses. Its server-side REST API handles video upload, media management, folders, dynamic viewer watermarking, and OTP/playbackInfo generation for authorized playback, all secured with an Apisecret authorization header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/apis.yml)

## Tags

- Video
- Secure Video Hosting
- DRM
- Streaming
- E-Learning
- OTT
- Watermarking

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### VdoCipher Videos API

List, search, retrieve, edit, and delete videos in a VdoCipher account. Supports pagination, folder scoping, free-text query, and tag filtering over the video library.

- **Human URL:** [https://www.vdocipher.com/docs/server/videomanagement/listing/](https://www.vdocipher.com/docs/server/videomanagement/listing/)
- **Base URL:** `https://dev.vdocipher.com/api`

#### Tags

- Videos
- Media Management
- Listing
- Search

#### Properties

- [Documentation](https://www.vdocipher.com/docs/server/videomanagement/listing/)
- [API Reference](https://www.vdocipher.com/docs/server/)
- [OpenAPI](openapi/vdocipher-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vdocipher.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vdocipher.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### VdoCipher Upload API

Obtain short-lived AWS S3 upload credentials (clientPayload) and a new videoId, then upload a source file directly to storage and poll transcoding status until the video is ready.

- **Human URL:** [https://www.vdocipher.com/docs/server/upload/credentials/](https://www.vdocipher.com/docs/server/upload/credentials/)
- **Base URL:** `https://dev.vdocipher.com/api`

#### Tags

- Upload
- Ingest
- Credentials

#### Properties

- [Documentation](https://www.vdocipher.com/docs/server/upload/credentials/)
- [API Reference](https://www.vdocipher.com/docs/server/upload/status/)
- [OpenAPI](openapi/vdocipher-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vdocipher.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vdocipher.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### VdoCipher OTP & Playback Credentials API

Generate a one-time otp and playbackInfo pair on the back end for a specific video so the DRM-protected player can authorize a single viewing session, with optional TTL, dynamic watermark, and IP/geo restrictions.

- **Human URL:** [https://www.vdocipher.com/docs/server/playbackauth/otp/](https://www.vdocipher.com/docs/server/playbackauth/otp/)
- **Base URL:** `https://dev.vdocipher.com/api`

#### Tags

- OTP
- Playback
- Authentication
- DRM

#### Properties

- [Documentation](https://www.vdocipher.com/docs/server/playbackauth/otp/)
- [API Reference](https://www.vdocipher.com/docs/server/playbackauth/offline/)
- [OpenAPI](openapi/vdocipher-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vdocipher.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vdocipher.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### VdoCipher Folders API

Create, list sub-folders under, and search a hierarchical folder tree (rooted at "root") used to organize the video library.

- **Human URL:** [https://www.vdocipher.com/docs/server/videomanagement/folder-create/](https://www.vdocipher.com/docs/server/videomanagement/folder-create/)
- **Base URL:** `https://dev.vdocipher.com/api`

#### Tags

- Folders
- Organization

#### Properties

- [Documentation](https://www.vdocipher.com/docs/server/videomanagement/folder-create/)
- [API Reference](https://www.vdocipher.com/docs/server/videomanagement/folder-search/)
- [OpenAPI](openapi/vdocipher-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vdocipher.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vdocipher.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### VdoCipher Watermark API

Attach a dynamic, per-viewer annotation (text, RTMP, or image watermark) to a playback session via the OTP request annotate parameter, burning identifying marks such as the viewer email or IP over the DRM stream.

- **Human URL:** [https://www.vdocipher.com/docs/server/playbackauth/otp/](https://www.vdocipher.com/docs/server/playbackauth/otp/)
- **Base URL:** `https://dev.vdocipher.com/api`

#### Tags

- Watermark
- Annotation
- Security

#### Properties

- [Documentation](https://www.vdocipher.com/docs/server/playbackauth/otp/)
- [OpenAPI](openapi/vdocipher-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vdocipher.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vdocipher.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### VdoCipher Meta & Files API

Retrieve detailed metadata for a video and list its associated files - poster images, captions/subtitles, and rendition assets - plus list and search the tags applied across the library.

- **Human URL:** [https://www.vdocipher.com/docs/server/videomanagement/files/list/](https://www.vdocipher.com/docs/server/videomanagement/files/list/)
- **Base URL:** `https://dev.vdocipher.com/api`

#### Tags

- Metadata
- Files
- Posters
- Captions

#### Properties

- [Documentation](https://www.vdocipher.com/docs/server/videomanagement/files/list/)
- [API Reference](https://www.vdocipher.com/docs/server/videomanagement/files/posters/)
- [OpenAPI](openapi/vdocipher-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vdocipher.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vdocipher.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/VdoCipher)
- [LinkedIn](https://www.linkedin.com/company/vdocipher)
- [Website](https://www.vdocipher.com/)
- [Documentation](https://www.vdocipher.com/docs/server/)
- [Plans](plans/vdocipher-plans-pricing.yml)
- [Rate Limits](rate-limits/vdocipher-rate-limits.yml)
- [Fin Ops](finops/vdocipher-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
