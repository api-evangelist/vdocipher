# VdoCipher (vdocipher)

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
